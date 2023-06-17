# Comparing `tmp/fabric_cf-1.5.0b5.tar.gz` & `tmp/fabric_cf-1.5.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric_cf-1.5.0b5.tar", last modified: Sun Jun 11 23:53:29 2023, max compression
+gzip compressed data, was "fabric_cf-1.5.1rc0.tar", last modified: Sat Jun 17 02:03:54 2023, max compression
```

## Comparing `fabric_cf-1.5.0b5.tar` & `fabric_cf-1.5.1rc0.tar`

### file list

```diff
@@ -1,528 +1,528 @@
--rw-r--r--   0        0        0     2035 2023-06-08 16:24:58.544106 fabric_cf-1.5.0b5/.gitignore
--rw-r--r--   0        0        0      851 2023-06-11 12:11:40.363304 fabric_cf-1.5.0b5/Dockerfile-auth
--rw-r--r--   0        0        0      769 2023-06-08 16:24:58.545457 fabric_cf-1.5.0b5/Dockerfile-broker
--rw-r--r--   0        0        0     1037 2023-06-08 16:24:58.546156 fabric_cf-1.5.0b5/Dockerfile-cf
--rw-r--r--   0        0        0      787 2023-06-08 16:24:58.546787 fabric_cf-1.5.0b5/Dockerfile-orchestrator
--rw-r--r--   0        0        0     1071 2023-04-03 14:50:53.535054 fabric_cf-1.5.0b5/LICENSE
--rw-r--r--   0        0        0     2046 2023-04-03 14:50:53.535620 fabric_cf-1.5.0b5/README.md
--rwxr-xr-x   0        0        0       74 2023-04-03 14:50:53.535840 fabric_cf-1.5.0b5/authority.sh
--rwxr-xr-x   0        0        0       79 2023-04-03 14:50:53.535996 fabric_cf-1.5.0b5/broker.sh
--rw-r--r--   0        0        0      947 2023-04-03 14:50:53.536169 fabric_cf-1.5.0b5/cleanup_old_schema_from_schema_registry.sh
--rw-r--r--   0        0        0     2861 2023-04-03 19:02:18.268979 fabric_cf-1.5.0b5/docker-compose-kafka.yaml
--rw-r--r--   0        0        0     1560 2023-04-03 14:50:53.536634 fabric_cf-1.5.0b5/docker-compose-no-ssl-kafka.yaml
--rw-r--r--   0        0        0    10307 2023-06-08 16:24:58.547590 fabric_cf-1.5.0b5/docker-compose-test.yaml
--rwxr-xr-x   0        0        0       45 2023-04-03 14:50:53.536998 fabric_cf-1.5.0b5/docker-entrypoint.sh
--rw-r--r--   0        0        0      350 2023-04-03 14:50:53.537353 fabric_cf-1.5.0b5/env.template
--rw-r--r--   0        0        0     1135 2023-04-03 17:25:25.716942 fabric_cf-1.5.0b5/env.template.test
--rw-r--r--   0        0        0    16609 2023-04-03 14:50:53.537818 fabric_cf-1.5.0b5/fabricNo.AnyActorNoPolicy.xml
--rw-r--r--   0        0        0     6343 2023-04-03 14:50:53.538166 fabric_cf-1.5.0b5/fabric_cf/Design.md
--rw-r--r--   0        0        0       50 2023-06-11 23:52:29.563452 fabric_cf-1.5.0b5/fabric_cf/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.538462 fabric_cf-1.5.0b5/fabric_cf/actor/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.538776 fabric_cf-1.5.0b5/fabric_cf/actor/boot/__init__.py
--rw-r--r--   0        0        0    15281 2023-04-03 14:50:53.539116 fabric_cf-1.5.0b5/fabric_cf/actor/boot/configuration.py
--rw-r--r--   0        0        0     1268 2023-04-03 14:50:53.539529 fabric_cf-1.5.0b5/fabric_cf/actor/boot/configuration_exception.py
--rw-r--r--   0        0        0     2509 2023-04-03 14:50:53.539906 fabric_cf-1.5.0b5/fabric_cf/actor/boot/configuration_loader.py
--rw-r--r--   0        0        0    23003 2023-05-22 19:03:15.215562 fabric_cf-1.5.0b5/fabric_cf/actor/boot/configuration_processor.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.540419 fabric_cf-1.5.0b5/fabric_cf/actor/boot/inventory/__init__.py
--rw-r--r--   0        0        0     4969 2023-04-03 14:50:53.540687 fabric_cf-1.5.0b5/fabric_cf/actor/boot/inventory/aggregate_resource_model_creator.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.540852 fabric_cf-1.5.0b5/fabric_cf/actor/core/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.541039 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/__init__.py
--rw-r--r--   0        0        0     4907 2023-04-03 14:50:53.541250 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_actor_container.py
--rw-r--r--   0        0        0     1530 2023-04-03 14:50:53.541590 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_actor_event.py
--rw-r--r--   0        0        0     2176 2023-04-03 14:50:53.541925 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_actor_identity.py
--rw-r--r--   0        0        0    10694 2023-06-10 11:17:47.369484 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_actor_management_object.py
--rw-r--r--   0        0        0    21823 2023-06-08 16:24:58.550149 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_actor_mixin.py
--rw-r--r--   0        0        0     1918 2023-04-03 14:50:53.543106 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_actor_proxy.py
--rw-r--r--   0        0        0     1323 2023-04-03 14:50:53.543429 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_actor_runnable.py
--rw-r--r--   0        0        0     4745 2023-06-08 16:24:58.550830 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_authority.py
--rw-r--r--   0        0        0     8736 2023-04-03 14:50:53.543930 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_authority_policy.py
--rw-r--r--   0        0        0     3657 2023-06-08 16:24:58.551495 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_authority_proxy.py
--rw-r--r--   0        0        0     3367 2023-04-03 14:50:53.545583 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_authority_reservation.py
--rw-r--r--   0        0        0     6071 2023-04-03 14:50:53.545879 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_base_plugin.py
--rw-r--r--   0        0        0     2290 2023-04-03 14:50:53.546104 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_broker_mixin.py
--rw-r--r--   0        0        0     1492 2023-04-03 14:50:53.546359 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_broker_policy_mixin.py
--rw-r--r--   0        0        0     3690 2023-04-03 14:50:53.546566 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_broker_proxy.py
--rw-r--r--   0        0        0     4012 2023-04-03 14:50:53.546780 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_broker_reservation.py
--rw-r--r--   0        0        0     2442 2023-04-03 14:50:53.547038 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_callback_proxy.py
--rw-r--r--   0        0        0     9846 2023-06-08 16:24:58.551946 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_client_actor.py
--rw-r--r--   0        0        0     6811 2023-06-08 16:24:58.552430 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_client_actor_management_object.py
--rw-r--r--   0        0        0     2640 2023-04-03 14:50:53.547942 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_client_callback_proxy.py
--rw-r--r--   0        0        0     5802 2023-04-03 14:50:53.548385 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_client_policy.py
--rw-r--r--   0        0        0     7724 2023-04-03 14:50:53.548730 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_client_reservation.py
--rw-r--r--   0        0        0     1936 2023-04-03 14:50:53.548982 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_component.py
--rw-r--r--   0        0        0    10115 2023-06-08 16:24:58.553102 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_concrete_set.py
--rw-r--r--   0        0        0     2729 2023-04-03 14:50:53.549801 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_container_clock.py
--rw-r--r--   0        0        0     3976 2023-04-03 14:50:53.550228 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_container_database.py
--rw-r--r--   0        0        0     3367 2023-04-03 14:50:53.550497 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_controller.py
--rw-r--r--   0        0        0     2855 2023-06-08 16:24:58.553889 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_controller_callback_proxy.py
--rw-r--r--   0        0        0     2787 2023-04-03 14:50:53.550900 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_controller_policy.py
--rw-r--r--   0        0        0     5713 2023-06-08 16:24:58.554304 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_controller_reservation.py
--rw-r--r--   0        0        0    11714 2023-06-10 11:17:47.363525 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_database.py
--rw-r--r--   0        0        0    11127 2023-06-08 16:24:58.555213 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_delegation.py
--rw-r--r--   0        0        0     1867 2023-04-03 14:50:53.551767 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_event.py
--rw-r--r--   0        0        0     1943 2023-04-03 14:50:53.552014 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_management_object.py
--rw-r--r--   0        0        0     9824 2023-06-10 11:17:47.342899 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_mgmt_actor.py
--rw-r--r--   0        0        0     2534 2023-04-03 14:50:53.552486 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_mgmt_authority.py
--rw-r--r--   0        0        0     1452 2023-04-03 14:50:53.552674 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_mgmt_broker_mixin.py
--rw-r--r--   0        0        0     6191 2023-04-03 14:50:53.552834 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_mgmt_client_actor.py
--rw-r--r--   0        0        0     5041 2023-04-03 14:50:53.553039 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_mgmt_container.py
--rw-r--r--   0        0        0     2486 2023-06-08 16:24:58.556125 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_mgmt_controller_mixin.py
--rw-r--r--   0        0        0     5014 2023-04-03 14:50:53.553457 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_mgmt_server_actor.py
--rw-r--r--   0        0        0    11147 2023-04-03 14:50:53.553629 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_policy.py
--rw-r--r--   0        0        0     2304 2023-04-03 14:50:53.553847 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_proxy.py
--rw-r--r--   0        0        0     2290 2023-04-03 14:50:53.554059 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_proxy_factory.py
--rw-r--r--   0        0        0     1658 2023-04-03 14:50:53.554593 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_query_response_handler.py
--rw-r--r--   0        0        0    14613 2023-06-08 16:24:58.556879 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_reservation_mixin.py
--rw-r--r--   0        0        0     9388 2023-04-03 14:50:53.555129 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_reservation_resources.py
--rw-r--r--   0        0        0     5581 2023-04-03 14:50:53.555376 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_reservation_status.py
--rw-r--r--   0        0        0     8963 2023-04-03 14:50:53.555582 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_resource_control.py
--rw-r--r--   0        0        0     1336 2023-04-03 14:50:53.555785 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_response_handler.py
--rw-r--r--   0        0        0     2246 2023-04-03 14:50:53.556014 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_rpc_request_state.py
--rw-r--r--   0        0        0     5634 2023-04-03 14:50:53.556345 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_server_actor.py
--rw-r--r--   0        0        0     6415 2023-04-03 14:50:53.556589 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_server_policy.py
--rw-r--r--   0        0        0     4846 2023-04-03 14:50:53.556782 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_server_reservation.py
--rw-r--r--   0        0        0    13280 2023-04-03 14:50:53.557016 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_slice.py
--rw-r--r--   0        0        0     3548 2023-06-08 16:24:58.557394 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_substrate.py
--rw-r--r--   0        0        0     2225 2023-04-03 14:50:53.557477 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_substrate_database.py
--rw-r--r--   0        0        0     2943 2023-04-03 14:50:53.557727 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_tick.py
--rw-r--r--   0        0        0     6121 2023-04-03 14:50:53.557931 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_ticker.py
--rw-r--r--   0        0        0     1590 2023-04-03 14:50:53.558112 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_timer_queue.py
--rw-r--r--   0        0        0     1387 2023-04-03 14:50:53.558344 fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_timer_task.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.558543 fabric_cf-1.5.0b5/fabric_cf/actor/core/common/__init__.py
--rw-r--r--   0        0        0    13142 2023-06-11 12:02:17.811584 fabric_cf-1.5.0b5/fabric_cf/actor/core/common/constants.py
--rw-r--r--   0        0        0     4941 2023-06-09 00:05:34.918444 fabric_cf-1.5.0b5/fabric_cf/actor/core/common/event_logger.py
--rw-r--r--   0        0        0     5517 2023-04-03 14:50:53.559364 fabric_cf-1.5.0b5/fabric_cf/actor/core/common/exceptions.py
--rw-r--r--   0        0        0     6108 2023-04-03 14:50:53.559599 fabric_cf-1.5.0b5/fabric_cf/actor/core/common/resource_config.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.559841 fabric_cf-1.5.0b5/fabric_cf/actor/core/container/__init__.py
--rw-r--r--   0        0        0    24564 2023-04-03 14:50:53.560251 fabric_cf-1.5.0b5/fabric_cf/actor/core/container/container.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.560471 fabric_cf-1.5.0b5/fabric_cf/actor/core/container/db/__init__.py
--rw-r--r--   0        0        0     8667 2023-05-22 19:03:15.216759 fabric_cf-1.5.0b5/fabric_cf/actor/core/container/db/container_database.py
--rw-r--r--   0        0        0    19408 2023-06-08 23:49:50.449976 fabric_cf-1.5.0b5/fabric_cf/actor/core/container/globals.py
--rw-r--r--   0        0        0     9216 2023-05-22 19:03:15.217738 fabric_cf-1.5.0b5/fabric_cf/actor/core/container/maintenance.py
--rw-r--r--   0        0        0     5472 2023-04-03 14:50:53.561525 fabric_cf-1.5.0b5/fabric_cf/actor/core/container/message_service.py
--rw-r--r--   0        0        0     1508 2023-04-03 14:50:53.561724 fabric_cf-1.5.0b5/fabric_cf/actor/core/container/protocol_descriptor.py
--rw-r--r--   0        0        0    13005 2023-04-03 14:50:53.562081 fabric_cf-1.5.0b5/fabric_cf/actor/core/container/remote_actor_cache.py
--rw-r--r--   0        0        0     8040 2023-04-03 14:50:53.562299 fabric_cf-1.5.0b5/fabric_cf/actor/core/container/rpc_producer.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.562481 fabric_cf-1.5.0b5/fabric_cf/actor/core/core/__init__.py
--rw-r--r--   0        0        0    35787 2023-06-08 16:24:58.558694 fabric_cf-1.5.0b5/fabric_cf/actor/core/core/actor.py
--rw-r--r--   0        0        0     1975 2023-04-03 14:50:53.563319 fabric_cf-1.5.0b5/fabric_cf/actor/core/core/actor_identity.py
--rw-r--r--   0        0        0    15513 2023-06-08 16:24:58.559224 fabric_cf-1.5.0b5/fabric_cf/actor/core/core/authority.py
--rw-r--r--   0        0        0     4845 2023-04-03 14:50:53.563854 fabric_cf-1.5.0b5/fabric_cf/actor/core/core/authority_policy.py
--rw-r--r--   0        0        0    20447 2023-06-08 16:24:58.560183 fabric_cf-1.5.0b5/fabric_cf/actor/core/core/broker.py
--rw-r--r--   0        0        0     5914 2023-04-03 14:50:53.565067 fabric_cf-1.5.0b5/fabric_cf/actor/core/core/broker_policy.py
--rw-r--r--   0        0        0    20420 2023-06-08 16:24:58.561094 fabric_cf-1.5.0b5/fabric_cf/actor/core/core/controller.py
--rw-r--r--   0        0        0     8604 2023-05-22 19:03:15.220393 fabric_cf-1.5.0b5/fabric_cf/actor/core/core/event_processor.py
--rw-r--r--   0        0        0     5467 2023-04-03 14:50:53.565861 fabric_cf-1.5.0b5/fabric_cf/actor/core/core/inventory_slice_manager.py
--rw-r--r--   0        0        0     6171 2023-04-03 14:50:53.566145 fabric_cf-1.5.0b5/fabric_cf/actor/core/core/policy.py
--rw-r--r--   0        0        0     2042 2023-04-03 14:50:53.566366 fabric_cf-1.5.0b5/fabric_cf/actor/core/core/rpc_request_state.py
--rw-r--r--   0        0        0     8688 2023-04-03 14:50:53.566587 fabric_cf-1.5.0b5/fabric_cf/actor/core/core/ticket.py
--rw-r--r--   0        0        0    16572 2023-06-11 12:02:17.823403 fabric_cf-1.5.0b5/fabric_cf/actor/core/core/unit.py
--rw-r--r--   0        0        0    13814 2023-06-08 16:24:58.562564 fabric_cf-1.5.0b5/fabric_cf/actor/core/core/unit_set.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.567201 fabric_cf-1.5.0b5/fabric_cf/actor/core/delegation/__init__.py
--rw-r--r--   0        0        0    11038 2023-06-08 16:24:58.563343 fabric_cf-1.5.0b5/fabric_cf/actor/core/delegation/broker_delegation.py
--rw-r--r--   0        0        0     1933 2023-06-08 16:24:58.564281 fabric_cf-1.5.0b5/fabric_cf/actor/core/delegation/broker_delegation_factory.py
--rw-r--r--   0        0        0    17061 2023-06-08 16:24:58.565169 fabric_cf-1.5.0b5/fabric_cf/actor/core/delegation/delegation.py
--rw-r--r--   0        0        0     1916 2023-06-08 16:24:58.565861 fabric_cf-1.5.0b5/fabric_cf/actor/core/delegation/delegation_factory.py
--rw-r--r--   0        0        0     5364 2023-04-03 14:50:53.568399 fabric_cf-1.5.0b5/fabric_cf/actor/core/delegation/resource_ticket.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.568570 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/__init__.py
--rw-r--r--   0        0        0    31973 2023-06-11 12:03:15.196954 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/authority_reservation.py
--rw-r--r--   0        0        0     3384 2023-04-03 14:50:53.569249 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/broker_query_model_publisher.py
--rw-r--r--   0        0        0    26805 2023-04-03 14:50:53.569537 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/broker_reservation.py
--rw-r--r--   0        0        0     2992 2023-04-03 14:50:53.569880 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/claim_timeout.py
--rw-r--r--   0        0        0     4396 2023-04-03 14:50:53.570217 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/failed_rpc.py
--rw-r--r--   0        0        0     3639 2023-04-03 14:50:53.570449 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/failed_rpc_event.py
--rw-r--r--   0        0        0     2668 2023-04-03 14:50:53.570827 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/incoming_delegation_rpc.py
--rw-r--r--   0        0        0     2708 2023-04-03 14:50:53.571106 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/incoming_failed_rpc.py
--rw-r--r--   0        0        0     2274 2023-06-08 16:24:58.567390 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/incoming_poa_rpc.py
--rw-r--r--   0        0        0     2105 2023-04-03 14:50:53.571543 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/incoming_query_rpc.py
--rw-r--r--   0        0        0     2703 2023-04-03 14:50:53.571750 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/incoming_reservation_rpc.py
--rw-r--r--   0        0        0     4158 2023-04-03 14:50:53.571968 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/incoming_rpc.py
--rw-r--r--   0        0        0    11227 2023-06-08 16:24:58.568032 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/incoming_rpc_event.py
--rw-r--r--   0        0        0    65705 2023-06-10 13:31:22.126818 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/kernel.py
--rw-r--r--   0        0        0     3314 2023-04-03 14:50:53.572703 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/kernel_tick.py
--rw-r--r--   0        0        0    57828 2023-06-10 10:05:11.955290 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/kernel_wrapper.py
--rw-r--r--   0        0        0    12824 2023-06-11 12:03:03.795997 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/poa.py
--rw-r--r--   0        0        0     2363 2023-04-03 14:50:53.573675 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/predecessor_state.py
--rw-r--r--   0        0        0     2860 2023-04-03 14:50:53.573873 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/query_timeout.py
--rw-r--r--   0        0        0     1404 2023-04-03 14:50:53.574038 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/request_types.py
--rw-r--r--   0        0        0    24674 2023-06-08 20:33:57.693304 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/reservation.py
--rw-r--r--   0        0        0    92717 2023-06-08 16:24:58.573662 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/reservation_client.py
--rw-r--r--   0        0        0     9994 2023-04-03 14:50:53.575366 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/reservation_server.py
--rw-r--r--   0        0        0     3311 2023-06-08 16:24:58.574548 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/reservation_states.py
--rw-r--r--   0        0        0    21131 2023-06-08 16:24:58.575397 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/resource_set.py
--rw-r--r--   0        0        0     1614 2023-04-03 14:50:53.576176 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/retry_rpc.py
--rw-r--r--   0        0        0     1899 2023-04-03 14:50:53.576398 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/retry_rpc_event.py
--rw-r--r--   0        0        0     4128 2023-06-07 16:02:47.944144 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/rpc_executor.py
--rw-r--r--   0        0        0    32934 2023-06-08 16:24:58.576277 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/rpc_manager.py
--rw-r--r--   0        0        0     1772 2023-04-03 14:50:53.577467 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/rpc_manager_singleton.py
--rw-r--r--   0        0        0     3793 2023-06-08 16:24:58.577098 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/rpc_request.py
--rw-r--r--   0        0        0     1650 2023-06-08 16:24:58.577883 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/rpc_request_type.py
--rw-r--r--   0        0        0     1340 2023-04-03 14:50:53.578168 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/sequence_comparison_codes.py
--rw-r--r--   0        0        0    12284 2023-04-03 14:50:53.578451 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/slice.py
--rw-r--r--   0        0        0    12785 2023-06-08 16:24:58.578359 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/slice_state_machine.py
--rw-r--r--   0        0        0     8319 2023-04-03 14:50:53.578901 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/slice_table.py
--rw-r--r--   0        0        0     6527 2023-04-03 14:50:53.579044 fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/tick.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.579204 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/__init__.py
--rw-r--r--   0        0        0    39627 2023-06-10 11:17:47.358416 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/actor_management_object.py
--rw-r--r--   0        0        0     8431 2023-04-03 14:50:53.579975 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/authority_management_object.py
--rw-r--r--   0        0        0     7315 2023-06-08 16:24:58.579957 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/broker_management_object.py
--rw-r--r--   0        0        0    29438 2023-06-08 16:24:58.580834 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/client_actor_management_object_helper.py
--rw-r--r--   0        0        0     9605 2023-04-03 14:50:53.580935 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/container_management_object.py
--rw-r--r--   0        0        0     9165 2023-06-08 16:24:58.581599 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/controller_management_object.py
--rw-r--r--   0        0        0    13007 2023-04-03 14:50:53.581333 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/converter.py
--rw-r--r--   0        0        0     1624 2023-04-03 14:50:53.581543 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/error.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.581729 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/kafka/__init__.py
--rw-r--r--   0        0        0    10535 2023-06-10 11:17:47.373825 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/kafka/kafka_actor.py
--rw-r--r--   0        0        0     3509 2023-04-03 14:50:53.582317 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/kafka/kafka_authority.py
--rw-r--r--   0        0        0     8200 2023-05-22 19:03:15.226498 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/kafka/kafka_broker.py
--rw-r--r--   0        0        0     4483 2023-04-03 14:50:53.583057 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/kafka/kafka_container.py
--rw-r--r--   0        0        0     5462 2023-06-08 16:24:58.583158 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/kafka/kafka_controller.py
--rw-r--r--   0        0        0     5462 2023-04-03 14:50:53.583439 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/kafka/kafka_mgmt_message_processor.py
--rw-r--r--   0        0        0     6960 2023-05-22 19:03:15.226922 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/kafka/kafka_proxy.py
--rw-r--r--   0        0        0     5730 2023-04-03 14:50:53.583847 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/kafka/kafka_server_actor.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.584078 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/kafka/services/__init__.py
--rw-r--r--   0        0        0    24550 2023-04-03 14:50:53.584410 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/kafka/services/kafka_actor_service.py
--rw-r--r--   0        0        0     5715 2023-04-03 14:50:53.584691 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/kafka/services/kafka_authority_service.py
--rw-r--r--   0        0        0     5797 2023-04-03 14:50:53.585104 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/kafka/services/kafka_broker_service.py
--rw-r--r--   0        0        0    15846 2023-04-03 14:50:53.585409 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/kafka/services/kafka_client_actor_service.py
--rw-r--r--   0        0        0     4008 2023-04-03 14:50:53.585584 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/kafka/services/kafka_controller_service.py
--rw-r--r--   0        0        0     8228 2023-04-03 14:50:53.585867 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/kafka/services/kafka_server_actor_service.py
--rw-r--r--   0        0        0     2148 2023-04-03 14:50:53.586169 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/kafka/services/kafka_service.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.586361 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/local/__init__.py
--rw-r--r--   0        0        0    11782 2023-06-10 11:17:47.350390 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/local/local_actor.py
--rw-r--r--   0        0        0     3902 2023-04-03 14:50:53.586852 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/local/local_authority.py
--rw-r--r--   0        0        0     8391 2023-04-03 14:50:53.587036 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/local/local_broker.py
--rw-r--r--   0        0        0    10119 2023-04-03 14:50:53.587201 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/local/local_container.py
--rw-r--r--   0        0        0     9646 2023-06-08 16:24:58.584522 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/local/local_controller.py
--rw-r--r--   0        0        0     2954 2023-06-08 16:24:58.585158 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/local/local_proxy.py
--rw-r--r--   0        0        0     8655 2023-04-03 14:50:53.587724 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/local/local_server_actor.py
--rw-r--r--   0        0        0     7217 2023-04-03 14:50:53.588020 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/management_object.py
--rw-r--r--   0        0        0     7841 2023-04-03 14:50:53.588258 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/management_object_manager.py
--rw-r--r--   0        0        0     4972 2023-04-03 14:50:53.588521 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/management_utils.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.588706 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/messages/__init__.py
--rw-r--r--   0        0        0     1604 2023-04-03 14:50:53.588914 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/messages/client_mng.py
--rw-r--r--   0        0        0     1570 2023-04-03 14:50:53.589110 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/messages/event_mng.py
--rw-r--r--   0        0        0     1802 2023-04-03 14:50:53.589285 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/messages/protocol_proxy_mng.py
--rw-r--r--   0        0        0     1741 2023-04-03 14:50:53.589460 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/messages/result_client_mng.py
--rw-r--r--   0        0        0     1554 2023-04-03 14:50:53.589750 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/messages/result_event_mng.py
--rw-r--r--   0        0        0     1904 2023-04-03 14:50:53.590017 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/proxy_protocol_descriptor.py
--rw-r--r--   0        0        0    15777 2023-04-03 14:50:53.590202 fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/server_actor_management_object.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.590369 fabric_cf-1.5.0b5/fabric_cf/actor/core/plugins/__init__.py
--rw-r--r--   0        0        0     7965 2023-06-08 16:24:58.586041 fabric_cf-1.5.0b5/fabric_cf/actor/core/plugins/base_plugin.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.590945 fabric_cf-1.5.0b5/fabric_cf/actor/core/plugins/db/__init__.py
--rw-r--r--   0        0        0    35944 2023-06-10 10:20:01.563499 fabric_cf-1.5.0b5/fabric_cf/actor/core/plugins/db/actor_database.py
--rw-r--r--   0        0        0     2624 2023-05-22 19:03:15.227552 fabric_cf-1.5.0b5/fabric_cf/actor/core/plugins/db/client_database.py
--rw-r--r--   0        0        0     3792 2023-05-22 19:03:15.227772 fabric_cf-1.5.0b5/fabric_cf/actor/core/plugins/db/server_actor_database.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.591940 fabric_cf-1.5.0b5/fabric_cf/actor/core/plugins/handlers/__init__.py
--rw-r--r--   0        0        0    13211 2023-06-08 16:24:58.587306 fabric_cf-1.5.0b5/fabric_cf/actor/core/plugins/handlers/ansible_handler_processor.py
--rw-r--r--   0        0        0     2955 2023-06-08 16:24:58.587956 fabric_cf-1.5.0b5/fabric_cf/actor/core/plugins/handlers/config_token.py
--rw-r--r--   0        0        0     2286 2023-04-03 14:50:53.592660 fabric_cf-1.5.0b5/fabric_cf/actor/core/plugins/handlers/configuration_mapping.py
--rw-r--r--   0        0        0     7556 2023-06-08 16:24:58.588624 fabric_cf-1.5.0b5/fabric_cf/actor/core/plugins/handlers/handler_processor.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.593035 fabric_cf-1.5.0b5/fabric_cf/actor/core/plugins/substrate/__init__.py
--rw-r--r--   0        0        0     3612 2023-04-03 14:50:53.593263 fabric_cf-1.5.0b5/fabric_cf/actor/core/plugins/substrate/authority_substrate.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.593460 fabric_cf-1.5.0b5/fabric_cf/actor/core/plugins/substrate/db/__init__.py
--rw-r--r--   0        0        0     4365 2023-05-22 19:03:15.228408 fabric_cf-1.5.0b5/fabric_cf/actor/core/plugins/substrate/db/substrate_actor_database.py
--rw-r--r--   0        0        0    16974 2023-06-11 12:02:17.817757 fabric_cf-1.5.0b5/fabric_cf/actor/core/plugins/substrate/substrate_mixin.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.594246 fabric_cf-1.5.0b5/fabric_cf/actor/core/policy/__init__.py
--rw-r--r--   0        0        0    28295 2023-04-03 14:50:53.594548 fabric_cf-1.5.0b5/fabric_cf/actor/core/policy/authority_calendar_policy.py
--rw-r--r--   0        0        0     8891 2023-04-03 14:50:53.595030 fabric_cf-1.5.0b5/fabric_cf/actor/core/policy/broker_calendar_policy.py
--rw-r--r--   0        0        0    64810 2023-05-22 19:03:15.229809 fabric_cf-1.5.0b5/fabric_cf/actor/core/policy/broker_simpler_units_policy.py
--rw-r--r--   0        0        0    19840 2023-05-22 19:03:15.230194 fabric_cf-1.5.0b5/fabric_cf/actor/core/policy/controller_calendar_policy.py
--rw-r--r--   0        0        0     9815 2023-05-22 19:03:15.230558 fabric_cf-1.5.0b5/fabric_cf/actor/core/policy/controller_simple_policy.py
--rw-r--r--   0        0        0     9546 2023-05-22 19:03:15.231097 fabric_cf-1.5.0b5/fabric_cf/actor/core/policy/controller_ticket_review_policy.py
--rw-r--r--   0        0        0     1814 2023-04-03 14:50:53.596494 fabric_cf-1.5.0b5/fabric_cf/actor/core/policy/fifo_queue.py
--rw-r--r--   0        0        0     2981 2023-04-03 14:50:53.596828 fabric_cf-1.5.0b5/fabric_cf/actor/core/policy/inventory.py
--rw-r--r--   0        0        0     2785 2023-04-03 14:50:53.597031 fabric_cf-1.5.0b5/fabric_cf/actor/core/policy/inventory_for_type.py
--rw-r--r--   0        0        0    14503 2023-06-08 16:24:58.590425 fabric_cf-1.5.0b5/fabric_cf/actor/core/policy/network_node_control.py
--rw-r--r--   0        0        0    28393 2023-06-11 17:59:15.642600 fabric_cf-1.5.0b5/fabric_cf/actor/core/policy/network_node_inventory.py
--rw-r--r--   0        0        0     5435 2023-04-03 14:50:53.597856 fabric_cf-1.5.0b5/fabric_cf/actor/core/policy/network_service_control.py
--rw-r--r--   0        0        0    22745 2023-04-03 14:50:53.598106 fabric_cf-1.5.0b5/fabric_cf/actor/core/policy/network_service_inventory.py
--rw-r--r--   0        0        0     2032 2023-04-03 14:50:53.598641 fabric_cf-1.5.0b5/fabric_cf/actor/core/policy/queue_wrapper.py
--rw-r--r--   0        0        0     5157 2023-04-03 14:50:53.598857 fabric_cf-1.5.0b5/fabric_cf/actor/core/policy/resource_control.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.599020 fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/__init__.py
--rw-r--r--   0        0        0     1821 2023-04-03 14:50:53.599277 fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/actor_location.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.599432 fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/kafka/__init__.py
--rw-r--r--   0        0        0     8301 2023-06-08 16:24:58.590907 fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/kafka/kafka_authority_proxy.py
--rw-r--r--   0        0        0     8924 2023-06-08 16:24:58.591543 fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/kafka/kafka_broker_proxy.py
--rw-r--r--   0        0        0     6744 2023-06-08 16:24:58.592307 fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/kafka/kafka_proxy.py
--rw-r--r--   0        0        0     4809 2023-04-03 14:50:53.600099 fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/kafka/kafka_proxy_factory.py
--rw-r--r--   0        0        0     9066 2023-06-11 12:09:33.224327 fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/kafka/kafka_retun.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.600601 fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/kafka/services/__init__.py
--rw-r--r--   0        0        0    12672 2023-06-08 16:24:58.593264 fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/kafka/services/actor_service.py
--rw-r--r--   0        0        0     7627 2023-06-08 16:24:58.593681 fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/kafka/services/authority_service.py
--rw-r--r--   0        0        0     8288 2023-06-08 16:24:58.594292 fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/kafka/services/broker_service.py
--rw-r--r--   0        0        0     1380 2023-04-03 14:50:53.601562 fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/kafka/services/controller_service.py
--rw-r--r--   0        0        0    19171 2023-06-11 02:28:17.565157 fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/kafka/translate.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.601999 fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/local/__init__.py
--rw-r--r--   0        0        0     4948 2023-06-08 16:24:58.595991 fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/local/local_authority.py
--rw-r--r--   0        0        0     5754 2023-06-08 16:24:58.596719 fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/local/local_broker.py
--rw-r--r--   0        0        0     6924 2023-06-08 16:24:58.597398 fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/local/local_proxy.py
--rw-r--r--   0        0        0     2868 2023-04-03 14:50:53.604580 fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/local/local_proxy_factory.py
--rw-r--r--   0        0        0     6762 2023-06-08 16:24:58.598180 fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/local/local_return.py
--rw-r--r--   0        0        0     8222 2023-06-08 16:24:58.598835 fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/proxy.py
--rw-r--r--   0        0        0     3013 2023-04-03 14:50:53.605545 fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/proxy_factory.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.605762 fabric_cf-1.5.0b5/fabric_cf/actor/core/registry/__init__.py
--rw-r--r--   0        0        0     7672 2023-04-03 14:50:53.605950 fabric_cf-1.5.0b5/fabric_cf/actor/core/registry/actor_registry.py
--rw-r--r--   0        0        0     2177 2023-04-03 14:50:53.606181 fabric_cf-1.5.0b5/fabric_cf/actor/core/registry/callback_registry.py
--rw-r--r--   0        0        0     4926 2023-04-03 14:50:53.606408 fabric_cf-1.5.0b5/fabric_cf/actor/core/registry/peer_registry.py
--rw-r--r--   0        0        0     3912 2023-04-03 14:50:53.606565 fabric_cf-1.5.0b5/fabric_cf/actor/core/registry/proxy_registry.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.606740 fabric_cf-1.5.0b5/fabric_cf/actor/core/time/__init__.py
--rw-r--r--   0        0        0     7165 2023-04-03 14:50:53.606931 fabric_cf-1.5.0b5/fabric_cf/actor/core/time/actor_clock.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.607146 fabric_cf-1.5.0b5/fabric_cf/actor/core/time/calendar/__init__.py
--rw-r--r--   0        0        0     8224 2023-04-03 14:50:53.607463 fabric_cf-1.5.0b5/fabric_cf/actor/core/time/calendar/authority_calendar.py
--rw-r--r--   0        0        0     1667 2023-04-03 14:50:53.607755 fabric_cf-1.5.0b5/fabric_cf/actor/core/time/calendar/base_calendar.py
--rw-r--r--   0        0        0    11573 2023-04-03 14:50:53.607991 fabric_cf-1.5.0b5/fabric_cf/actor/core/time/calendar/broker_calendar.py
--rw-r--r--   0        0        0     9733 2023-04-03 14:50:53.608213 fabric_cf-1.5.0b5/fabric_cf/actor/core/time/calendar/client_calendar.py
--rw-r--r--   0        0        0     5239 2023-04-03 14:50:53.608505 fabric_cf-1.5.0b5/fabric_cf/actor/core/time/calendar/controller_calendar.py
--rw-r--r--   0        0        0     2550 2023-04-03 14:50:53.608738 fabric_cf-1.5.0b5/fabric_cf/actor/core/time/calendar/source_calendar.py
--rw-r--r--   0        0        0    15769 2023-04-03 14:50:53.609015 fabric_cf-1.5.0b5/fabric_cf/actor/core/time/term.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.609215 fabric_cf-1.5.0b5/fabric_cf/actor/core/util/__init__.py
--rw-r--r--   0        0        0     2213 2023-04-03 14:50:53.609476 fabric_cf-1.5.0b5/fabric_cf/actor/core/util/bids.py
--rw-r--r--   0        0        0     2905 2023-04-03 14:50:53.609992 fabric_cf-1.5.0b5/fabric_cf/actor/core/util/client.py
--rw-r--r--   0        0        0     2063 2023-04-03 14:50:53.610294 fabric_cf-1.5.0b5/fabric_cf/actor/core/util/graceful_interrupt_handler.py
--rw-r--r--   0        0        0     2163 2023-04-03 14:50:53.610582 fabric_cf-1.5.0b5/fabric_cf/actor/core/util/id.py
--rw-r--r--   0        0        0     1488 2023-04-03 14:50:53.610758 fabric_cf-1.5.0b5/fabric_cf/actor/core/util/iterable_queue.py
--rw-r--r--   0        0        0     2263 2023-04-03 14:50:53.611043 fabric_cf-1.5.0b5/fabric_cf/actor/core/util/kernel_timer.py
--rw-r--r--   0        0        0     3231 2023-06-08 23:46:35.738141 fabric_cf-1.5.0b5/fabric_cf/actor/core/util/log_helper.py
--rw-r--r--   0        0        0     2238 2023-04-03 14:50:53.611511 fabric_cf-1.5.0b5/fabric_cf/actor/core/util/notice.py
--rw-r--r--   0        0        0     1999 2023-04-03 14:50:53.611700 fabric_cf-1.5.0b5/fabric_cf/actor/core/util/reflection_utils.py
--rw-r--r--   0        0        0     8380 2023-04-03 14:50:53.612072 fabric_cf-1.5.0b5/fabric_cf/actor/core/util/reservation_holdings.py
--rw-r--r--   0        0        0     8864 2023-04-03 14:50:53.612305 fabric_cf-1.5.0b5/fabric_cf/actor/core/util/reservation_list.py
--rw-r--r--   0        0        0     6700 2023-06-06 00:51:32.745023 fabric_cf-1.5.0b5/fabric_cf/actor/core/util/reservation_set.py
--rw-r--r--   0        0        0     3144 2023-04-03 14:50:53.612687 fabric_cf-1.5.0b5/fabric_cf/actor/core/util/reservation_state.py
--rw-r--r--   0        0        0     2250 2023-04-03 14:50:53.612855 fabric_cf-1.5.0b5/fabric_cf/actor/core/util/resource_type.py
--rw-r--r--   0        0        0     1690 2023-04-03 14:50:53.613024 fabric_cf-1.5.0b5/fabric_cf/actor/core/util/rpc_exception.py
--rw-r--r--   0        0        0     4440 2023-04-03 14:50:53.613195 fabric_cf-1.5.0b5/fabric_cf/actor/core/util/update_data.py
--rw-r--r--   0        0        0     4188 2023-04-03 14:50:53.613384 fabric_cf-1.5.0b5/fabric_cf/actor/core/util/utils.py
--rw-r--r--   0        0        0     8424 2023-06-08 16:24:58.599600 fabric_cf-1.5.0b5/fabric_cf/actor/db/__init__.py
--rw-r--r--   0        0        0    63500 2023-06-10 10:25:14.802857 fabric_cf-1.5.0b5/fabric_cf/actor/db/psql_database.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.614689 fabric_cf-1.5.0b5/fabric_cf/actor/fim/__init__.py
--rw-r--r--   0        0        0     6326 2023-05-22 19:03:15.233111 fabric_cf-1.5.0b5/fabric_cf/actor/fim/asm_update_thread.py
--rw-r--r--   0        0        0    28243 2023-05-22 19:03:15.233510 fabric_cf-1.5.0b5/fabric_cf/actor/fim/fim_helper.py
--rw-r--r--   0        0        0        1 2023-04-03 14:50:53.616623 fabric_cf-1.5.0b5/fabric_cf/actor/fim/plugins/__init__.py
--rw-r--r--   0        0        0        1 2023-04-03 14:50:53.616848 fabric_cf-1.5.0b5/fabric_cf/actor/fim/plugins/broker/__init__.py
--rw-r--r--   0        0        0    23911 2023-05-24 00:04:37.573265 fabric_cf-1.5.0b5/fabric_cf/actor/fim/plugins/broker/aggregate_bqm_plugin.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.617325 fabric_cf-1.5.0b5/fabric_cf/actor/handlers/__init__.py
--rw-r--r--   0        0        0     3015 2023-06-08 16:24:58.601458 fabric_cf-1.5.0b5/fabric_cf/actor/handlers/handler_base.py
--rw-r--r--   0        0        0    11187 2023-06-11 12:09:10.465545 fabric_cf-1.5.0b5/fabric_cf/actor/handlers/no_op_handler.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.617898 fabric_cf-1.5.0b5/fabric_cf/actor/security/__init__.py
--rw-r--r--   0        0        0     4918 2023-06-09 00:19:33.906077 fabric_cf-1.5.0b5/fabric_cf/actor/security/access_checker.py
--rw-r--r--   0        0        0     2955 2023-04-03 14:50:53.618313 fabric_cf-1.5.0b5/fabric_cf/actor/security/auth_token.py
--rw-r--r--   0        0        0     3983 2023-05-22 19:03:15.233844 fabric_cf-1.5.0b5/fabric_cf/actor/security/fabric_token.py
--rw-r--r--   0        0        0     8648 2023-06-08 16:24:58.602753 fabric_cf-1.5.0b5/fabric_cf/actor/security/pdp_auth.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.618864 fabric_cf-1.5.0b5/fabric_cf/actor/test/__init__.py
--rw-r--r--   0        0        0    10932 2023-04-04 13:01:29.470229 fabric_cf-1.5.0b5/fabric_cf/actor/test/base_test_case.py
--rw-r--r--   0        0        0     4679 2023-04-03 14:50:53.619270 fabric_cf-1.5.0b5/fabric_cf/actor/test/client_callback_helper.py
--rw-r--r--   0        0        0     4639 2023-06-08 16:24:58.603699 fabric_cf-1.5.0b5/fabric_cf/actor/test/config/config.jenkins.yaml
--rw-r--r--   0        0        0     4305 2023-04-04 15:28:06.631503 fabric_cf-1.5.0b5/fabric_cf/actor/test/config/config.orchestrator.yaml
--rw-r--r--   0        0        0     4696 2023-06-08 16:24:58.604566 fabric_cf-1.5.0b5/fabric_cf/actor/test/config/config.test.yaml
--rw-r--r--   0        0        0     5376 2023-04-03 14:50:53.620212 fabric_cf-1.5.0b5/fabric_cf/actor/test/controller_callback_helper.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.620415 fabric_cf-1.5.0b5/fabric_cf/actor/test/core/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.620599 fabric_cf-1.5.0b5/fabric_cf/actor/test/core/container/__init__.py
--rw-r--r--   0        0        0     2815 2023-04-04 13:02:25.891866 fabric_cf-1.5.0b5/fabric_cf/actor/test/core/container/container_database_test.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.621040 fabric_cf-1.5.0b5/fabric_cf/actor/test/core/core/__init__.py
--rw-r--r--   0        0        0     4091 2023-04-04 13:02:48.136107 fabric_cf-1.5.0b5/fabric_cf/actor/test/core/core/unit_test.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.621493 fabric_cf-1.5.0b5/fabric_cf/actor/test/core/kernel/__init__.py
--rw-r--r--   0        0        0    21480 2023-04-04 15:12:06.450576 fabric_cf-1.5.0b5/fabric_cf/actor/test/core/kernel/kernel_test.py
--rw-r--r--   0        0        0     3378 2023-04-04 15:11:51.860496 fabric_cf-1.5.0b5/fabric_cf/actor/test/core/kernel/tick_test.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.624033 fabric_cf-1.5.0b5/fabric_cf/actor/test/core/plugins/__init__.py
--rw-r--r--   0        0        0     3176 2023-04-04 15:15:43.466105 fabric_cf-1.5.0b5/fabric_cf/actor/test/core/plugins/actor_database_test.py
--rw-r--r--   0        0        0     4729 2023-04-04 17:23:55.100076 fabric_cf-1.5.0b5/fabric_cf/actor/test/core/plugins/ansible_handler_processor_test.py
--rw-r--r--   0        0        0     1963 2023-04-03 14:50:53.624564 fabric_cf-1.5.0b5/fabric_cf/actor/test/core/plugins/authority_substrate_test.py
--rw-r--r--   0        0        0     3263 2023-04-03 14:50:53.624725 fabric_cf-1.5.0b5/fabric_cf/actor/test/core/plugins/substrate_database_test.py
--rw-r--r--   0        0        0     2280 2023-04-04 15:15:47.470348 fabric_cf-1.5.0b5/fabric_cf/actor/test/core/plugins/substrate_test_base.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.625348 fabric_cf-1.5.0b5/fabric_cf/actor/test/core/policy/__init__.py
--rw-r--r--   0        0        0    21995 2023-06-08 16:24:58.605499 fabric_cf-1.5.0b5/fabric_cf/actor/test/core/policy/authoity_calendar_policy_test.py
--rw-r--r--   0        0        0    23678 2023-06-08 16:24:58.606650 fabric_cf-1.5.0b5/fabric_cf/actor/test/core/policy/broker_simpler_units_policy_test.py
--rw-r--r--   0        0        0     4515 2023-06-08 16:24:58.607440 fabric_cf-1.5.0b5/fabric_cf/actor/test/core/policy/controller_simple_policy_test.py
--rw-r--r--   0        0        0     1561 2023-04-03 14:50:53.626668 fabric_cf-1.5.0b5/fabric_cf/actor/test/core/policy/controller_simple_policy_test_wrapper.py
--rw-r--r--   0        0        0     8437 2023-04-03 14:50:53.626899 fabric_cf-1.5.0b5/fabric_cf/actor/test/core/policy/controller_test_wrapper.py
--rw-r--r--   0        0        0     7719 2023-06-08 16:24:58.608430 fabric_cf-1.5.0b5/fabric_cf/actor/test/core/policy/controller_ticket_review_policy_test.py
--rw-r--r--   0        0        0     1586 2023-04-03 14:50:53.627291 fabric_cf-1.5.0b5/fabric_cf/actor/test/core/policy/controller_ticket_review_policy_test_wrapper.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.627471 fabric_cf-1.5.0b5/fabric_cf/actor/test/core/time/__init__.py
--rw-r--r--   0        0        0     3786 2023-04-03 14:50:53.627666 fabric_cf-1.5.0b5/fabric_cf/actor/test/core/time/actor_clock_test.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.627830 fabric_cf-1.5.0b5/fabric_cf/actor/test/core/time/calendar/__init__.py
--rw-r--r--   0        0        0     4290 2023-04-03 14:50:53.628007 fabric_cf-1.5.0b5/fabric_cf/actor/test/core/time/calendar/client_calendar_test.py
--rw-r--r--   0        0        0     2225 2023-04-03 14:50:53.628189 fabric_cf-1.5.0b5/fabric_cf/actor/test/core/time/calendar/controller_calendar_test.py
--rw-r--r--   0        0        0    14887 2023-04-03 14:50:53.628405 fabric_cf-1.5.0b5/fabric_cf/actor/test/core/time/term_test.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.628584 fabric_cf-1.5.0b5/fabric_cf/actor/test/core/util/__init__.py
--rw-r--r--   0        0        0     8041 2023-04-03 14:50:53.628792 fabric_cf-1.5.0b5/fabric_cf/actor/test/core/util/reservation_holdings_test.py
--rw-r--r--   0        0        0     5072 2023-04-03 14:50:53.628930 fabric_cf-1.5.0b5/fabric_cf/actor/test/core/util/reservation_list_test.py
--rw-r--r--   0        0        0     3738 2023-04-03 14:50:53.629079 fabric_cf-1.5.0b5/fabric_cf/actor/test/dummy_authority_proxy.py
--rw-r--r--   0        0        0     1953 2023-04-03 14:50:53.629248 fabric_cf-1.5.0b5/fabric_cf/actor/test/dummy_proxy.py
--rw-r--r--   0        0        0     2498 2023-04-04 16:00:31.265177 fabric_cf-1.5.0b5/fabric_cf/actor/test/fim_test_helper.py
--rw-r--r--   0        0        0       92 2023-04-03 15:02:26.648185 fabric_cf-1.5.0b5/fabric_cf/actor/test/schema/key.avsc
--rw-r--r--   0        0        0    27389 2023-04-03 15:02:26.648701 fabric_cf-1.5.0b5/fabric_cf/actor/test/schema/message.avsc
--rw-r--r--   0        0        0     4532 2023-04-03 15:21:18.938300 fabric_cf-1.5.0b5/fabric_cf/actor/test/test_abqm.py
--rw-r--r--   0        0        0     1892 2023-04-03 14:50:53.630509 fabric_cf-1.5.0b5/fabric_cf/actor/test/test_actor.py
--rw-r--r--   0        0        0     1249 2023-04-03 14:50:53.630745 fabric_cf-1.5.0b5/fabric_cf/actor/test/test_exception.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.630912 fabric_cf-1.5.0b5/fabric_cf/aits/__init__.py
--rw-r--r--   0        0        0     4826 2023-06-08 16:24:58.609228 fabric_cf-1.5.0b5/fabric_cf/aits/config/config.broker.yaml
--rw-r--r--   0        0        0     4808 2023-06-08 16:24:58.610052 fabric_cf-1.5.0b5/fabric_cf/aits/config/config.netam.yaml
--rw-r--r--   0        0        0     4414 2023-06-08 16:24:58.610770 fabric_cf-1.5.0b5/fabric_cf/aits/config/config.orchestrator.yaml
--rw-r--r--   0        0        0     4788 2023-06-08 16:24:58.611552 fabric_cf-1.5.0b5/fabric_cf/aits/config/config.siteam.yaml
--rw-r--r--   0        0        0    49220 2023-06-08 16:24:58.612484 fabric_cf-1.5.0b5/fabric_cf/aits/integration_test.py
--rw-r--r--   0        0        0     7393 2023-06-08 16:24:58.613180 fabric_cf-1.5.0b5/fabric_cf/aits/kafka_processor.py
--rw-r--r--   0        0        0     8633 2023-06-08 16:24:58.613893 fabric_cf-1.5.0b5/fabric_cf/aits/manage_helper.py
--rw-r--r--   0        0        0     8339 2023-06-08 16:24:58.614531 fabric_cf-1.5.0b5/fabric_cf/aits/orchestrator_helper.py
--rw-r--r--   0        0        0    16256 2023-04-03 14:50:53.634161 fabric_cf-1.5.0b5/fabric_cf/authority/Readme.md
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.634241 fabric_cf-1.5.0b5/fabric_cf/authority/__init__.py
--rw-r--r--   0        0        0     2164 2023-04-03 14:50:53.634418 fabric_cf-1.5.0b5/fabric_cf/authority/__main__.py
--rw-r--r--   0        0        0    32973 2023-04-03 14:50:53.634699 fabric_cf-1.5.0b5/fabric_cf/authority/am-yes.xml
--rw-r--r--   0        0        0     5020 2023-06-08 20:13:22.200306 fabric_cf-1.5.0b5/fabric_cf/authority/config.al2s.am.yaml
--rw-r--r--   0        0        0     5114 2023-06-08 20:13:22.209683 fabric_cf-1.5.0b5/fabric_cf/authority/config.net.am.yaml
--rw-r--r--   0        0        0     5485 2023-06-08 20:13:22.194352 fabric_cf-1.5.0b5/fabric_cf/authority/config.site.am.geni.yaml
--rw-r--r--   0        0        0     4979 2023-06-08 20:13:37.444062 fabric_cf-1.5.0b5/fabric_cf/authority/config.site.am.yaml
--rw-r--r--   0        0        0     3427 2023-06-08 16:24:58.617235 fabric_cf-1.5.0b5/fabric_cf/authority/docker-compose.geni.yml
--rw-r--r--   0        0        0     3336 2023-06-08 16:24:58.617973 fabric_cf-1.5.0b5/fabric_cf/authority/docker-compose.yml
--rw-r--r--   0        0        0     1188 2023-06-08 16:24:58.618728 fabric_cf-1.5.0b5/fabric_cf/authority/env.template
--rw-r--r--   0        0        0    16080 2023-04-03 14:50:53.636162 fabric_cf-1.5.0b5/fabric_cf/authority/fabricYes.AnyActorYesPolicy.xml
--rw-r--r--   0        0        0     1588 2023-04-03 14:50:53.636606 fabric_cf-1.5.0b5/fabric_cf/authority/net_handler_config.yml
--rw-r--r--   0        0        0     1523 2023-04-03 14:50:53.636812 fabric_cf-1.5.0b5/fabric_cf/authority/oess_handler_config.yml
--rw-r--r--   0        0        0     1380 2023-04-03 14:50:53.636998 fabric_cf-1.5.0b5/fabric_cf/authority/pdp.xml
--rwxr-xr-x   0        0        0     2446 2023-04-03 14:50:53.637179 fabric_cf-1.5.0b5/fabric_cf/authority/setup.sh
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.637346 fabric_cf-1.5.0b5/fabric_cf/authority/test/__init__.py
--rw-r--r--   0        0        0     2463 2023-04-03 14:50:53.637572 fabric_cf-1.5.0b5/fabric_cf/authority/test/al2s_am.py
--rw-r--r--   0        0        0     2459 2023-04-03 14:50:53.637740 fabric_cf-1.5.0b5/fabric_cf/authority/test/net_am.py
--rw-r--r--   0        0        0     2456 2023-04-03 14:50:53.637876 fabric_cf-1.5.0b5/fabric_cf/authority/test/site_am.py
--rw-r--r--   0        0        0     2461 2023-04-03 14:50:53.638045 fabric_cf-1.5.0b5/fabric_cf/authority/test/site_am_geni.py
--rw-r--r--   0        0        0     4730 2023-06-08 16:24:58.619817 fabric_cf-1.5.0b5/fabric_cf/authority/test/test-al2sam.yaml
--rw-r--r--   0        0        0     4839 2023-06-08 16:24:58.620545 fabric_cf-1.5.0b5/fabric_cf/authority/test/test-netam.yaml
--rw-r--r--   0        0        0     5071 2023-04-03 14:50:53.638536 fabric_cf-1.5.0b5/fabric_cf/authority/test/test.geni.yaml
--rw-r--r--   0        0        0     4685 2023-06-08 16:24:58.621151 fabric_cf-1.5.0b5/fabric_cf/authority/test/test.yaml
--rw-r--r--   0        0        0     2976 2023-06-08 16:31:24.054182 fabric_cf-1.5.0b5/fabric_cf/authority/vm_handler_config.yml
--rw-r--r--   0        0        0     1448 2023-04-03 14:50:53.639031 fabric_cf-1.5.0b5/fabric_cf/authority/vnic_net_handler_config.yml
--rw-r--r--   0        0        0    14262 2023-04-03 14:50:53.639328 fabric_cf-1.5.0b5/fabric_cf/broker/Readme.md
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.639412 fabric_cf-1.5.0b5/fabric_cf/broker/__init__.py
--rw-r--r--   0        0        0     2290 2023-04-03 14:50:53.639603 fabric_cf-1.5.0b5/fabric_cf/broker/__main__.py
--rw-r--r--   0        0        0    27944 2023-04-03 14:50:53.639781 fabric_cf-1.5.0b5/fabric_cf/broker/broker-yes.xml
--rw-r--r--   0        0        0     5118 2023-06-08 20:13:22.204432 fabric_cf-1.5.0b5/fabric_cf/broker/config.broker.yaml
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.640163 fabric_cf-1.5.0b5/fabric_cf/broker/core/__init__.py
--rw-r--r--   0        0        0     3314 2023-04-03 14:50:53.640348 fabric_cf-1.5.0b5/fabric_cf/broker/core/broker_kernel.py
--rw-r--r--   0        0        0     3135 2023-06-08 16:24:58.622513 fabric_cf-1.5.0b5/fabric_cf/broker/docker-compose.yml
--rw-r--r--   0        0        0     1192 2023-06-08 16:24:58.623116 fabric_cf-1.5.0b5/fabric_cf/broker/env.template
--rw-r--r--   0        0        0    16080 2023-04-03 14:50:53.640954 fabric_cf-1.5.0b5/fabric_cf/broker/fabricYes.AnyActorYesPolicy.xml
--rw-r--r--   0        0        0     1380 2023-04-03 14:50:53.641105 fabric_cf-1.5.0b5/fabric_cf/broker/pdp.xml
--rwxr-xr-x   0        0        0     2239 2023-04-03 14:50:53.641257 fabric_cf-1.5.0b5/fabric_cf/broker/setup.sh
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.641487 fabric_cf-1.5.0b5/fabric_cf/broker/test/__init__.py
--rw-r--r--   0        0        0     2507 2023-04-03 14:50:53.641689 fabric_cf-1.5.0b5/fabric_cf/broker/test/broker.py
--rw-r--r--   0        0        0     5042 2023-06-08 16:24:58.623748 fabric_cf-1.5.0b5/fabric_cf/broker/test/test.yaml
--rw-r--r--   0        0        0    20305 2023-05-22 19:03:15.236804 fabric_cf-1.5.0b5/fabric_cf/orchestrator/README.md
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.642384 fabric_cf-1.5.0b5/fabric_cf/orchestrator/__init__.py
--rw-r--r--   0        0        0     3355 2023-05-22 19:03:15.237157 fabric_cf-1.5.0b5/fabric_cf/orchestrator/__main__.py
--rw-r--r--   0        0        0     1757 2023-04-03 14:50:53.642803 fabric_cf-1.5.0b5/fabric_cf/orchestrator/certs/fullchain.pem
--rw-r--r--   0        0        0     3272 2023-04-03 14:50:53.642965 fabric_cf-1.5.0b5/fabric_cf/orchestrator/certs/privkey.pem
--rw-r--r--   0        0        0     4942 2023-06-08 20:12:01.740065 fabric_cf-1.5.0b5/fabric_cf/orchestrator/config.orchestrator.yaml
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.643278 fabric_cf-1.5.0b5/fabric_cf/orchestrator/core/__init__.py
--rw-r--r--   0        0        0     2917 2023-04-03 14:50:53.643501 fabric_cf-1.5.0b5/fabric_cf/orchestrator/core/active_status_checker.py
--rw-r--r--   0        0        0     3050 2023-04-03 14:50:53.643707 fabric_cf-1.5.0b5/fabric_cf/orchestrator/core/bqm_wrapper.py
--rw-r--r--   0        0        0     1556 2023-04-03 14:50:53.643947 fabric_cf-1.5.0b5/fabric_cf/orchestrator/core/exceptions.py
--rw-r--r--   0        0        0     1884 2023-04-03 14:50:53.644155 fabric_cf-1.5.0b5/fabric_cf/orchestrator/core/i_status_update_callback.py
--rw-r--r--   0        0        0    45517 2023-06-11 12:07:05.428270 fabric_cf-1.5.0b5/fabric_cf/orchestrator/core/orchestrator_handler.py
--rw-r--r--   0        0        0     5389 2023-04-03 14:50:53.644692 fabric_cf-1.5.0b5/fabric_cf/orchestrator/core/orchestrator_kernel.py
--rw-r--r--   0        0        0    34864 2023-05-22 18:59:29.517601 fabric_cf-1.5.0b5/fabric_cf/orchestrator/core/orchestrator_slice_wrapper.py
--rw-r--r--   0        0        0     3581 2023-04-03 14:50:53.645306 fabric_cf-1.5.0b5/fabric_cf/orchestrator/core/reservation_converter.py
--rw-r--r--   0        0        0     4880 2023-04-03 14:50:53.645464 fabric_cf-1.5.0b5/fabric_cf/orchestrator/core/reservation_status_update.py
--rw-r--r--   0        0        0     7876 2023-04-03 14:50:53.645708 fabric_cf-1.5.0b5/fabric_cf/orchestrator/core/reservation_status_update_thread.py
--rw-r--r--   0        0        0     7219 2023-06-11 02:28:17.556662 fabric_cf-1.5.0b5/fabric_cf/orchestrator/core/response_builder.py
--rw-r--r--   0        0        0     8722 2023-06-08 16:24:58.626362 fabric_cf-1.5.0b5/fabric_cf/orchestrator/core/slice_defer_thread.py
--rw-r--r--   0        0        0     1972 2023-04-03 14:50:53.646372 fabric_cf-1.5.0b5/fabric_cf/orchestrator/core/status_checker.py
--rw-r--r--   0        0        0     1581 2023-04-03 14:50:53.646556 fabric_cf-1.5.0b5/fabric_cf/orchestrator/core/watch_entry.py
--rw-r--r--   0        0        0     3501 2023-06-08 16:24:58.627013 fabric_cf-1.5.0b5/fabric_cf/orchestrator/docker-compose.yml
--rw-r--r--   0        0        0     1198 2023-06-08 16:24:58.627686 fabric_cf-1.5.0b5/fabric_cf/orchestrator/env.template
--rw-r--r--   0        0        0    72323 2023-04-03 14:50:53.647218 fabric_cf-1.5.0b5/fabric_cf/orchestrator/fabricTags.OrchestratorTags.xml
--rw-r--r--   0        0        0     1626 2023-04-03 14:50:53.647500 fabric_cf-1.5.0b5/fabric_cf/orchestrator/nginx/default.conf
--rw-r--r--   0        0        0    60103 2023-06-11 02:24:34.870624 fabric_cf-1.5.0b5/fabric_cf/orchestrator/openapi.json
--rw-r--r--   0        0        0    30829 2023-04-03 14:50:53.648266 fabric_cf-1.5.0b5/fabric_cf/orchestrator/orchestrator-yes.xml
--rw-r--r--   0        0        0     1548 2023-04-03 14:50:53.648514 fabric_cf-1.5.0b5/fabric_cf/orchestrator/pdp.xml
--rwxr-xr-x   0        0        0     2284 2023-04-03 14:50:53.648696 fabric_cf-1.5.0b5/fabric_cf/orchestrator/setup.sh
--rw-r--r--   0        0        0      430 2023-06-11 02:30:01.477191 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/__init__.py
--rw-r--r--   0        0        0      392 2023-06-11 02:30:01.479801 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/__main__.py
--rw-r--r--   0        0        0        0 2023-06-11 02:30:01.464454 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/controllers/__init__.py
--rw-r--r--   0        0        0      311 2023-06-11 02:30:19.930901 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/controllers/authorization_controller.py
--rw-r--r--   0        0        0     1927 2023-06-11 02:30:25.254003 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/controllers/poas_controller.py
--rw-r--r--   0        0        0     1249 2023-06-11 02:30:30.641124 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/controllers/resources_controller.py
--rw-r--r--   0        0        0     6147 2023-06-11 02:30:38.939352 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/controllers/slices_controller.py
--rw-r--r--   0        0        0     1094 2023-06-11 02:30:44.749719 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/controllers/slivers_controller.py
--rw-r--r--   0        0        0      305 2023-06-11 02:30:49.257651 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/controllers/version_controller.py
--rw-r--r--   0        0        0      631 2023-06-11 02:30:01.463631 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/encoder.py
--rw-r--r--   0        0        0     2757 2023-06-11 02:30:01.458703 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/__init__.py
--rw-r--r--   0        0        0     1889 2023-06-11 02:30:01.460369 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/base_model_.py
--rw-r--r--   0        0        0     3400 2023-06-11 02:30:01.457640 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/poa.py
--rw-r--r--   0        0        0     5315 2023-06-11 02:30:01.462695 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/poa_data.py
--rw-r--r--   0        0        0     2624 2023-06-11 02:30:01.456650 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/poa_post.py
--rw-r--r--   0        0        0     2712 2023-06-11 02:30:01.459068 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/poa_post_data.py
--rw-r--r--   0        0        0     2254 2023-06-11 02:30:01.463293 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/poa_post_data_vcpu_cpu_map.py
--rw-r--r--   0        0        0     1628 2023-06-11 02:30:01.458513 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/resource.py
--rw-r--r--   0        0        0     3564 2023-06-11 02:30:01.460675 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/resources.py
--rw-r--r--   0        0        0     7311 2023-06-11 02:30:01.457428 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/slice.py
--rw-r--r--   0        0        0     3616 2023-06-11 02:30:01.456334 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/slice_details.py
--rw-r--r--   0        0        0     5251 2023-06-11 02:30:01.461701 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/slices.py
--rw-r--r--   0        0        0     2634 2023-06-11 02:30:01.460524 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/slices_post.py
--rw-r--r--   0        0        0     8995 2023-06-11 02:30:01.462864 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/sliver.py
--rw-r--r--   0        0        0     5301 2023-06-11 02:30:01.461341 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/slivers.py
--rw-r--r--   0        0        0     3896 2023-06-11 02:30:01.461866 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/status200_ok_no_content.py
--rw-r--r--   0        0        0     2464 2023-06-11 02:30:01.457862 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/status200_ok_no_content_data.py
--rw-r--r--   0        0        0     4929 2023-06-11 02:30:01.460159 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/status200_ok_paginated.py
--rw-r--r--   0        0        0     2870 2023-06-11 02:30:01.459399 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/status200_ok_single.py
--rw-r--r--   0        0        0     1983 2023-06-11 02:30:01.459895 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/status400_bad_request.py
--rw-r--r--   0        0        0     4503 2023-06-11 02:30:01.462170 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/status400_bad_request_errors.py
--rw-r--r--   0        0        0     3984 2023-06-11 02:30:01.461209 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/status401_unauthorized.py
--rw-r--r--   0        0        0     2512 2023-06-11 02:30:01.456495 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/status401_unauthorized_errors.py
--rw-r--r--   0        0        0     3879 2023-06-11 02:30:01.460908 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/status403_forbidden.py
--rw-r--r--   0        0        0     2461 2023-06-11 02:30:01.458293 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/status403_forbidden_errors.py
--rw-r--r--   0        0        0     3846 2023-06-11 02:30:01.459604 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/status404_not_found.py
--rw-r--r--   0        0        0     2446 2023-06-11 02:30:01.462425 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/status404_not_found_errors.py
--rw-r--r--   0        0        0     4233 2023-06-11 02:30:01.458110 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/status500_internal_server_error.py
--rw-r--r--   0        0        0     2635 2023-06-11 02:30:01.456913 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/status500_internal_server_error_errors.py
--rw-r--r--   0        0        0     3540 2023-06-11 02:30:01.457231 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/version.py
--rw-r--r--   0        0        0     2536 2023-06-11 02:30:01.457071 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/version_data.py
--rw-r--r--   0        0        0        0 2023-06-11 02:30:01.469802 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/response/__init__.py
--rw-r--r--   0        0        0     1355 2023-06-11 02:30:01.474051 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/response/authorization_controller.py
--rw-r--r--   0        0        0     1997 2023-06-11 02:30:01.469671 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/response/constants.py
--rw-r--r--   0        0        0     5537 2023-06-11 02:30:01.469404 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/response/cors_response.py
--rw-r--r--   0        0        0     5428 2023-06-11 02:30:01.473655 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/response/poas_controller.py
--rw-r--r--   0        0        0     4321 2023-06-11 02:30:01.474504 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/response/resources_controller.py
--rw-r--r--   0        0        0    15437 2023-06-11 02:30:01.473280 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/response/slices_controller.py
--rw-r--r--   0        0        0     4642 2023-06-11 02:30:01.473814 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/response/slivers_controller.py
--rw-r--r--   0        0        0     2530 2023-06-11 02:30:01.472872 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/response/utils.py
--rw-r--r--   0        0        0     2632 2023-06-11 02:30:01.474262 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/response/version_controller.py
--rw-r--r--   0        0        0    43331 2023-06-11 02:30:01.455579 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/swagger/swagger.yaml
--rw-r--r--   0        0        0      438 2023-06-11 02:30:01.454657 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/test/__init__.py
--rw-r--r--   0        0        0     2531 2023-06-11 02:30:01.454942 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/test/test_poas_controller.py
--rw-r--r--   0        0        0     2094 2023-06-11 02:30:01.454312 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/test/test_resources_controller.py
--rw-r--r--   0        0        0     5271 2023-06-11 02:30:01.453987 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/test/test_slices_controller.py
--rw-r--r--   0        0        0     1989 2023-06-11 02:30:01.453756 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/test/test_slivers_controller.py
--rw-r--r--   0        0        0      855 2023-06-11 02:30:01.454164 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/test/test_version_controller.py
--rw-r--r--   0        0        0      809 2023-06-11 02:30:01.463946 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/type_util.py
--rw-r--r--   0        0        0     3452 2023-06-11 02:30:01.455776 fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/util.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.659106 fabric_cf-1.5.0b5/fabric_cf/orchestrator/test/__init__.py
--rw-r--r--   0        0        0     3542 2023-04-03 14:50:53.659281 fabric_cf-1.5.0b5/fabric_cf/orchestrator/test/orchestrator.py
--rwxr-xr-x   0        0        0       78 2023-04-03 14:50:53.659409 fabric_cf-1.5.0b5/fabric_cf/orchestrator/test/test.sh
--rw-r--r--   0        0        0     4453 2023-06-08 16:24:58.640149 fabric_cf-1.5.0b5/fabric_cf/orchestrator/test/test.yaml
--rwxr-xr-x   0        0        0     2900 2023-04-03 14:50:53.659782 fabric_cf-1.5.0b5/fabric_cf/orchestrator/update_swagger_stub.sh
--rw-r--r--   0        0        0    18177 2023-04-03 14:50:53.660187 fabric_cf-1.5.0b5/images/am-pod.png
--rw-r--r--   0        0        0    74927 2023-04-03 14:50:53.660890 fabric_cf-1.5.0b5/images/am.png
--rw-r--r--   0        0        0    18471 2023-04-03 14:50:53.661225 fabric_cf-1.5.0b5/images/broker-pod.png
--rw-r--r--   0        0        0    73799 2023-04-03 14:50:53.661878 fabric_cf-1.5.0b5/images/broker.png
--rw-r--r--   0        0        0    90831 2023-04-03 14:50:53.662835 fabric_cf-1.5.0b5/images/cf.png
--rw-r--r--   0        0        0    19611 2023-04-03 14:50:53.663247 fabric_cf-1.5.0b5/images/orchestrator-pod.png
--rw-r--r--   0        0        0    78622 2023-04-03 14:50:53.664084 fabric_cf-1.5.0b5/images/orchestrator.png
--rw-r--r--   0        0        0   145542 2023-04-03 14:50:53.664854 fabric_cf-1.5.0b5/neo4j/AL2S.graphml
--rw-r--r--   0        0        0    96363 2023-04-03 14:50:53.665732 fabric_cf-1.5.0b5/neo4j/LBNL-ad.graphml
--rw-r--r--   0        0        0    68182 2023-04-03 14:50:53.666334 fabric_cf-1.5.0b5/neo4j/Network-ad.graphml
--rw-r--r--   0        0        0   108181 2023-06-11 20:42:11.223136 fabric_cf-1.5.0b5/neo4j/RENCI-ad.graphml
--rw-r--r--   0        0        0    96286 2023-04-03 14:50:53.667143 fabric_cf-1.5.0b5/neo4j/UKY-ad.graphml
--rw-r--r--   0        0        0  1297955 2023-04-03 14:50:53.672629 fabric_cf-1.5.0b5/neo4j/UKY2.graphml
--rw-r--r--   0        0        0    14808 2023-04-03 14:50:53.673167 fabric_cf-1.5.0b5/neo4j/abqm.graphml
--rw-r--r--   0        0        0     1757 2023-04-03 14:50:53.673435 fabric_cf-1.5.0b5/neo4j/certs/fullchain.pem
--rw-r--r--   0        0        0     3272 2023-04-03 14:50:53.673617 fabric_cf-1.5.0b5/neo4j/certs/privkey.pem
--rwxr-xr-x   0        0        0       91 2023-04-03 14:50:53.673785 fabric_cf-1.5.0b5/orchestrator.sh
--rw-r--r--   0        0        0      698 2023-04-03 14:50:53.673962 fabric_cf-1.5.0b5/psql.upgrade
--rw-r--r--   0        0        0     1251 2023-06-11 23:52:23.364027 fabric_cf-1.5.0b5/pyproject.toml
--rwxr-xr-x   0        0        0     2594 2023-06-08 16:24:58.641210 fabric_cf-1.5.0b5/secrets/create-certs.sh
--rw-r--r--   0        0        0    12796 2023-05-22 19:03:15.242478 fabric_cf-1.5.0b5/tools/audit.py
--rw-r--r--   0        0        0     8005 2023-04-03 14:50:53.675250 fabric_cf-1.5.0b5/tools/db_cli.py
--rw-r--r--   0        0        0      354 2023-05-22 19:03:15.243289 fabric_cf-1.5.0b5/tools/install.sh
--rw-r--r--   0        0        0      143 2023-04-03 14:50:53.675627 fabric_cf-1.5.0b5/tox.ini
--rw-r--r--   0        0        0     3315 1970-01-01 00:00:00.000000 fabric_cf-1.5.0b5/PKG-INFO
+-rw-r--r--   0        0        0     2035 2023-06-17 01:45:40.863412 fabric_cf-1.5.1rc0/.gitignore
+-rw-r--r--   0        0        0      849 2023-06-17 01:48:45.788958 fabric_cf-1.5.1rc0/Dockerfile-auth
+-rw-r--r--   0        0        0      769 2023-06-17 01:45:40.863751 fabric_cf-1.5.1rc0/Dockerfile-broker
+-rw-r--r--   0        0        0     1037 2023-06-17 01:45:40.863865 fabric_cf-1.5.1rc0/Dockerfile-cf
+-rw-r--r--   0        0        0      787 2023-06-17 01:45:40.864056 fabric_cf-1.5.1rc0/Dockerfile-orchestrator
+-rw-r--r--   0        0        0     1071 2023-06-17 01:45:40.864264 fabric_cf-1.5.1rc0/LICENSE
+-rw-r--r--   0        0        0     2046 2023-06-17 01:45:40.864609 fabric_cf-1.5.1rc0/README.md
+-rwxr-xr-x   0        0        0       74 2023-06-17 01:45:40.864811 fabric_cf-1.5.1rc0/authority.sh
+-rwxr-xr-x   0        0        0       79 2023-06-17 01:45:40.865118 fabric_cf-1.5.1rc0/broker.sh
+-rw-r--r--   0        0        0      947 2023-06-17 01:45:40.865265 fabric_cf-1.5.1rc0/cleanup_old_schema_from_schema_registry.sh
+-rw-r--r--   0        0        0     2861 2023-06-17 01:45:40.865477 fabric_cf-1.5.1rc0/docker-compose-kafka.yaml
+-rw-r--r--   0        0        0     1560 2023-06-17 01:45:40.865633 fabric_cf-1.5.1rc0/docker-compose-no-ssl-kafka.yaml
+-rw-r--r--   0        0        0    10307 2023-06-17 01:45:40.865796 fabric_cf-1.5.1rc0/docker-compose-test.yaml
+-rwxr-xr-x   0        0        0       45 2023-06-17 01:45:40.865908 fabric_cf-1.5.1rc0/docker-entrypoint.sh
+-rw-r--r--   0        0        0      350 2023-06-17 01:45:40.866057 fabric_cf-1.5.1rc0/env.template
+-rw-r--r--   0        0        0     1135 2023-06-17 01:45:40.866253 fabric_cf-1.5.1rc0/env.template.test
+-rw-r--r--   0        0        0    16609 2023-06-17 01:45:40.866486 fabric_cf-1.5.1rc0/fabricNo.AnyActorNoPolicy.xml
+-rw-r--r--   0        0        0     6343 2023-06-17 01:45:40.866737 fabric_cf-1.5.1rc0/fabric_cf/Design.md
+-rw-r--r--   0        0        0       51 2023-06-17 02:03:48.742043 fabric_cf-1.5.1rc0/fabric_cf/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.866935 fabric_cf-1.5.1rc0/fabric_cf/actor/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.867028 fabric_cf-1.5.1rc0/fabric_cf/actor/boot/__init__.py
+-rw-r--r--   0        0        0    15281 2023-06-17 01:45:40.867198 fabric_cf-1.5.1rc0/fabric_cf/actor/boot/configuration.py
+-rw-r--r--   0        0        0     1268 2023-06-17 01:45:40.867402 fabric_cf-1.5.1rc0/fabric_cf/actor/boot/configuration_exception.py
+-rw-r--r--   0        0        0     2509 2023-06-17 01:45:40.867741 fabric_cf-1.5.1rc0/fabric_cf/actor/boot/configuration_loader.py
+-rw-r--r--   0        0        0    23003 2023-06-17 01:45:40.868096 fabric_cf-1.5.1rc0/fabric_cf/actor/boot/configuration_processor.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.868344 fabric_cf-1.5.1rc0/fabric_cf/actor/boot/inventory/__init__.py
+-rw-r--r--   0        0        0     4969 2023-06-17 01:45:40.868546 fabric_cf-1.5.1rc0/fabric_cf/actor/boot/inventory/aggregate_resource_model_creator.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.868656 fabric_cf-1.5.1rc0/fabric_cf/actor/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.868776 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/__init__.py
+-rw-r--r--   0        0        0     4907 2023-06-17 01:45:40.868918 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_actor_container.py
+-rw-r--r--   0        0        0     1530 2023-06-17 01:45:40.869075 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_actor_event.py
+-rw-r--r--   0        0        0     2176 2023-06-17 01:45:40.869326 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_actor_identity.py
+-rw-r--r--   0        0        0    10694 2023-06-17 01:45:40.869680 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_actor_management_object.py
+-rw-r--r--   0        0        0    21823 2023-06-17 01:45:40.869978 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_actor_mixin.py
+-rw-r--r--   0        0        0     1918 2023-06-17 01:45:40.870436 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_actor_proxy.py
+-rw-r--r--   0        0        0     1323 2023-06-17 01:45:40.870759 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_actor_runnable.py
+-rw-r--r--   0        0        0     4745 2023-06-17 01:45:40.870983 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_authority.py
+-rw-r--r--   0        0        0     8736 2023-06-17 01:45:40.871245 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_authority_policy.py
+-rw-r--r--   0        0        0     3657 2023-06-17 01:45:40.871530 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_authority_proxy.py
+-rw-r--r--   0        0        0     3367 2023-06-17 01:45:40.872840 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_authority_reservation.py
+-rw-r--r--   0        0        0     6071 2023-06-17 01:45:40.873202 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_base_plugin.py
+-rw-r--r--   0        0        0     2290 2023-06-17 01:45:40.873473 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_broker_mixin.py
+-rw-r--r--   0        0        0     1492 2023-06-17 01:45:40.873734 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_broker_policy_mixin.py
+-rw-r--r--   0        0        0     3690 2023-06-17 01:45:40.873956 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_broker_proxy.py
+-rw-r--r--   0        0        0     4012 2023-06-17 01:45:40.874219 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_broker_reservation.py
+-rw-r--r--   0        0        0     2442 2023-06-17 01:45:40.874471 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_callback_proxy.py
+-rw-r--r--   0        0        0     9846 2023-06-17 01:45:40.874749 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_client_actor.py
+-rw-r--r--   0        0        0     6811 2023-06-17 01:45:40.875221 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_client_actor_management_object.py
+-rw-r--r--   0        0        0     2640 2023-06-17 01:45:40.875500 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_client_callback_proxy.py
+-rw-r--r--   0        0        0     5802 2023-06-17 01:45:40.875807 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_client_policy.py
+-rw-r--r--   0        0        0     7724 2023-06-17 01:45:40.876153 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_client_reservation.py
+-rw-r--r--   0        0        0     1936 2023-06-17 01:45:40.876471 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_component.py
+-rw-r--r--   0        0        0    10115 2023-06-17 01:45:40.876704 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_concrete_set.py
+-rw-r--r--   0        0        0     2729 2023-06-17 01:45:40.877257 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_container_clock.py
+-rw-r--r--   0        0        0     3976 2023-06-17 01:45:40.877655 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_container_database.py
+-rw-r--r--   0        0        0     3367 2023-06-17 01:45:40.878017 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_controller.py
+-rw-r--r--   0        0        0     2855 2023-06-17 01:45:40.878409 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_controller_callback_proxy.py
+-rw-r--r--   0        0        0     2787 2023-06-17 01:45:40.878639 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_controller_policy.py
+-rw-r--r--   0        0        0     5713 2023-06-17 01:45:40.878840 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_controller_reservation.py
+-rw-r--r--   0        0        0    11714 2023-06-17 01:45:40.879061 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_database.py
+-rw-r--r--   0        0        0    11127 2023-06-17 01:45:40.879498 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_delegation.py
+-rw-r--r--   0        0        0     1867 2023-06-17 01:45:40.879821 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_event.py
+-rw-r--r--   0        0        0     1943 2023-06-17 01:45:40.880478 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_management_object.py
+-rw-r--r--   0        0        0     9824 2023-06-17 01:45:40.880799 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_mgmt_actor.py
+-rw-r--r--   0        0        0     2534 2023-06-17 01:45:40.881069 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_mgmt_authority.py
+-rw-r--r--   0        0        0     1452 2023-06-17 01:45:40.881307 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_mgmt_broker_mixin.py
+-rw-r--r--   0        0        0     6191 2023-06-17 01:45:40.881515 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_mgmt_client_actor.py
+-rw-r--r--   0        0        0     5041 2023-06-17 01:45:40.881698 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_mgmt_container.py
+-rw-r--r--   0        0        0     2486 2023-06-17 01:45:40.881920 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_mgmt_controller_mixin.py
+-rw-r--r--   0        0        0     5014 2023-06-17 01:45:40.882105 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_mgmt_server_actor.py
+-rw-r--r--   0        0        0    11147 2023-06-17 01:45:40.882278 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_policy.py
+-rw-r--r--   0        0        0     2304 2023-06-17 01:45:40.882460 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_proxy.py
+-rw-r--r--   0        0        0     2290 2023-06-17 01:45:40.883011 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_proxy_factory.py
+-rw-r--r--   0        0        0     1658 2023-06-17 01:45:40.883589 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_query_response_handler.py
+-rw-r--r--   0        0        0    14613 2023-06-17 01:45:40.883981 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_reservation_mixin.py
+-rw-r--r--   0        0        0     9388 2023-06-17 01:45:40.884267 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_reservation_resources.py
+-rw-r--r--   0        0        0     5581 2023-06-17 01:45:40.884494 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_reservation_status.py
+-rw-r--r--   0        0        0     8963 2023-06-17 01:45:40.884761 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_resource_control.py
+-rw-r--r--   0        0        0     1336 2023-06-17 01:45:40.885119 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_response_handler.py
+-rw-r--r--   0        0        0     2246 2023-06-17 01:45:40.885404 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_rpc_request_state.py
+-rw-r--r--   0        0        0     5634 2023-06-17 01:45:40.885793 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_server_actor.py
+-rw-r--r--   0        0        0     6415 2023-06-17 01:45:40.886064 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_server_policy.py
+-rw-r--r--   0        0        0     4846 2023-06-17 01:45:40.886279 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_server_reservation.py
+-rw-r--r--   0        0        0    13280 2023-06-17 01:45:40.886495 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_slice.py
+-rw-r--r--   0        0        0     3548 2023-06-17 01:45:40.886734 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_substrate.py
+-rw-r--r--   0        0        0     2225 2023-06-17 01:45:40.886964 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_substrate_database.py
+-rw-r--r--   0        0        0     2943 2023-06-17 01:45:40.887211 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_tick.py
+-rw-r--r--   0        0        0     6121 2023-06-17 01:45:40.887540 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_ticker.py
+-rw-r--r--   0        0        0     1590 2023-06-17 01:45:40.887740 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_timer_queue.py
+-rw-r--r--   0        0        0     1387 2023-06-17 01:45:40.887994 fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_timer_task.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.888217 fabric_cf-1.5.1rc0/fabric_cf/actor/core/common/__init__.py
+-rw-r--r--   0        0        0    13142 2023-06-17 01:45:40.888673 fabric_cf-1.5.1rc0/fabric_cf/actor/core/common/constants.py
+-rw-r--r--   0        0        0     4877 2023-06-17 01:46:19.228595 fabric_cf-1.5.1rc0/fabric_cf/actor/core/common/event_logger.py
+-rw-r--r--   0        0        0     5517 2023-06-17 01:45:40.889343 fabric_cf-1.5.1rc0/fabric_cf/actor/core/common/exceptions.py
+-rw-r--r--   0        0        0     6108 2023-06-17 01:45:40.889607 fabric_cf-1.5.1rc0/fabric_cf/actor/core/common/resource_config.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.889797 fabric_cf-1.5.1rc0/fabric_cf/actor/core/container/__init__.py
+-rw-r--r--   0        0        0    24564 2023-06-17 01:45:40.890212 fabric_cf-1.5.1rc0/fabric_cf/actor/core/container/container.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.890449 fabric_cf-1.5.1rc0/fabric_cf/actor/core/container/db/__init__.py
+-rw-r--r--   0        0        0     8667 2023-06-17 01:45:40.890888 fabric_cf-1.5.1rc0/fabric_cf/actor/core/container/db/container_database.py
+-rw-r--r--   0        0        0    19408 2023-06-17 01:45:40.891134 fabric_cf-1.5.1rc0/fabric_cf/actor/core/container/globals.py
+-rw-r--r--   0        0        0     9216 2023-06-17 01:45:40.891411 fabric_cf-1.5.1rc0/fabric_cf/actor/core/container/maintenance.py
+-rw-r--r--   0        0        0     5472 2023-06-17 01:45:40.891732 fabric_cf-1.5.1rc0/fabric_cf/actor/core/container/message_service.py
+-rw-r--r--   0        0        0     1508 2023-06-17 01:45:40.891975 fabric_cf-1.5.1rc0/fabric_cf/actor/core/container/protocol_descriptor.py
+-rw-r--r--   0        0        0    13005 2023-06-17 01:45:40.892261 fabric_cf-1.5.1rc0/fabric_cf/actor/core/container/remote_actor_cache.py
+-rw-r--r--   0        0        0     8040 2023-06-17 01:45:40.892492 fabric_cf-1.5.1rc0/fabric_cf/actor/core/container/rpc_producer.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.892673 fabric_cf-1.5.1rc0/fabric_cf/actor/core/core/__init__.py
+-rw-r--r--   0        0        0    35787 2023-06-17 01:45:40.893317 fabric_cf-1.5.1rc0/fabric_cf/actor/core/core/actor.py
+-rw-r--r--   0        0        0     1975 2023-06-17 01:45:40.893769 fabric_cf-1.5.1rc0/fabric_cf/actor/core/core/actor_identity.py
+-rw-r--r--   0        0        0    15513 2023-06-17 01:45:40.894080 fabric_cf-1.5.1rc0/fabric_cf/actor/core/core/authority.py
+-rw-r--r--   0        0        0     4845 2023-06-17 01:45:40.894403 fabric_cf-1.5.1rc0/fabric_cf/actor/core/core/authority_policy.py
+-rw-r--r--   0        0        0    20447 2023-06-17 01:45:40.894765 fabric_cf-1.5.1rc0/fabric_cf/actor/core/core/broker.py
+-rw-r--r--   0        0        0     5914 2023-06-17 01:45:40.895329 fabric_cf-1.5.1rc0/fabric_cf/actor/core/core/broker_policy.py
+-rw-r--r--   0        0        0    20420 2023-06-17 01:45:40.895550 fabric_cf-1.5.1rc0/fabric_cf/actor/core/core/controller.py
+-rw-r--r--   0        0        0     8604 2023-06-17 01:45:40.895789 fabric_cf-1.5.1rc0/fabric_cf/actor/core/core/event_processor.py
+-rw-r--r--   0        0        0     5467 2023-06-17 01:45:40.900418 fabric_cf-1.5.1rc0/fabric_cf/actor/core/core/inventory_slice_manager.py
+-rw-r--r--   0        0        0     6171 2023-06-17 01:45:40.900826 fabric_cf-1.5.1rc0/fabric_cf/actor/core/core/policy.py
+-rw-r--r--   0        0        0     2042 2023-06-17 01:45:40.901080 fabric_cf-1.5.1rc0/fabric_cf/actor/core/core/rpc_request_state.py
+-rw-r--r--   0        0        0     8688 2023-06-17 01:45:40.901396 fabric_cf-1.5.1rc0/fabric_cf/actor/core/core/ticket.py
+-rw-r--r--   0        0        0    16572 2023-06-17 01:45:40.902085 fabric_cf-1.5.1rc0/fabric_cf/actor/core/core/unit.py
+-rw-r--r--   0        0        0    13814 2023-06-17 01:45:40.902521 fabric_cf-1.5.1rc0/fabric_cf/actor/core/core/unit_set.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.902808 fabric_cf-1.5.1rc0/fabric_cf/actor/core/delegation/__init__.py
+-rw-r--r--   0        0        0    11038 2023-06-17 01:45:40.903490 fabric_cf-1.5.1rc0/fabric_cf/actor/core/delegation/broker_delegation.py
+-rw-r--r--   0        0        0     1933 2023-06-17 01:45:40.903790 fabric_cf-1.5.1rc0/fabric_cf/actor/core/delegation/broker_delegation_factory.py
+-rw-r--r--   0        0        0    17061 2023-06-17 01:45:40.904110 fabric_cf-1.5.1rc0/fabric_cf/actor/core/delegation/delegation.py
+-rw-r--r--   0        0        0     1916 2023-06-17 01:45:40.904369 fabric_cf-1.5.1rc0/fabric_cf/actor/core/delegation/delegation_factory.py
+-rw-r--r--   0        0        0     5364 2023-06-17 01:45:40.904697 fabric_cf-1.5.1rc0/fabric_cf/actor/core/delegation/resource_ticket.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.904962 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/__init__.py
+-rw-r--r--   0        0        0    31973 2023-06-17 01:45:40.905269 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/authority_reservation.py
+-rw-r--r--   0        0        0     3384 2023-06-17 01:45:40.905811 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/broker_query_model_publisher.py
+-rw-r--r--   0        0        0    26805 2023-06-17 01:45:40.906235 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/broker_reservation.py
+-rw-r--r--   0        0        0     2992 2023-06-17 01:45:40.906560 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/claim_timeout.py
+-rw-r--r--   0        0        0     4396 2023-06-17 01:45:40.907195 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/failed_rpc.py
+-rw-r--r--   0        0        0     3639 2023-06-17 01:45:40.907601 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/failed_rpc_event.py
+-rw-r--r--   0        0        0     2668 2023-06-17 01:45:40.907875 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/incoming_delegation_rpc.py
+-rw-r--r--   0        0        0     2708 2023-06-17 01:45:40.908814 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/incoming_failed_rpc.py
+-rw-r--r--   0        0        0     2274 2023-06-17 01:45:40.909146 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/incoming_poa_rpc.py
+-rw-r--r--   0        0        0     2105 2023-06-17 01:45:40.909676 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/incoming_query_rpc.py
+-rw-r--r--   0        0        0     2703 2023-06-17 01:45:40.909938 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/incoming_reservation_rpc.py
+-rw-r--r--   0        0        0     4158 2023-06-17 01:45:40.910172 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/incoming_rpc.py
+-rw-r--r--   0        0        0    11227 2023-06-17 01:45:40.910406 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/incoming_rpc_event.py
+-rw-r--r--   0        0        0    65705 2023-06-17 01:45:40.910921 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/kernel.py
+-rw-r--r--   0        0        0     3314 2023-06-17 01:45:40.911164 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/kernel_tick.py
+-rw-r--r--   0        0        0    57828 2023-06-17 01:45:40.911601 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/kernel_wrapper.py
+-rw-r--r--   0        0        0    12824 2023-06-17 01:45:40.911960 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/poa.py
+-rw-r--r--   0        0        0     2363 2023-06-17 01:45:40.912248 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/predecessor_state.py
+-rw-r--r--   0        0        0     2860 2023-06-17 01:45:40.912445 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/query_timeout.py
+-rw-r--r--   0        0        0     1404 2023-06-17 01:45:40.912669 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/request_types.py
+-rw-r--r--   0        0        0    24674 2023-06-17 01:45:40.912980 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/reservation.py
+-rw-r--r--   0        0        0    92717 2023-06-17 01:45:40.913551 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/reservation_client.py
+-rw-r--r--   0        0        0     9994 2023-06-17 01:45:40.913821 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/reservation_server.py
+-rw-r--r--   0        0        0     3311 2023-06-17 01:45:40.914385 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/reservation_states.py
+-rw-r--r--   0        0        0    21131 2023-06-17 01:45:40.914668 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/resource_set.py
+-rw-r--r--   0        0        0     1614 2023-06-17 01:45:40.914912 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/retry_rpc.py
+-rw-r--r--   0        0        0     1899 2023-06-17 01:45:40.915177 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/retry_rpc_event.py
+-rw-r--r--   0        0        0     4128 2023-06-17 01:45:40.915550 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/rpc_executor.py
+-rw-r--r--   0        0        0    32934 2023-06-17 01:45:40.915918 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/rpc_manager.py
+-rw-r--r--   0        0        0     1772 2023-06-17 01:45:40.916193 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/rpc_manager_singleton.py
+-rw-r--r--   0        0        0     3793 2023-06-17 01:45:40.916409 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/rpc_request.py
+-rw-r--r--   0        0        0     1650 2023-06-17 01:45:40.916665 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/rpc_request_type.py
+-rw-r--r--   0        0        0     1340 2023-06-17 01:45:40.916871 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/sequence_comparison_codes.py
+-rw-r--r--   0        0        0    12284 2023-06-17 01:45:40.917135 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/slice.py
+-rw-r--r--   0        0        0    12785 2023-06-17 01:45:40.917554 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/slice_state_machine.py
+-rw-r--r--   0        0        0     8319 2023-06-17 01:45:40.917865 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/slice_table.py
+-rw-r--r--   0        0        0     6527 2023-06-17 01:45:40.918021 fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/tick.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.918260 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/__init__.py
+-rw-r--r--   0        0        0    39627 2023-06-17 01:45:40.918580 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/actor_management_object.py
+-rw-r--r--   0        0        0     8431 2023-06-17 01:45:40.919181 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/authority_management_object.py
+-rw-r--r--   0        0        0     7315 2023-06-17 01:45:40.919477 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/broker_management_object.py
+-rw-r--r--   0        0        0    29438 2023-06-17 01:45:40.919948 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/client_actor_management_object_helper.py
+-rw-r--r--   0        0        0     9605 2023-06-17 01:45:40.920652 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/container_management_object.py
+-rw-r--r--   0        0        0     9165 2023-06-17 01:45:40.920962 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/controller_management_object.py
+-rw-r--r--   0        0        0    13007 2023-06-17 01:45:40.921229 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/converter.py
+-rw-r--r--   0        0        0     1624 2023-06-17 01:45:40.921530 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/error.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.921728 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/kafka/__init__.py
+-rw-r--r--   0        0        0    10535 2023-06-17 01:45:40.921949 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/kafka/kafka_actor.py
+-rw-r--r--   0        0        0     3509 2023-06-17 01:45:40.922172 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/kafka/kafka_authority.py
+-rw-r--r--   0        0        0     8200 2023-06-17 01:45:40.922389 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/kafka/kafka_broker.py
+-rw-r--r--   0        0        0     4483 2023-06-17 01:45:40.922670 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/kafka/kafka_container.py
+-rw-r--r--   0        0        0     5462 2023-06-17 01:45:40.922906 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/kafka/kafka_controller.py
+-rw-r--r--   0        0        0     5462 2023-06-17 01:45:40.923164 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/kafka/kafka_mgmt_message_processor.py
+-rw-r--r--   0        0        0     6960 2023-06-17 01:45:40.923443 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/kafka/kafka_proxy.py
+-rw-r--r--   0        0        0     5730 2023-06-17 01:45:40.923744 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/kafka/kafka_server_actor.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.923936 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/kafka/services/__init__.py
+-rw-r--r--   0        0        0    24550 2023-06-17 01:45:40.924329 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/kafka/services/kafka_actor_service.py
+-rw-r--r--   0        0        0     5715 2023-06-17 01:45:40.924612 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/kafka/services/kafka_authority_service.py
+-rw-r--r--   0        0        0     5797 2023-06-17 01:45:40.924963 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/kafka/services/kafka_broker_service.py
+-rw-r--r--   0        0        0    15846 2023-06-17 01:45:40.925294 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/kafka/services/kafka_client_actor_service.py
+-rw-r--r--   0        0        0     4008 2023-06-17 01:45:40.925501 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/kafka/services/kafka_controller_service.py
+-rw-r--r--   0        0        0     8228 2023-06-17 01:45:40.930286 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/kafka/services/kafka_server_actor_service.py
+-rw-r--r--   0        0        0     2148 2023-06-17 01:45:40.930647 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/kafka/services/kafka_service.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.931033 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/local/__init__.py
+-rw-r--r--   0        0        0    11782 2023-06-17 01:45:40.931261 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/local/local_actor.py
+-rw-r--r--   0        0        0     3902 2023-06-17 01:45:40.932273 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/local/local_authority.py
+-rw-r--r--   0        0        0     8391 2023-06-17 01:45:40.932650 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/local/local_broker.py
+-rw-r--r--   0        0        0    10119 2023-06-17 01:45:40.932861 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/local/local_container.py
+-rw-r--r--   0        0        0     9646 2023-06-17 01:45:40.933065 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/local/local_controller.py
+-rw-r--r--   0        0        0     2954 2023-06-17 01:45:40.933241 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/local/local_proxy.py
+-rw-r--r--   0        0        0     8655 2023-06-17 01:45:40.933384 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/local/local_server_actor.py
+-rw-r--r--   0        0        0     7217 2023-06-17 01:45:40.933585 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/management_object.py
+-rw-r--r--   0        0        0     7841 2023-06-17 01:45:40.933855 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/management_object_manager.py
+-rw-r--r--   0        0        0     4972 2023-06-17 01:45:40.934076 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/management_utils.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.934263 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/messages/__init__.py
+-rw-r--r--   0        0        0     1604 2023-06-17 01:45:40.934481 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/messages/client_mng.py
+-rw-r--r--   0        0        0     1570 2023-06-17 01:45:40.934692 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/messages/event_mng.py
+-rw-r--r--   0        0        0     1802 2023-06-17 01:45:40.934924 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/messages/protocol_proxy_mng.py
+-rw-r--r--   0        0        0     1741 2023-06-17 01:45:40.938560 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/messages/result_client_mng.py
+-rw-r--r--   0        0        0     1554 2023-06-17 01:45:40.938854 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/messages/result_event_mng.py
+-rw-r--r--   0        0        0     1904 2023-06-17 01:45:40.939179 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/proxy_protocol_descriptor.py
+-rw-r--r--   0        0        0    15777 2023-06-17 01:45:40.939532 fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/server_actor_management_object.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.939771 fabric_cf-1.5.1rc0/fabric_cf/actor/core/plugins/__init__.py
+-rw-r--r--   0        0        0     7965 2023-06-17 01:45:40.940014 fabric_cf-1.5.1rc0/fabric_cf/actor/core/plugins/base_plugin.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.940197 fabric_cf-1.5.1rc0/fabric_cf/actor/core/plugins/db/__init__.py
+-rw-r--r--   0        0        0    35944 2023-06-17 01:45:40.940502 fabric_cf-1.5.1rc0/fabric_cf/actor/core/plugins/db/actor_database.py
+-rw-r--r--   0        0        0     2624 2023-06-17 01:45:40.940665 fabric_cf-1.5.1rc0/fabric_cf/actor/core/plugins/db/client_database.py
+-rw-r--r--   0        0        0     3792 2023-06-17 01:45:40.940816 fabric_cf-1.5.1rc0/fabric_cf/actor/core/plugins/db/server_actor_database.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.941005 fabric_cf-1.5.1rc0/fabric_cf/actor/core/plugins/handlers/__init__.py
+-rw-r--r--   0        0        0    13211 2023-06-17 01:45:40.941275 fabric_cf-1.5.1rc0/fabric_cf/actor/core/plugins/handlers/ansible_handler_processor.py
+-rw-r--r--   0        0        0     2955 2023-06-17 01:45:40.941502 fabric_cf-1.5.1rc0/fabric_cf/actor/core/plugins/handlers/config_token.py
+-rw-r--r--   0        0        0     2286 2023-06-17 01:45:40.941792 fabric_cf-1.5.1rc0/fabric_cf/actor/core/plugins/handlers/configuration_mapping.py
+-rw-r--r--   0        0        0     7556 2023-06-17 01:45:40.942008 fabric_cf-1.5.1rc0/fabric_cf/actor/core/plugins/handlers/handler_processor.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.942195 fabric_cf-1.5.1rc0/fabric_cf/actor/core/plugins/substrate/__init__.py
+-rw-r--r--   0        0        0     3612 2023-06-17 01:45:40.942499 fabric_cf-1.5.1rc0/fabric_cf/actor/core/plugins/substrate/authority_substrate.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.942688 fabric_cf-1.5.1rc0/fabric_cf/actor/core/plugins/substrate/db/__init__.py
+-rw-r--r--   0        0        0     4365 2023-06-17 01:45:40.942906 fabric_cf-1.5.1rc0/fabric_cf/actor/core/plugins/substrate/db/substrate_actor_database.py
+-rw-r--r--   0        0        0    16974 2023-06-17 01:45:40.943189 fabric_cf-1.5.1rc0/fabric_cf/actor/core/plugins/substrate/substrate_mixin.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.943461 fabric_cf-1.5.1rc0/fabric_cf/actor/core/policy/__init__.py
+-rw-r--r--   0        0        0    28295 2023-06-17 01:45:40.943685 fabric_cf-1.5.1rc0/fabric_cf/actor/core/policy/authority_calendar_policy.py
+-rw-r--r--   0        0        0     8891 2023-06-17 01:45:40.944049 fabric_cf-1.5.1rc0/fabric_cf/actor/core/policy/broker_calendar_policy.py
+-rw-r--r--   0        0        0    64810 2023-06-17 01:45:40.944341 fabric_cf-1.5.1rc0/fabric_cf/actor/core/policy/broker_simpler_units_policy.py
+-rw-r--r--   0        0        0    19840 2023-06-17 01:45:40.944655 fabric_cf-1.5.1rc0/fabric_cf/actor/core/policy/controller_calendar_policy.py
+-rw-r--r--   0        0        0     9815 2023-06-17 01:45:40.944901 fabric_cf-1.5.1rc0/fabric_cf/actor/core/policy/controller_simple_policy.py
+-rw-r--r--   0        0        0     9546 2023-06-17 01:45:40.945130 fabric_cf-1.5.1rc0/fabric_cf/actor/core/policy/controller_ticket_review_policy.py
+-rw-r--r--   0        0        0     1814 2023-06-17 01:45:40.945299 fabric_cf-1.5.1rc0/fabric_cf/actor/core/policy/fifo_queue.py
+-rw-r--r--   0        0        0     2981 2023-06-17 01:45:40.945644 fabric_cf-1.5.1rc0/fabric_cf/actor/core/policy/inventory.py
+-rw-r--r--   0        0        0     2785 2023-06-17 01:45:40.945901 fabric_cf-1.5.1rc0/fabric_cf/actor/core/policy/inventory_for_type.py
+-rw-r--r--   0        0        0    14503 2023-06-17 01:45:40.946128 fabric_cf-1.5.1rc0/fabric_cf/actor/core/policy/network_node_control.py
+-rw-r--r--   0        0        0    28393 2023-06-17 01:45:40.946455 fabric_cf-1.5.1rc0/fabric_cf/actor/core/policy/network_node_inventory.py
+-rw-r--r--   0        0        0     5435 2023-06-17 01:45:40.946792 fabric_cf-1.5.1rc0/fabric_cf/actor/core/policy/network_service_control.py
+-rw-r--r--   0        0        0    22745 2023-06-17 01:45:40.947080 fabric_cf-1.5.1rc0/fabric_cf/actor/core/policy/network_service_inventory.py
+-rw-r--r--   0        0        0     2032 2023-06-17 01:45:40.947821 fabric_cf-1.5.1rc0/fabric_cf/actor/core/policy/queue_wrapper.py
+-rw-r--r--   0        0        0     5157 2023-06-17 01:45:40.948155 fabric_cf-1.5.1rc0/fabric_cf/actor/core/policy/resource_control.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.948359 fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/__init__.py
+-rw-r--r--   0        0        0     1821 2023-06-17 01:45:40.948682 fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/actor_location.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.948972 fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/kafka/__init__.py
+-rw-r--r--   0        0        0     8301 2023-06-17 01:45:40.949135 fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/kafka/kafka_authority_proxy.py
+-rw-r--r--   0        0        0     8924 2023-06-17 01:45:40.949314 fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/kafka/kafka_broker_proxy.py
+-rw-r--r--   0        0        0     6744 2023-06-17 01:45:40.949489 fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/kafka/kafka_proxy.py
+-rw-r--r--   0        0        0     4809 2023-06-17 01:45:40.949629 fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/kafka/kafka_proxy_factory.py
+-rw-r--r--   0        0        0     9066 2023-06-17 01:45:40.949823 fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/kafka/kafka_retun.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.949986 fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/kafka/services/__init__.py
+-rw-r--r--   0        0        0    12672 2023-06-17 01:45:40.950307 fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/kafka/services/actor_service.py
+-rw-r--r--   0        0        0     7627 2023-06-17 01:45:40.950544 fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/kafka/services/authority_service.py
+-rw-r--r--   0        0        0     8288 2023-06-17 01:45:40.950739 fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/kafka/services/broker_service.py
+-rw-r--r--   0        0        0     1380 2023-06-17 01:45:40.950952 fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/kafka/services/controller_service.py
+-rw-r--r--   0        0        0    19171 2023-06-17 01:45:40.951226 fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/kafka/translate.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.951442 fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/local/__init__.py
+-rw-r--r--   0        0        0     4948 2023-06-17 01:45:40.951647 fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/local/local_authority.py
+-rw-r--r--   0        0        0     5754 2023-06-17 01:45:40.951817 fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/local/local_broker.py
+-rw-r--r--   0        0        0     6924 2023-06-17 01:45:40.951994 fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/local/local_proxy.py
+-rw-r--r--   0        0        0     2868 2023-06-17 01:45:40.952145 fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/local/local_proxy_factory.py
+-rw-r--r--   0        0        0     6762 2023-06-17 01:45:40.952314 fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/local/local_return.py
+-rw-r--r--   0        0        0     8222 2023-06-17 01:45:40.952505 fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/proxy.py
+-rw-r--r--   0        0        0     3013 2023-06-17 01:45:40.952660 fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/proxy_factory.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.952814 fabric_cf-1.5.1rc0/fabric_cf/actor/core/registry/__init__.py
+-rw-r--r--   0        0        0     7672 2023-06-17 01:45:40.952963 fabric_cf-1.5.1rc0/fabric_cf/actor/core/registry/actor_registry.py
+-rw-r--r--   0        0        0     2177 2023-06-17 01:45:40.953134 fabric_cf-1.5.1rc0/fabric_cf/actor/core/registry/callback_registry.py
+-rw-r--r--   0        0        0     4926 2023-06-17 01:45:40.953314 fabric_cf-1.5.1rc0/fabric_cf/actor/core/registry/peer_registry.py
+-rw-r--r--   0        0        0     3912 2023-06-17 01:45:40.953470 fabric_cf-1.5.1rc0/fabric_cf/actor/core/registry/proxy_registry.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.953647 fabric_cf-1.5.1rc0/fabric_cf/actor/core/time/__init__.py
+-rw-r--r--   0        0        0     7165 2023-06-17 01:45:40.953843 fabric_cf-1.5.1rc0/fabric_cf/actor/core/time/actor_clock.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.954075 fabric_cf-1.5.1rc0/fabric_cf/actor/core/time/calendar/__init__.py
+-rw-r--r--   0        0        0     8224 2023-06-17 01:45:40.954310 fabric_cf-1.5.1rc0/fabric_cf/actor/core/time/calendar/authority_calendar.py
+-rw-r--r--   0        0        0     1667 2023-06-17 01:45:40.954596 fabric_cf-1.5.1rc0/fabric_cf/actor/core/time/calendar/base_calendar.py
+-rw-r--r--   0        0        0    11573 2023-06-17 01:45:40.954880 fabric_cf-1.5.1rc0/fabric_cf/actor/core/time/calendar/broker_calendar.py
+-rw-r--r--   0        0        0     9733 2023-06-17 01:45:40.955112 fabric_cf-1.5.1rc0/fabric_cf/actor/core/time/calendar/client_calendar.py
+-rw-r--r--   0        0        0     5239 2023-06-17 01:45:40.955329 fabric_cf-1.5.1rc0/fabric_cf/actor/core/time/calendar/controller_calendar.py
+-rw-r--r--   0        0        0     2550 2023-06-17 01:45:40.955506 fabric_cf-1.5.1rc0/fabric_cf/actor/core/time/calendar/source_calendar.py
+-rw-r--r--   0        0        0    15769 2023-06-17 01:45:40.955735 fabric_cf-1.5.1rc0/fabric_cf/actor/core/time/term.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.955915 fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/__init__.py
+-rw-r--r--   0        0        0     2213 2023-06-17 01:45:40.956146 fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/bids.py
+-rw-r--r--   0        0        0     2905 2023-06-17 01:45:40.956611 fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/client.py
+-rw-r--r--   0        0        0     2063 2023-06-17 01:45:40.956844 fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/graceful_interrupt_handler.py
+-rw-r--r--   0        0        0     2163 2023-06-17 01:45:40.957085 fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/id.py
+-rw-r--r--   0        0        0     1488 2023-06-17 01:45:40.957236 fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/iterable_queue.py
+-rw-r--r--   0        0        0     2263 2023-06-17 01:45:40.957481 fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/kernel_timer.py
+-rw-r--r--   0        0        0     3231 2023-06-17 01:45:40.957672 fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/log_helper.py
+-rw-r--r--   0        0        0     2238 2023-06-17 01:45:40.957969 fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/notice.py
+-rw-r--r--   0        0        0     1999 2023-06-17 01:45:40.958176 fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/reflection_utils.py
+-rw-r--r--   0        0        0     8380 2023-06-17 01:45:40.958377 fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/reservation_holdings.py
+-rw-r--r--   0        0        0     8864 2023-06-17 01:45:40.958575 fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/reservation_list.py
+-rw-r--r--   0        0        0     6700 2023-06-17 01:45:40.958776 fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/reservation_set.py
+-rw-r--r--   0        0        0     3144 2023-06-17 01:45:40.975106 fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/reservation_state.py
+-rw-r--r--   0        0        0     2250 2023-06-17 01:45:40.976043 fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/resource_type.py
+-rw-r--r--   0        0        0     1690 2023-06-17 01:45:40.976247 fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/rpc_exception.py
+-rw-r--r--   0        0        0     4440 2023-06-17 01:45:40.976429 fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/update_data.py
+-rw-r--r--   0        0        0     4188 2023-06-17 01:45:40.976626 fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/utils.py
+-rw-r--r--   0        0        0     8424 2023-06-17 01:45:40.976889 fabric_cf-1.5.1rc0/fabric_cf/actor/db/__init__.py
+-rw-r--r--   0        0        0    63500 2023-06-17 01:45:40.977548 fabric_cf-1.5.1rc0/fabric_cf/actor/db/psql_database.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.977745 fabric_cf-1.5.1rc0/fabric_cf/actor/fim/__init__.py
+-rw-r--r--   0        0        0     6326 2023-06-17 01:45:40.980858 fabric_cf-1.5.1rc0/fabric_cf/actor/fim/asm_update_thread.py
+-rw-r--r--   0        0        0    28243 2023-06-17 01:45:40.981251 fabric_cf-1.5.1rc0/fabric_cf/actor/fim/fim_helper.py
+-rw-r--r--   0        0        0        1 2023-06-17 01:45:40.981553 fabric_cf-1.5.1rc0/fabric_cf/actor/fim/plugins/__init__.py
+-rw-r--r--   0        0        0        1 2023-06-17 01:45:40.981784 fabric_cf-1.5.1rc0/fabric_cf/actor/fim/plugins/broker/__init__.py
+-rw-r--r--   0        0        0    23911 2023-06-17 01:45:40.982102 fabric_cf-1.5.1rc0/fabric_cf/actor/fim/plugins/broker/aggregate_bqm_plugin.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.982321 fabric_cf-1.5.1rc0/fabric_cf/actor/handlers/__init__.py
+-rw-r--r--   0        0        0     3015 2023-06-17 01:45:40.982541 fabric_cf-1.5.1rc0/fabric_cf/actor/handlers/handler_base.py
+-rw-r--r--   0        0        0    11187 2023-06-17 01:45:40.982734 fabric_cf-1.5.1rc0/fabric_cf/actor/handlers/no_op_handler.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.983200 fabric_cf-1.5.1rc0/fabric_cf/actor/security/__init__.py
+-rw-r--r--   0        0        0     4918 2023-06-17 01:45:40.983547 fabric_cf-1.5.1rc0/fabric_cf/actor/security/access_checker.py
+-rw-r--r--   0        0        0     2955 2023-06-17 01:45:40.983796 fabric_cf-1.5.1rc0/fabric_cf/actor/security/auth_token.py
+-rw-r--r--   0        0        0     3983 2023-06-17 01:45:40.983962 fabric_cf-1.5.1rc0/fabric_cf/actor/security/fabric_token.py
+-rw-r--r--   0        0        0     8648 2023-06-17 01:45:40.984098 fabric_cf-1.5.1rc0/fabric_cf/actor/security/pdp_auth.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.984252 fabric_cf-1.5.1rc0/fabric_cf/actor/test/__init__.py
+-rw-r--r--   0        0        0    10932 2023-06-17 01:45:40.984443 fabric_cf-1.5.1rc0/fabric_cf/actor/test/base_test_case.py
+-rw-r--r--   0        0        0     4679 2023-06-17 01:45:40.984642 fabric_cf-1.5.1rc0/fabric_cf/actor/test/client_callback_helper.py
+-rw-r--r--   0        0        0     4639 2023-06-17 01:45:40.984925 fabric_cf-1.5.1rc0/fabric_cf/actor/test/config/config.jenkins.yaml
+-rw-r--r--   0        0        0     4305 2023-06-17 01:45:40.985097 fabric_cf-1.5.1rc0/fabric_cf/actor/test/config/config.orchestrator.yaml
+-rw-r--r--   0        0        0     4696 2023-06-17 01:45:40.985241 fabric_cf-1.5.1rc0/fabric_cf/actor/test/config/config.test.yaml
+-rw-r--r--   0        0        0     5376 2023-06-17 01:45:40.985386 fabric_cf-1.5.1rc0/fabric_cf/actor/test/controller_callback_helper.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.985524 fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.985675 fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/container/__init__.py
+-rw-r--r--   0        0        0     2815 2023-06-17 01:45:40.985925 fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/container/container_database_test.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.986083 fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/core/__init__.py
+-rw-r--r--   0        0        0     4091 2023-06-17 01:45:40.986364 fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/core/unit_test.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.986519 fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/kernel/__init__.py
+-rw-r--r--   0        0        0    21480 2023-06-17 01:45:40.986761 fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/kernel/kernel_test.py
+-rw-r--r--   0        0        0     3378 2023-06-17 01:45:40.986972 fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/kernel/tick_test.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.987112 fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/plugins/__init__.py
+-rw-r--r--   0        0        0     3176 2023-06-17 01:45:40.987276 fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/plugins/actor_database_test.py
+-rw-r--r--   0        0        0     4729 2023-06-17 01:45:40.987542 fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/plugins/ansible_handler_processor_test.py
+-rw-r--r--   0        0        0     1963 2023-06-17 01:45:40.987733 fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/plugins/authority_substrate_test.py
+-rw-r--r--   0        0        0     3263 2023-06-17 01:45:40.987902 fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/plugins/substrate_database_test.py
+-rw-r--r--   0        0        0     2280 2023-06-17 01:45:40.988551 fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/plugins/substrate_test_base.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.988730 fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/policy/__init__.py
+-rw-r--r--   0        0        0    21995 2023-06-17 01:45:40.988906 fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/policy/authoity_calendar_policy_test.py
+-rw-r--r--   0        0        0    23678 2023-06-17 01:45:40.989174 fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/policy/broker_simpler_units_policy_test.py
+-rw-r--r--   0        0        0     4515 2023-06-17 01:45:40.989592 fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/policy/controller_simple_policy_test.py
+-rw-r--r--   0        0        0     1561 2023-06-17 01:45:40.989880 fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/policy/controller_simple_policy_test_wrapper.py
+-rw-r--r--   0        0        0     8437 2023-06-17 01:45:40.990111 fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/policy/controller_test_wrapper.py
+-rw-r--r--   0        0        0     7719 2023-06-17 01:45:40.990315 fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/policy/controller_ticket_review_policy_test.py
+-rw-r--r--   0        0        0     1586 2023-06-17 01:45:40.990499 fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/policy/controller_ticket_review_policy_test_wrapper.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.990668 fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/time/__init__.py
+-rw-r--r--   0        0        0     3786 2023-06-17 01:45:40.990929 fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/time/actor_clock_test.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.991081 fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/time/calendar/__init__.py
+-rw-r--r--   0        0        0     4290 2023-06-17 01:45:40.991264 fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/time/calendar/client_calendar_test.py
+-rw-r--r--   0        0        0     2225 2023-06-17 01:45:40.991433 fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/time/calendar/controller_calendar_test.py
+-rw-r--r--   0        0        0    14887 2023-06-17 01:45:40.991628 fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/time/term_test.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.991779 fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/util/__init__.py
+-rw-r--r--   0        0        0     8041 2023-06-17 01:45:40.991983 fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/util/reservation_holdings_test.py
+-rw-r--r--   0        0        0     5072 2023-06-17 01:45:40.992144 fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/util/reservation_list_test.py
+-rw-r--r--   0        0        0     3738 2023-06-17 01:45:40.992339 fabric_cf-1.5.1rc0/fabric_cf/actor/test/dummy_authority_proxy.py
+-rw-r--r--   0        0        0     1953 2023-06-17 01:45:40.992515 fabric_cf-1.5.1rc0/fabric_cf/actor/test/dummy_proxy.py
+-rw-r--r--   0        0        0     2498 2023-06-17 01:45:40.992704 fabric_cf-1.5.1rc0/fabric_cf/actor/test/fim_test_helper.py
+-rw-r--r--   0        0        0       92 2023-06-17 01:45:40.992923 fabric_cf-1.5.1rc0/fabric_cf/actor/test/schema/key.avsc
+-rw-r--r--   0        0        0    27389 2023-06-17 01:45:40.993152 fabric_cf-1.5.1rc0/fabric_cf/actor/test/schema/message.avsc
+-rw-r--r--   0        0        0     4532 2023-06-17 01:45:40.993409 fabric_cf-1.5.1rc0/fabric_cf/actor/test/test_abqm.py
+-rw-r--r--   0        0        0     1892 2023-06-17 01:45:40.993760 fabric_cf-1.5.1rc0/fabric_cf/actor/test/test_actor.py
+-rw-r--r--   0        0        0     1249 2023-06-17 01:45:40.994040 fabric_cf-1.5.1rc0/fabric_cf/actor/test/test_exception.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.994219 fabric_cf-1.5.1rc0/fabric_cf/aits/__init__.py
+-rw-r--r--   0        0        0     4826 2023-06-17 01:45:40.994452 fabric_cf-1.5.1rc0/fabric_cf/aits/config/config.broker.yaml
+-rw-r--r--   0        0        0     4808 2023-06-17 01:45:40.994616 fabric_cf-1.5.1rc0/fabric_cf/aits/config/config.netam.yaml
+-rw-r--r--   0        0        0     4414 2023-06-17 01:45:40.994771 fabric_cf-1.5.1rc0/fabric_cf/aits/config/config.orchestrator.yaml
+-rw-r--r--   0        0        0     4788 2023-06-17 01:45:40.994923 fabric_cf-1.5.1rc0/fabric_cf/aits/config/config.siteam.yaml
+-rw-r--r--   0        0        0    49220 2023-06-17 01:45:40.995231 fabric_cf-1.5.1rc0/fabric_cf/aits/integration_test.py
+-rw-r--r--   0        0        0     7393 2023-06-17 01:45:40.995500 fabric_cf-1.5.1rc0/fabric_cf/aits/kafka_processor.py
+-rw-r--r--   0        0        0     8633 2023-06-17 01:45:40.995812 fabric_cf-1.5.1rc0/fabric_cf/aits/manage_helper.py
+-rw-r--r--   0        0        0     8339 2023-06-17 01:45:40.996037 fabric_cf-1.5.1rc0/fabric_cf/aits/orchestrator_helper.py
+-rw-r--r--   0        0        0    16256 2023-06-17 01:45:40.996423 fabric_cf-1.5.1rc0/fabric_cf/authority/Readme.md
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.996512 fabric_cf-1.5.1rc0/fabric_cf/authority/__init__.py
+-rw-r--r--   0        0        0     2164 2023-06-17 01:45:40.996707 fabric_cf-1.5.1rc0/fabric_cf/authority/__main__.py
+-rw-r--r--   0        0        0    32973 2023-06-17 01:45:40.997055 fabric_cf-1.5.1rc0/fabric_cf/authority/am-yes.xml
+-rw-r--r--   0        0        0     5020 2023-06-17 01:45:40.997335 fabric_cf-1.5.1rc0/fabric_cf/authority/config.al2s.am.yaml
+-rw-r--r--   0        0        0     5114 2023-06-17 01:45:40.997490 fabric_cf-1.5.1rc0/fabric_cf/authority/config.net.am.yaml
+-rw-r--r--   0        0        0     5485 2023-06-17 01:45:40.997644 fabric_cf-1.5.1rc0/fabric_cf/authority/config.site.am.geni.yaml
+-rw-r--r--   0        0        0     4979 2023-06-17 01:45:40.997810 fabric_cf-1.5.1rc0/fabric_cf/authority/config.site.am.yaml
+-rw-r--r--   0        0        0     3427 2023-06-17 01:45:40.998006 fabric_cf-1.5.1rc0/fabric_cf/authority/docker-compose.geni.yml
+-rw-r--r--   0        0        0     3336 2023-06-17 01:45:40.998182 fabric_cf-1.5.1rc0/fabric_cf/authority/docker-compose.yml
+-rw-r--r--   0        0        0     1188 2023-06-17 01:45:40.998383 fabric_cf-1.5.1rc0/fabric_cf/authority/env.template
+-rw-r--r--   0        0        0    16080 2023-06-17 01:45:40.998552 fabric_cf-1.5.1rc0/fabric_cf/authority/fabricYes.AnyActorYesPolicy.xml
+-rw-r--r--   0        0        0     1588 2023-06-17 01:45:40.999003 fabric_cf-1.5.1rc0/fabric_cf/authority/net_handler_config.yml
+-rw-r--r--   0        0        0     1523 2023-06-17 01:45:40.999213 fabric_cf-1.5.1rc0/fabric_cf/authority/oess_handler_config.yml
+-rw-r--r--   0        0        0     1380 2023-06-17 01:45:40.999387 fabric_cf-1.5.1rc0/fabric_cf/authority/pdp.xml
+-rwxr-xr-x   0        0        0     2446 2023-06-17 01:45:40.999615 fabric_cf-1.5.1rc0/fabric_cf/authority/setup.sh
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:40.999779 fabric_cf-1.5.1rc0/fabric_cf/authority/test/__init__.py
+-rw-r--r--   0        0        0     2463 2023-06-17 01:45:41.000141 fabric_cf-1.5.1rc0/fabric_cf/authority/test/al2s_am.py
+-rw-r--r--   0        0        0     2459 2023-06-17 01:45:41.000375 fabric_cf-1.5.1rc0/fabric_cf/authority/test/net_am.py
+-rw-r--r--   0        0        0     2456 2023-06-17 01:45:41.000684 fabric_cf-1.5.1rc0/fabric_cf/authority/test/site_am.py
+-rw-r--r--   0        0        0     2461 2023-06-17 01:45:41.000983 fabric_cf-1.5.1rc0/fabric_cf/authority/test/site_am_geni.py
+-rw-r--r--   0        0        0     4730 2023-06-17 01:45:41.001160 fabric_cf-1.5.1rc0/fabric_cf/authority/test/test-al2sam.yaml
+-rw-r--r--   0        0        0     4839 2023-06-17 01:45:41.001406 fabric_cf-1.5.1rc0/fabric_cf/authority/test/test-netam.yaml
+-rw-r--r--   0        0        0     5071 2023-06-17 01:45:41.001616 fabric_cf-1.5.1rc0/fabric_cf/authority/test/test.geni.yaml
+-rw-r--r--   0        0        0     4685 2023-06-17 01:45:41.001778 fabric_cf-1.5.1rc0/fabric_cf/authority/test/test.yaml
+-rw-r--r--   0        0        0     2976 2023-06-17 01:45:41.001962 fabric_cf-1.5.1rc0/fabric_cf/authority/vm_handler_config.yml
+-rw-r--r--   0        0        0     1448 2023-06-17 01:45:41.002160 fabric_cf-1.5.1rc0/fabric_cf/authority/vnic_net_handler_config.yml
+-rw-r--r--   0        0        0    14262 2023-06-17 01:45:41.002472 fabric_cf-1.5.1rc0/fabric_cf/broker/Readme.md
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:41.002565 fabric_cf-1.5.1rc0/fabric_cf/broker/__init__.py
+-rw-r--r--   0        0        0     2290 2023-06-17 01:45:41.003027 fabric_cf-1.5.1rc0/fabric_cf/broker/__main__.py
+-rw-r--r--   0        0        0    27944 2023-06-17 01:45:41.003219 fabric_cf-1.5.1rc0/fabric_cf/broker/broker-yes.xml
+-rw-r--r--   0        0        0     5118 2023-06-17 01:45:41.003440 fabric_cf-1.5.1rc0/fabric_cf/broker/config.broker.yaml
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:41.003760 fabric_cf-1.5.1rc0/fabric_cf/broker/core/__init__.py
+-rw-r--r--   0        0        0     3314 2023-06-17 01:45:41.003951 fabric_cf-1.5.1rc0/fabric_cf/broker/core/broker_kernel.py
+-rw-r--r--   0        0        0     3135 2023-06-17 01:45:41.004136 fabric_cf-1.5.1rc0/fabric_cf/broker/docker-compose.yml
+-rw-r--r--   0        0        0     1192 2023-06-17 01:45:41.004298 fabric_cf-1.5.1rc0/fabric_cf/broker/env.template
+-rw-r--r--   0        0        0    16080 2023-06-17 01:45:41.004465 fabric_cf-1.5.1rc0/fabric_cf/broker/fabricYes.AnyActorYesPolicy.xml
+-rw-r--r--   0        0        0     1380 2023-06-17 01:45:41.004614 fabric_cf-1.5.1rc0/fabric_cf/broker/pdp.xml
+-rwxr-xr-x   0        0        0     2239 2023-06-17 01:45:41.004779 fabric_cf-1.5.1rc0/fabric_cf/broker/setup.sh
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:41.004943 fabric_cf-1.5.1rc0/fabric_cf/broker/test/__init__.py
+-rw-r--r--   0        0        0     2507 2023-06-17 01:45:41.005115 fabric_cf-1.5.1rc0/fabric_cf/broker/test/broker.py
+-rw-r--r--   0        0        0     5042 2023-06-17 01:45:41.005274 fabric_cf-1.5.1rc0/fabric_cf/broker/test/test.yaml
+-rw-r--r--   0        0        0    20305 2023-06-17 01:45:41.005618 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/README.md
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:41.005725 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/__init__.py
+-rw-r--r--   0        0        0     3355 2023-06-17 01:45:41.005996 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/__main__.py
+-rw-r--r--   0        0        0     1757 2023-06-17 01:45:41.006293 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/certs/fullchain.pem
+-rw-r--r--   0        0        0     3272 2023-06-17 01:45:41.006459 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/certs/privkey.pem
+-rw-r--r--   0        0        0     4942 2023-06-17 01:45:41.006620 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/config.orchestrator.yaml
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:41.006809 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/core/__init__.py
+-rw-r--r--   0        0        0     2917 2023-06-17 01:45:41.007109 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/core/active_status_checker.py
+-rw-r--r--   0        0        0     3050 2023-06-17 01:45:41.007322 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/core/bqm_wrapper.py
+-rw-r--r--   0        0        0     1556 2023-06-17 01:45:41.007535 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/core/exceptions.py
+-rw-r--r--   0        0        0     1884 2023-06-17 01:45:41.007756 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/core/i_status_update_callback.py
+-rw-r--r--   0        0        0    45517 2023-06-17 01:45:41.008024 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/core/orchestrator_handler.py
+-rw-r--r--   0        0        0     5389 2023-06-17 01:45:41.008315 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/core/orchestrator_kernel.py
+-rw-r--r--   0        0        0    34864 2023-06-17 01:45:41.008698 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/core/orchestrator_slice_wrapper.py
+-rw-r--r--   0        0        0     3581 2023-06-17 01:45:41.008921 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/core/reservation_converter.py
+-rw-r--r--   0        0        0     4880 2023-06-17 01:45:41.009087 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/core/reservation_status_update.py
+-rw-r--r--   0        0        0     7876 2023-06-17 01:45:41.009317 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/core/reservation_status_update_thread.py
+-rw-r--r--   0        0        0     7219 2023-06-17 01:45:41.009500 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/core/response_builder.py
+-rw-r--r--   0        0        0     8722 2023-06-17 01:45:41.009708 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/core/slice_defer_thread.py
+-rw-r--r--   0        0        0     1972 2023-06-17 01:45:41.009928 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/core/status_checker.py
+-rw-r--r--   0        0        0     1581 2023-06-17 01:45:41.010122 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/core/watch_entry.py
+-rw-r--r--   0        0        0     3501 2023-06-17 01:45:41.010272 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/docker-compose.yml
+-rw-r--r--   0        0        0     1198 2023-06-17 01:45:41.010413 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/env.template
+-rw-r--r--   0        0        0    72323 2023-06-17 01:45:41.010766 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/fabricTags.OrchestratorTags.xml
+-rw-r--r--   0        0        0     1626 2023-06-17 01:45:41.011039 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/nginx/default.conf
+-rw-r--r--   0        0        0    63932 2023-06-17 01:45:41.011346 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/openapi.json
+-rw-r--r--   0        0        0    30829 2023-06-17 01:45:41.011570 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/orchestrator-yes.xml
+-rw-r--r--   0        0        0     1548 2023-06-17 01:45:41.011868 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/pdp.xml
+-rwxr-xr-x   0        0        0     2284 2023-06-17 01:45:41.012060 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/setup.sh
+-rw-r--r--   0        0        0      430 2023-06-17 01:45:41.012320 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/__init__.py
+-rw-r--r--   0        0        0      392 2023-06-17 01:45:41.012550 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:41.012732 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/controllers/__init__.py
+-rw-r--r--   0        0        0      311 2023-06-17 01:45:41.012901 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/controllers/authorization_controller.py
+-rw-r--r--   0        0        0     1927 2023-06-17 01:45:41.013213 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/controllers/poas_controller.py
+-rw-r--r--   0        0        0     1249 2023-06-17 01:45:41.013431 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/controllers/resources_controller.py
+-rw-r--r--   0        0        0     7376 2023-06-17 01:45:41.013658 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/controllers/slices_controller.py
+-rw-r--r--   0        0        0     1094 2023-06-17 01:45:41.013842 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/controllers/slivers_controller.py
+-rw-r--r--   0        0        0      305 2023-06-17 01:45:41.014184 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/controllers/version_controller.py
+-rw-r--r--   0        0        0      631 2023-06-17 01:45:41.014347 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/encoder.py
+-rw-r--r--   0        0        0     2757 2023-06-17 01:45:41.014624 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/__init__.py
+-rw-r--r--   0        0        0     1889 2023-06-17 01:45:41.014783 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/base_model_.py
+-rw-r--r--   0        0        0     3400 2023-06-17 01:45:41.015057 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/poa.py
+-rw-r--r--   0        0        0     5315 2023-06-17 01:45:41.015243 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/poa_data.py
+-rw-r--r--   0        0        0     2624 2023-06-17 01:45:41.015477 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/poa_post.py
+-rw-r--r--   0        0        0     2712 2023-06-17 01:45:41.015650 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/poa_post_data.py
+-rw-r--r--   0        0        0     2254 2023-06-17 01:45:41.015812 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/poa_post_data_vcpu_cpu_map.py
+-rw-r--r--   0        0        0     1628 2023-06-17 01:45:41.015987 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/resource.py
+-rw-r--r--   0        0        0     3564 2023-06-17 01:45:41.016156 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/resources.py
+-rw-r--r--   0        0        0     7311 2023-06-17 01:45:41.016351 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/slice.py
+-rw-r--r--   0        0        0     3616 2023-06-17 01:45:41.016572 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/slice_details.py
+-rw-r--r--   0        0        0     5251 2023-06-17 01:45:41.016758 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/slices.py
+-rw-r--r--   0        0        0     2634 2023-06-17 01:45:41.016960 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/slices_post.py
+-rw-r--r--   0        0        0     8995 2023-06-17 01:45:41.017218 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/sliver.py
+-rw-r--r--   0        0        0     5301 2023-06-17 01:45:41.017484 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/slivers.py
+-rw-r--r--   0        0        0     3896 2023-06-17 01:45:41.017721 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/status200_ok_no_content.py
+-rw-r--r--   0        0        0     2464 2023-06-17 01:45:41.017937 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/status200_ok_no_content_data.py
+-rw-r--r--   0        0        0     4929 2023-06-17 01:45:41.018213 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/status200_ok_paginated.py
+-rw-r--r--   0        0        0     2870 2023-06-17 01:45:41.018413 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/status200_ok_single.py
+-rw-r--r--   0        0        0     1983 2023-06-17 01:45:41.018634 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/status400_bad_request.py
+-rw-r--r--   0        0        0     4503 2023-06-17 01:45:41.018806 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/status400_bad_request_errors.py
+-rw-r--r--   0        0        0     3984 2023-06-17 01:45:41.019013 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/status401_unauthorized.py
+-rw-r--r--   0        0        0     2512 2023-06-17 01:45:41.019195 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/status401_unauthorized_errors.py
+-rw-r--r--   0        0        0     3879 2023-06-17 01:45:41.019355 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/status403_forbidden.py
+-rw-r--r--   0        0        0     2461 2023-06-17 01:45:41.019600 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/status403_forbidden_errors.py
+-rw-r--r--   0        0        0     3846 2023-06-17 01:45:41.019907 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/status404_not_found.py
+-rw-r--r--   0        0        0     2446 2023-06-17 01:45:41.020139 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/status404_not_found_errors.py
+-rw-r--r--   0        0        0     4233 2023-06-17 01:45:41.020315 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/status500_internal_server_error.py
+-rw-r--r--   0        0        0     2635 2023-06-17 01:45:41.020482 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0     3540 2023-06-17 01:45:41.020652 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/version.py
+-rw-r--r--   0        0        0     2536 2023-06-17 01:45:41.020847 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/version_data.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:41.021020 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/response/__init__.py
+-rw-r--r--   0        0        0     1355 2023-06-17 01:45:41.021229 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/response/authorization_controller.py
+-rw-r--r--   0        0        0     1997 2023-06-17 01:45:41.021527 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/response/constants.py
+-rw-r--r--   0        0        0     5537 2023-06-17 01:45:41.021830 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/response/cors_response.py
+-rw-r--r--   0        0        0     5428 2023-06-17 01:45:41.022024 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/response/poas_controller.py
+-rw-r--r--   0        0        0     4321 2023-06-17 01:45:41.022194 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/response/resources_controller.py
+-rw-r--r--   0        0        0    15437 2023-06-17 01:45:41.022411 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/response/slices_controller.py
+-rw-r--r--   0        0        0     4642 2023-06-17 01:45:41.022563 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/response/slivers_controller.py
+-rw-r--r--   0        0        0     2530 2023-06-17 01:45:41.022725 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/response/utils.py
+-rw-r--r--   0        0        0     2632 2023-06-17 01:45:41.022874 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/response/version_controller.py
+-rw-r--r--   0        0        0    46265 2023-06-17 01:45:41.023351 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/swagger/swagger.yaml
+-rw-r--r--   0        0        0      438 2023-06-17 01:45:41.023754 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/test/__init__.py
+-rw-r--r--   0        0        0     2531 2023-06-17 01:45:41.023923 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/test/test_poas_controller.py
+-rw-r--r--   0        0        0     2094 2023-06-17 01:45:41.024150 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/test/test_resources_controller.py
+-rw-r--r--   0        0        0     5917 2023-06-17 01:45:41.024337 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/test/test_slices_controller.py
+-rw-r--r--   0        0        0     1989 2023-06-17 01:45:41.024516 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/test/test_slivers_controller.py
+-rw-r--r--   0        0        0      855 2023-06-17 01:45:41.024672 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/test/test_version_controller.py
+-rw-r--r--   0        0        0      809 2023-06-17 01:45:41.024927 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/type_util.py
+-rw-r--r--   0        0        0     3452 2023-06-17 01:45:41.025175 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/util.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:45:41.025447 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/test/__init__.py
+-rw-r--r--   0        0        0     3542 2023-06-17 01:45:41.025637 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/test/orchestrator.py
+-rwxr-xr-x   0        0        0       78 2023-06-17 01:45:41.025779 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/test/test.sh
+-rw-r--r--   0        0        0     4453 2023-06-17 01:45:41.025962 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/test/test.yaml
+-rwxr-xr-x   0        0        0     2900 2023-06-17 01:45:41.026171 fabric_cf-1.5.1rc0/fabric_cf/orchestrator/update_swagger_stub.sh
+-rw-r--r--   0        0        0    18177 2023-06-17 01:45:41.026554 fabric_cf-1.5.1rc0/images/am-pod.png
+-rw-r--r--   0        0        0    74927 2023-06-17 01:45:41.027412 fabric_cf-1.5.1rc0/images/am.png
+-rw-r--r--   0        0        0    18471 2023-06-17 01:45:41.027803 fabric_cf-1.5.1rc0/images/broker-pod.png
+-rw-r--r--   0        0        0    73799 2023-06-17 01:45:41.028849 fabric_cf-1.5.1rc0/images/broker.png
+-rw-r--r--   0        0        0    90831 2023-06-17 01:45:41.029809 fabric_cf-1.5.1rc0/images/cf.png
+-rw-r--r--   0        0        0    19611 2023-06-17 01:45:41.030274 fabric_cf-1.5.1rc0/images/orchestrator-pod.png
+-rw-r--r--   0        0        0    78622 2023-06-17 01:45:41.031009 fabric_cf-1.5.1rc0/images/orchestrator.png
+-rw-r--r--   0        0        0   145542 2023-06-17 01:45:41.031908 fabric_cf-1.5.1rc0/neo4j/AL2S.graphml
+-rw-r--r--   0        0        0    96363 2023-06-17 01:45:41.032689 fabric_cf-1.5.1rc0/neo4j/LBNL-ad.graphml
+-rw-r--r--   0        0        0    68182 2023-06-17 01:45:41.033202 fabric_cf-1.5.1rc0/neo4j/Network-ad.graphml
+-rw-r--r--   0        0        0   108181 2023-06-17 01:45:41.033710 fabric_cf-1.5.1rc0/neo4j/RENCI-ad.graphml
+-rw-r--r--   0        0        0    96286 2023-06-17 01:45:41.034122 fabric_cf-1.5.1rc0/neo4j/UKY-ad.graphml
+-rw-r--r--   0        0        0  1297955 2023-06-17 01:45:41.040536 fabric_cf-1.5.1rc0/neo4j/UKY2.graphml
+-rw-r--r--   0        0        0    14808 2023-06-17 01:45:41.041113 fabric_cf-1.5.1rc0/neo4j/abqm.graphml
+-rw-r--r--   0        0        0     1757 2023-06-17 01:45:41.041369 fabric_cf-1.5.1rc0/neo4j/certs/fullchain.pem
+-rw-r--r--   0        0        0     3272 2023-06-17 01:45:41.041560 fabric_cf-1.5.1rc0/neo4j/certs/privkey.pem
+-rwxr-xr-x   0        0        0       91 2023-06-17 01:45:41.041724 fabric_cf-1.5.1rc0/orchestrator.sh
+-rw-r--r--   0        0        0      698 2023-06-17 01:45:41.042025 fabric_cf-1.5.1rc0/psql.upgrade
+-rw-r--r--   0        0        0     1246 2023-06-17 01:46:28.206627 fabric_cf-1.5.1rc0/pyproject.toml
+-rwxr-xr-x   0        0        0     2594 2023-06-17 01:45:41.042472 fabric_cf-1.5.1rc0/secrets/create-certs.sh
+-rw-r--r--   0        0        0    12796 2023-06-17 01:45:41.042756 fabric_cf-1.5.1rc0/tools/audit.py
+-rw-r--r--   0        0        0     8005 2023-06-17 01:45:41.043087 fabric_cf-1.5.1rc0/tools/db_cli.py
+-rw-r--r--   0        0        0      354 2023-06-17 01:45:41.043268 fabric_cf-1.5.1rc0/tools/install.sh
+-rw-r--r--   0        0        0      143 2023-06-17 01:45:41.043421 fabric_cf-1.5.1rc0/tox.ini
+-rw-r--r--   0        0        0     3311 1970-01-01 00:00:00.000000 fabric_cf-1.5.1rc0/PKG-INFO
```

### Comparing `fabric_cf-1.5.0b5/.gitignore` & `fabric_cf-1.5.1rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/Dockerfile-auth` & `fabric_cf-1.5.1rc0/Dockerfile-auth`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 FROM python:3.9.0
 MAINTAINER Komal Thareja<komal.thareja@gmail.com>
 
-ARG HANDLERS_VER=1.5.0b8
+ARG HANDLERS_VER=1.5.1
 
 RUN mkdir -p /usr/src/app
 WORKDIR /usr/src/app
 VOLUME ["/usr/src/app"]
 
 EXPOSE 11000
```

### Comparing `fabric_cf-1.5.0b5/Dockerfile-broker` & `fabric_cf-1.5.1rc0/Dockerfile-broker`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/Dockerfile-cf` & `fabric_cf-1.5.1rc0/Dockerfile-cf`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/Dockerfile-orchestrator` & `fabric_cf-1.5.1rc0/Dockerfile-orchestrator`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/LICENSE` & `fabric_cf-1.5.1rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/README.md` & `fabric_cf-1.5.1rc0/README.md`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/cleanup_old_schema_from_schema_registry.sh` & `fabric_cf-1.5.1rc0/cleanup_old_schema_from_schema_registry.sh`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/docker-compose-kafka.yaml` & `fabric_cf-1.5.1rc0/docker-compose-kafka.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/docker-compose-no-ssl-kafka.yaml` & `fabric_cf-1.5.1rc0/docker-compose-no-ssl-kafka.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/docker-compose-test.yaml` & `fabric_cf-1.5.1rc0/docker-compose-test.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/env.template.test` & `fabric_cf-1.5.1rc0/env.template.test`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabricNo.AnyActorNoPolicy.xml` & `fabric_cf-1.5.1rc0/fabricNo.AnyActorNoPolicy.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/Design.md` & `fabric_cf-1.5.1rc0/fabric_cf/Design.md`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/boot/configuration.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/boot/configuration.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/boot/configuration_exception.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/boot/configuration_exception.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/boot/configuration_loader.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/boot/configuration_loader.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/boot/configuration_processor.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/boot/configuration_processor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/boot/inventory/aggregate_resource_model_creator.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/boot/inventory/aggregate_resource_model_creator.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_actor_container.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_actor_container.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_actor_event.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_actor_event.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_actor_identity.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_actor_identity.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_actor_management_object.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_actor_management_object.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_actor_mixin.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_actor_mixin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_actor_proxy.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_actor_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_actor_runnable.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_actor_runnable.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_authority.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_authority.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_authority_policy.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_authority_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_authority_proxy.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_authority_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_authority_reservation.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_authority_reservation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_base_plugin.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_base_plugin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_broker_mixin.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_broker_mixin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_broker_policy_mixin.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_broker_policy_mixin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_broker_proxy.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_broker_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_broker_reservation.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_broker_reservation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_callback_proxy.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_callback_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_client_actor.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_client_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_client_actor_management_object.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_client_actor_management_object.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_client_callback_proxy.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_client_callback_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_client_policy.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_client_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_client_reservation.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_client_reservation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_component.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_component.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_concrete_set.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_concrete_set.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_container_clock.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_container_clock.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_container_database.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_container_database.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_controller.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_controller_callback_proxy.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_controller_callback_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_controller_policy.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_controller_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_controller_reservation.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_controller_reservation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_database.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_database.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_delegation.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_delegation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_event.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_event.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_management_object.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_management_object.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_mgmt_actor.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_mgmt_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_mgmt_authority.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_mgmt_authority.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_mgmt_broker_mixin.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_mgmt_broker_mixin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_mgmt_client_actor.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_mgmt_client_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_mgmt_container.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_mgmt_container.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_mgmt_controller_mixin.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_mgmt_controller_mixin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_mgmt_server_actor.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_mgmt_server_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_policy.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_proxy.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_proxy_factory.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_query_response_handler.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_query_response_handler.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_reservation_mixin.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_reservation_mixin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_reservation_resources.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_reservation_resources.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_reservation_status.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_reservation_status.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_resource_control.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_resource_control.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_response_handler.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_response_handler.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_rpc_request_state.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_rpc_request_state.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_server_actor.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_server_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_server_policy.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_server_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_server_reservation.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_server_reservation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_slice.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_slice.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_substrate.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_substrate.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_substrate_database.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_substrate_database.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_tick.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_tick.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_ticker.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_ticker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_timer_queue.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_timer_queue.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/apis/abc_timer_task.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/apis/abc_timer_task.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/common/constants.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/common/constants.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/common/event_logger.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/common/event_logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                                             log_format=log_format)
 
     def log_slice_event(self, *, slice_object: SliceAvro, action: ActionId, topology: ExperimentTopology = None):
         """
         Log Slice Event for metrics
         """
         try:
-            log_message = f"CFEL Slice event slc:{slice_object.get_slice_name()}:{slice_object.get_slice_id()} " \
+            log_message = f"CFEL Slice event slc:{slice_object.get_slice_id()} " \
                           f"{action} by prj:{slice_object.get_project_id()} " \
                           f"usr:{slice_object.get_owner().get_oidc_sub_claim()}:{slice_object.get_owner().get_email()}"
 
             if topology is not None:
                 lc = LogCollector()
                 lc.collect_resource_attributes(source=topology)
                 log_message += f" {str(lc)}"
@@ -78,15 +78,15 @@
         """
         Log Sliver events
         """
         try:
             lc = LogCollector()
             lc.collect_resource_attributes(source=sliver)
 
-            log_message = f"CFEL Sliver event slc:{slice_object.get_slice_name()}:{slice_object.get_slice_id()} " \
+            log_message = f"CFEL Sliver event slc:{slice_object.get_slice_id()} " \
                           f"slvr:{sliver.get_reservation_info().reservation_id} of " \
                           f"type {sliver.get_type()} {sliver.get_reservation_info().reservation_state} " \
                           f"by prj:{slice_object.get_project_id()} usr:{slice_object.get_owner().get_oidc_sub_claim()}" \
                           f":{slice_object.get_owner().get_email()} {str(lc)}"
 
             self.logger.info(log_message)
         except Exception as e:
```

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/common/exceptions.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/common/resource_config.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/common/resource_config.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/container/container.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/container/container.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/container/db/container_database.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/container/db/container_database.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/container/globals.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/container/globals.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/container/maintenance.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/container/maintenance.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/container/message_service.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/container/message_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/container/protocol_descriptor.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/container/protocol_descriptor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/container/remote_actor_cache.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/container/remote_actor_cache.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/container/rpc_producer.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/container/rpc_producer.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/core/actor.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/core/actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/core/actor_identity.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/core/actor_identity.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/core/authority.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/core/authority.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/core/authority_policy.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/core/authority_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/core/broker.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/core/broker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/core/broker_policy.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/core/broker_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/core/controller.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/core/controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/core/event_processor.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/core/event_processor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/core/inventory_slice_manager.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/core/inventory_slice_manager.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/core/policy.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/core/policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/core/rpc_request_state.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/core/rpc_request_state.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/core/ticket.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/core/ticket.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/core/unit.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/core/unit.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/core/unit_set.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/core/unit_set.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/delegation/broker_delegation.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/delegation/broker_delegation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/delegation/broker_delegation_factory.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/delegation/broker_delegation_factory.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/delegation/delegation.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/delegation/delegation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/delegation/delegation_factory.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/delegation/delegation_factory.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/delegation/resource_ticket.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/delegation/resource_ticket.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/authority_reservation.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/authority_reservation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/broker_query_model_publisher.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/broker_query_model_publisher.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/broker_reservation.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/broker_reservation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/claim_timeout.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/claim_timeout.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/failed_rpc.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/failed_rpc.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/failed_rpc_event.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/failed_rpc_event.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/incoming_delegation_rpc.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/incoming_delegation_rpc.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/incoming_failed_rpc.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/incoming_failed_rpc.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/incoming_poa_rpc.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/incoming_poa_rpc.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/incoming_query_rpc.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/incoming_query_rpc.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/incoming_reservation_rpc.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/incoming_reservation_rpc.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/incoming_rpc.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/incoming_rpc.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/incoming_rpc_event.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/incoming_rpc_event.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/kernel.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/kernel.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/kernel_tick.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/kernel_tick.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/kernel_wrapper.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/kernel_wrapper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/poa.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/poa.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/predecessor_state.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/predecessor_state.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/query_timeout.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/query_timeout.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/request_types.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/request_types.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/reservation.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/reservation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/reservation_client.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/reservation_client.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/reservation_server.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/reservation_server.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/reservation_states.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/reservation_states.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/resource_set.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/resource_set.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/retry_rpc.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/retry_rpc.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/retry_rpc_event.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/retry_rpc_event.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/rpc_executor.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/rpc_executor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/rpc_manager.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/rpc_manager.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/rpc_manager_singleton.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/rpc_manager_singleton.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/rpc_request.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/rpc_request.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/rpc_request_type.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/rpc_request_type.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/sequence_comparison_codes.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/sequence_comparison_codes.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/slice.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/slice.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/slice_state_machine.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/slice_state_machine.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/slice_table.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/slice_table.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/kernel/tick.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/kernel/tick.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/actor_management_object.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/actor_management_object.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/authority_management_object.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/authority_management_object.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/broker_management_object.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/broker_management_object.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/client_actor_management_object_helper.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/client_actor_management_object_helper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/container_management_object.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/container_management_object.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/controller_management_object.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/controller_management_object.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/converter.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/converter.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/error.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/error.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/kafka/kafka_actor.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/kafka/kafka_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/kafka/kafka_authority.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/kafka/kafka_authority.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/kafka/kafka_broker.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/kafka/kafka_broker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/kafka/kafka_container.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/kafka/kafka_container.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/kafka/kafka_controller.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/kafka/kafka_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/kafka/kafka_mgmt_message_processor.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/kafka/kafka_mgmt_message_processor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/kafka/kafka_proxy.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/kafka/kafka_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/kafka/kafka_server_actor.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/kafka/kafka_server_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/kafka/services/kafka_actor_service.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/kafka/services/kafka_actor_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/kafka/services/kafka_authority_service.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/kafka/services/kafka_authority_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/kafka/services/kafka_broker_service.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/kafka/services/kafka_broker_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/kafka/services/kafka_client_actor_service.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/kafka/services/kafka_client_actor_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/kafka/services/kafka_controller_service.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/kafka/services/kafka_controller_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/kafka/services/kafka_server_actor_service.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/kafka/services/kafka_server_actor_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/kafka/services/kafka_service.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/kafka/services/kafka_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/local/local_actor.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/local/local_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/local/local_authority.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/local/local_authority.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/local/local_broker.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/local/local_broker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/local/local_container.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/local/local_container.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/local/local_controller.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/local/local_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/local/local_proxy.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/local/local_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/local/local_server_actor.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/local/local_server_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/management_object.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/management_object.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/management_object_manager.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/management_object_manager.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/management_utils.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/management_utils.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/messages/client_mng.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/messages/client_mng.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/messages/event_mng.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/messages/event_mng.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/messages/protocol_proxy_mng.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/messages/protocol_proxy_mng.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/messages/result_client_mng.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/messages/result_client_mng.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/messages/result_event_mng.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/messages/result_event_mng.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/proxy_protocol_descriptor.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/proxy_protocol_descriptor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/manage/server_actor_management_object.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/manage/server_actor_management_object.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/plugins/base_plugin.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/plugins/base_plugin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/plugins/db/actor_database.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/plugins/db/actor_database.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/plugins/db/client_database.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/plugins/db/client_database.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/plugins/db/server_actor_database.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/plugins/db/server_actor_database.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/plugins/handlers/ansible_handler_processor.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/plugins/handlers/ansible_handler_processor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/plugins/handlers/config_token.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/plugins/handlers/config_token.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/plugins/handlers/configuration_mapping.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/plugins/handlers/configuration_mapping.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/plugins/handlers/handler_processor.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/plugins/handlers/handler_processor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/plugins/substrate/authority_substrate.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/plugins/substrate/authority_substrate.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/plugins/substrate/db/substrate_actor_database.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/plugins/substrate/db/substrate_actor_database.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/plugins/substrate/substrate_mixin.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/plugins/substrate/substrate_mixin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/policy/authority_calendar_policy.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/policy/authority_calendar_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/policy/broker_calendar_policy.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/policy/broker_calendar_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/policy/broker_simpler_units_policy.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/policy/broker_simpler_units_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/policy/controller_calendar_policy.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/policy/controller_calendar_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/policy/controller_simple_policy.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/policy/controller_simple_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/policy/controller_ticket_review_policy.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/policy/controller_ticket_review_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/policy/fifo_queue.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/policy/fifo_queue.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/policy/inventory.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/policy/inventory.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/policy/inventory_for_type.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/policy/inventory_for_type.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/policy/network_node_control.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/policy/network_node_control.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/policy/network_node_inventory.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/policy/network_node_inventory.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/policy/network_service_control.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/policy/network_service_control.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/policy/network_service_inventory.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/policy/network_service_inventory.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/policy/queue_wrapper.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/policy/queue_wrapper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/policy/resource_control.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/policy/resource_control.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/actor_location.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/actor_location.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/kafka/kafka_authority_proxy.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/kafka/kafka_authority_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/kafka/kafka_broker_proxy.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/kafka/kafka_broker_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/kafka/kafka_proxy.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/kafka/kafka_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/kafka/kafka_proxy_factory.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/kafka/kafka_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/kafka/kafka_retun.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/kafka/kafka_retun.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/kafka/services/actor_service.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/kafka/services/actor_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/kafka/services/authority_service.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/kafka/services/authority_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/kafka/services/broker_service.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/kafka/services/broker_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/kafka/services/controller_service.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/kafka/services/controller_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/kafka/translate.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/kafka/translate.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/local/local_authority.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/local/local_authority.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/local/local_broker.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/local/local_broker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/local/local_proxy.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/local/local_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/local/local_proxy_factory.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/local/local_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/local/local_return.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/local/local_return.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/proxy.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/proxies/proxy_factory.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/proxies/proxy_factory.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/registry/actor_registry.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/registry/actor_registry.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/registry/callback_registry.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/registry/callback_registry.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/registry/peer_registry.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/registry/peer_registry.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/registry/proxy_registry.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/registry/proxy_registry.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/time/actor_clock.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/time/actor_clock.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/time/calendar/authority_calendar.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/time/calendar/authority_calendar.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/time/calendar/base_calendar.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/time/calendar/base_calendar.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/time/calendar/broker_calendar.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/time/calendar/broker_calendar.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/time/calendar/client_calendar.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/time/calendar/client_calendar.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/time/calendar/controller_calendar.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/time/calendar/controller_calendar.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/time/calendar/source_calendar.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/time/calendar/source_calendar.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/time/term.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/time/term.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/util/bids.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/bids.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/util/client.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/client.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/util/graceful_interrupt_handler.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/graceful_interrupt_handler.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/util/id.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/id.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/util/iterable_queue.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/iterable_queue.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/util/kernel_timer.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/kernel_timer.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/util/log_helper.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/log_helper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/util/notice.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/notice.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/util/reflection_utils.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/reflection_utils.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/util/reservation_holdings.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/reservation_holdings.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/util/reservation_list.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/reservation_list.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/util/reservation_set.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/reservation_set.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/util/reservation_state.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/reservation_state.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/util/resource_type.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/resource_type.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/util/rpc_exception.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/rpc_exception.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/util/update_data.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/update_data.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/core/util/utils.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/core/util/utils.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/db/__init__.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/db/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/db/psql_database.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/db/psql_database.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/fim/asm_update_thread.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/fim/asm_update_thread.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/fim/fim_helper.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/fim/fim_helper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/fim/plugins/broker/aggregate_bqm_plugin.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/fim/plugins/broker/aggregate_bqm_plugin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/handlers/handler_base.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/handlers/handler_base.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/handlers/no_op_handler.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/handlers/no_op_handler.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/security/access_checker.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/security/access_checker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/security/auth_token.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/security/auth_token.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/security/fabric_token.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/security/fabric_token.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/security/pdp_auth.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/security/pdp_auth.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/base_test_case.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/base_test_case.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/client_callback_helper.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/client_callback_helper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/config/config.jenkins.yaml` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/config/config.jenkins.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/config/config.orchestrator.yaml` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/config/config.orchestrator.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/config/config.test.yaml` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/config/config.test.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/controller_callback_helper.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/controller_callback_helper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/core/container/container_database_test.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/container/container_database_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/core/core/unit_test.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/core/unit_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/core/kernel/kernel_test.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/kernel/kernel_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/core/kernel/tick_test.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/kernel/tick_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/core/plugins/actor_database_test.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/plugins/actor_database_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/core/plugins/ansible_handler_processor_test.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/plugins/ansible_handler_processor_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/core/plugins/authority_substrate_test.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/plugins/authority_substrate_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/core/plugins/substrate_database_test.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/plugins/substrate_database_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/core/plugins/substrate_test_base.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/plugins/substrate_test_base.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/core/policy/authoity_calendar_policy_test.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/policy/authoity_calendar_policy_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/core/policy/broker_simpler_units_policy_test.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/policy/broker_simpler_units_policy_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/core/policy/controller_simple_policy_test.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/policy/controller_simple_policy_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/core/policy/controller_simple_policy_test_wrapper.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/policy/controller_simple_policy_test_wrapper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/core/policy/controller_test_wrapper.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/policy/controller_test_wrapper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/core/policy/controller_ticket_review_policy_test.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/policy/controller_ticket_review_policy_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/core/policy/controller_ticket_review_policy_test_wrapper.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/policy/controller_ticket_review_policy_test_wrapper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/core/time/actor_clock_test.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/time/actor_clock_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/core/time/calendar/client_calendar_test.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/time/calendar/client_calendar_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/core/time/calendar/controller_calendar_test.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/time/calendar/controller_calendar_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/core/time/term_test.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/time/term_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/core/util/reservation_holdings_test.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/util/reservation_holdings_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/core/util/reservation_list_test.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/core/util/reservation_list_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/dummy_authority_proxy.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/dummy_authority_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/dummy_proxy.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/dummy_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/fim_test_helper.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/fim_test_helper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/schema/message.avsc` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/schema/message.avsc`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/test_abqm.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/test_abqm.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/test_actor.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/test_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/actor/test/test_exception.py` & `fabric_cf-1.5.1rc0/fabric_cf/actor/test/test_exception.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/aits/config/config.broker.yaml` & `fabric_cf-1.5.1rc0/fabric_cf/aits/config/config.broker.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/aits/config/config.netam.yaml` & `fabric_cf-1.5.1rc0/fabric_cf/aits/config/config.netam.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/aits/config/config.orchestrator.yaml` & `fabric_cf-1.5.1rc0/fabric_cf/aits/config/config.orchestrator.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/aits/config/config.siteam.yaml` & `fabric_cf-1.5.1rc0/fabric_cf/aits/config/config.siteam.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/aits/integration_test.py` & `fabric_cf-1.5.1rc0/fabric_cf/aits/integration_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/aits/kafka_processor.py` & `fabric_cf-1.5.1rc0/fabric_cf/aits/kafka_processor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/aits/manage_helper.py` & `fabric_cf-1.5.1rc0/fabric_cf/aits/manage_helper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/aits/orchestrator_helper.py` & `fabric_cf-1.5.1rc0/fabric_cf/aits/orchestrator_helper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/authority/Readme.md` & `fabric_cf-1.5.1rc0/fabric_cf/authority/Readme.md`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/authority/__main__.py` & `fabric_cf-1.5.1rc0/fabric_cf/authority/__main__.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/authority/am-yes.xml` & `fabric_cf-1.5.1rc0/fabric_cf/authority/am-yes.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/authority/config.al2s.am.yaml` & `fabric_cf-1.5.1rc0/fabric_cf/authority/config.al2s.am.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/authority/config.net.am.yaml` & `fabric_cf-1.5.1rc0/fabric_cf/authority/config.net.am.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/authority/config.site.am.geni.yaml` & `fabric_cf-1.5.1rc0/fabric_cf/authority/config.site.am.geni.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/authority/config.site.am.yaml` & `fabric_cf-1.5.1rc0/fabric_cf/authority/config.site.am.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/authority/docker-compose.geni.yml` & `fabric_cf-1.5.1rc0/fabric_cf/authority/docker-compose.geni.yml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/authority/docker-compose.yml` & `fabric_cf-1.5.1rc0/fabric_cf/authority/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/authority/env.template` & `fabric_cf-1.5.1rc0/fabric_cf/authority/env.template`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/authority/fabricYes.AnyActorYesPolicy.xml` & `fabric_cf-1.5.1rc0/fabric_cf/authority/fabricYes.AnyActorYesPolicy.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/authority/net_handler_config.yml` & `fabric_cf-1.5.1rc0/fabric_cf/authority/net_handler_config.yml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/authority/oess_handler_config.yml` & `fabric_cf-1.5.1rc0/fabric_cf/authority/oess_handler_config.yml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/authority/pdp.xml` & `fabric_cf-1.5.1rc0/fabric_cf/authority/pdp.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/authority/setup.sh` & `fabric_cf-1.5.1rc0/fabric_cf/authority/setup.sh`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/authority/test/al2s_am.py` & `fabric_cf-1.5.1rc0/fabric_cf/authority/test/al2s_am.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/authority/test/net_am.py` & `fabric_cf-1.5.1rc0/fabric_cf/authority/test/net_am.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/authority/test/site_am.py` & `fabric_cf-1.5.1rc0/fabric_cf/authority/test/site_am.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/authority/test/site_am_geni.py` & `fabric_cf-1.5.1rc0/fabric_cf/authority/test/site_am_geni.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/authority/test/test-al2sam.yaml` & `fabric_cf-1.5.1rc0/fabric_cf/authority/test/test-al2sam.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/authority/test/test-netam.yaml` & `fabric_cf-1.5.1rc0/fabric_cf/authority/test/test-netam.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/authority/test/test.geni.yaml` & `fabric_cf-1.5.1rc0/fabric_cf/authority/test/test.geni.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/authority/test/test.yaml` & `fabric_cf-1.5.1rc0/fabric_cf/authority/test/test.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/authority/vm_handler_config.yml` & `fabric_cf-1.5.1rc0/fabric_cf/authority/vm_handler_config.yml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/authority/vnic_net_handler_config.yml` & `fabric_cf-1.5.1rc0/fabric_cf/authority/vnic_net_handler_config.yml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/broker/Readme.md` & `fabric_cf-1.5.1rc0/fabric_cf/broker/Readme.md`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/broker/__main__.py` & `fabric_cf-1.5.1rc0/fabric_cf/broker/__main__.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/broker/broker-yes.xml` & `fabric_cf-1.5.1rc0/fabric_cf/broker/broker-yes.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/broker/config.broker.yaml` & `fabric_cf-1.5.1rc0/fabric_cf/broker/config.broker.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/broker/core/broker_kernel.py` & `fabric_cf-1.5.1rc0/fabric_cf/broker/core/broker_kernel.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/broker/docker-compose.yml` & `fabric_cf-1.5.1rc0/fabric_cf/broker/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/broker/env.template` & `fabric_cf-1.5.1rc0/fabric_cf/broker/env.template`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/broker/fabricYes.AnyActorYesPolicy.xml` & `fabric_cf-1.5.1rc0/fabric_cf/broker/fabricYes.AnyActorYesPolicy.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/broker/pdp.xml` & `fabric_cf-1.5.1rc0/fabric_cf/broker/pdp.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/broker/setup.sh` & `fabric_cf-1.5.1rc0/fabric_cf/broker/setup.sh`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/broker/test/broker.py` & `fabric_cf-1.5.1rc0/fabric_cf/broker/test/broker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/broker/test/test.yaml` & `fabric_cf-1.5.1rc0/fabric_cf/broker/test/test.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/README.md` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/README.md`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/__main__.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/__main__.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/certs/fullchain.pem` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/certs/fullchain.pem`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/certs/privkey.pem` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/certs/privkey.pem`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/config.orchestrator.yaml` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/config.orchestrator.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/core/active_status_checker.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/core/active_status_checker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/core/bqm_wrapper.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/core/bqm_wrapper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/core/exceptions.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/core/i_status_update_callback.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/core/i_status_update_callback.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/core/orchestrator_handler.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/core/orchestrator_handler.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/core/orchestrator_kernel.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/core/orchestrator_kernel.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/core/orchestrator_slice_wrapper.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/core/orchestrator_slice_wrapper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/core/reservation_converter.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/core/reservation_converter.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/core/reservation_status_update.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/core/reservation_status_update.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/core/reservation_status_update_thread.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/core/reservation_status_update_thread.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/core/response_builder.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/core/response_builder.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/core/slice_defer_thread.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/core/slice_defer_thread.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/core/status_checker.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/core/status_checker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/core/watch_entry.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/core/watch_entry.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/docker-compose.yml` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/env.template` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/env.template`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/fabricTags.OrchestratorTags.xml` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/fabricTags.OrchestratorTags.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/nginx/default.conf` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/nginx/default.conf`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/openapi.json` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/openapi.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9915528711484595%*

 * *Differences: {"'components'": "{'requestBodies': {'Request': OrderedDict([('content', "*

 * *                 "OrderedDict([('text/plain', OrderedDict([('schema', OrderedDict([('type', "*

 * *                 "'string')]))]))])), ('required', True)])}}",*

 * * "'paths'": "{'/slices/create': {'post': {'parameters': {insert: [(1, OrderedDict([('name', "*

 * *            "'ssh_key'), ('in', 'query'), ('description', 'User SSH Key'), ('required', True), "*

 * *            "('style', 'form'), ('explode', True), ('schema', OrderedDict([('type', "*

 * *    […]*

```diff
@@ -1,10 +1,20 @@
 {
     "components": {
         "requestBodies": {
+            "Request": {
+                "content": {
+                    "text/plain": {
+                        "schema": {
+                            "type": "string"
+                        }
+                    }
+                },
+                "required": true
+            },
             "payload_poa": {
                 "content": {
                     "application/json": {
                         "schema": {
                             "$ref": "#/components/schemas/poa_post"
                         }
                     }
@@ -1305,14 +1315,129 @@
             "post": {
                 "description": "Request to create slice as described in the request. Request would be a graph ML describing the requested resources. Resources may be requested to be created now or in future. On success, one or more slivers are allocated, containing resources satisfying the request, and assigned to the given slice. This API returns list and description of the resources reserved for the slice in the form of Graph ML. Orchestrator would also trigger provisioning of these resources asynchronously on the appropriate sites either now or in the future as requested. Experimenter can invoke get slice API to get the latest state of the requested resources. \n",
                 "parameters": [
                     {
                         "description": "Slice Name",
                         "explode": true,
                         "in": "query",
+                        "name": "name",
+                        "required": true,
+                        "schema": {
+                            "minLength": 3,
+                            "type": "string"
+                        },
+                        "style": "form"
+                    },
+                    {
+                        "description": "User SSH Key",
+                        "explode": true,
+                        "in": "query",
+                        "name": "ssh_key",
+                        "required": true,
+                        "schema": {
+                            "type": "string"
+                        },
+                        "style": "form"
+                    },
+                    {
+                        "description": "Lease End Time for the Slice",
+                        "explode": true,
+                        "in": "query",
+                        "name": "lease_end_time",
+                        "required": false,
+                        "schema": {
+                            "type": "string"
+                        },
+                        "style": "form"
+                    }
+                ],
+                "requestBody": {
+                    "$ref": "#/components/requestBodies/Request"
+                },
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/slivers"
+                                }
+                            }
+                        },
+                        "description": "OK"
+                    },
+                    "400": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/status_400_bad_request"
+                                }
+                            }
+                        },
+                        "description": "Bad Request"
+                    },
+                    "401": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/status_401_unauthorized"
+                                }
+                            }
+                        },
+                        "description": "Unauthorized"
+                    },
+                    "403": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/status_403_forbidden"
+                                }
+                            }
+                        },
+                        "description": "Forbidden"
+                    },
+                    "404": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/status_404_not_found"
+                                }
+                            }
+                        },
+                        "description": "Not Found"
+                    },
+                    "500": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/status_500_internal_server_error"
+                                }
+                            }
+                        },
+                        "description": "Internal Server Error"
+                    }
+                },
+                "security": [
+                    {
+                        "bearerAuth": []
+                    }
+                ],
+                "summary": "Create slice",
+                "tags": [
+                    "slices"
+                ]
+            }
+        },
+        "/slices/creates": {
+            "post": {
+                "description": "Request to create slice as described in the request. Request would be a graph ML describing the requested resources. Resources may be requested to be created now or in future. On success, one or more slivers are allocated, containing resources satisfying the request, and assigned to the given slice. This API returns list and description of the resources reserved for the slice in the form of Graph ML. Orchestrator would also trigger provisioning of these resources asynchronously on the appropriate sites either now or in the future as requested. Experimenter can invoke get slice API to get the latest state of the requested resources. \n",
+                "parameters": [
+                    {
+                        "description": "Slice Name",
+                        "explode": true,
+                        "in": "query",
                         "name": "name",
                         "required": true,
                         "schema": {
                             "minLength": 3,
                             "type": "string"
                         },
                         "style": "form"
```

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/orchestrator-yes.xml` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/orchestrator-yes.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/pdp.xml` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/pdp.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/setup.sh` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/setup.sh`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/controllers/poas_controller.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/controllers/poas_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/controllers/resources_controller.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/controllers/resources_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/controllers/slices_controller.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/controllers/slices_controller.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,23 +5,50 @@
 from fabric_cf.orchestrator.swagger_server.models.slices import Slices  # noqa: E501
 from fabric_cf.orchestrator.swagger_server.models.slices_post import SlicesPost  # noqa: E501
 from fabric_cf.orchestrator.swagger_server.models.slivers import Slivers  # noqa: E501
 from fabric_cf.orchestrator.swagger_server.models.status200_ok_no_content import Status200OkNoContent  # noqa: E501
 from fabric_cf.orchestrator.swagger_server.response import slices_controller as rc
 
 
-def slices_create_post(body, name, lease_end_time=None):  # noqa: E501
+def slices_create_post(body, name, ssh_key, lease_end_time=None):  # noqa: E501
     """Create slice
 
     Request to create slice as described in the request. Request would be a graph ML describing the requested resources.
     Resources may be requested to be created now or in future. On success, one or more slivers are allocated, containing
     resources satisfying the request, and assigned to the given slice. This API returns list and description of the
     resources reserved for the slice in the form of Graph ML. Orchestrator would also trigger provisioning of these
-    resources asynchronously on the appropriate sites either now or in the future as requested. Experimenter can invoke
-    get slice API to get the latest state of the requested resources.   # noqa: E501
+    resources asynchronously on the appropriate sites either now or in the future as requested. Experimenter can
+    invoke get slice API to get the latest state of the requested resources.   # noqa: E501
+
+    :param body: 
+    :type body: dict | bytes
+    :param name: Slice Name
+    :type name: str
+    :param ssh_key: User SSH Key
+    :type ssh_key: str
+    :param lease_end_time: Lease End Time for the Slice
+    :type lease_end_time: str
+
+    :rtype: Slivers
+    """
+    post_body = SlicesPost()
+    post_body.graph_model = body.decode("utf-8")
+    post_body.ssh_keys = [ssh_key]
+    return rc.slices_create_post(post_body, name, lease_end_time)
+
+
+def slices_creates_post(body, name, lease_end_time=None):  # noqa: E501
+    """Create slice
+
+    Request to create slice as described in the request. Request would be a graph ML describing the requested resources.
+    Resources may be requested to be created now or in future. On success, one or more slivers are allocated,
+    containing resources satisfying the request, and assigned to the given slice. This API returns list and
+    description of the resources reserved for the slice in the form of Graph ML. Orchestrator would also trigger
+    provisioning of these resources asynchronously on the appropriate sites either now or in the future as requested.
+    Experimenter can invoke get slice API to get the latest state of the requested resources.   # noqa: E501
 
     :param body: Create new Slice
     :type body: dict | bytes
     :param name: Slice Name
     :type name: str
     :param lease_end_time: Lease End Time for the Slice
     :type lease_end_time: str
```

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/controllers/slivers_controller.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/controllers/slivers_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/encoder.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/encoder.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/__init__.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/base_model_.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/base_model_.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/poa.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/poa.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/poa_data.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/poa_data.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/poa_post.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/poa_post.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/poa_post_data.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/poa_post_data.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/poa_post_data_vcpu_cpu_map.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/poa_post_data_vcpu_cpu_map.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/resource.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/resource.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/resources.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/resources.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/slice.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/slice.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/slice_details.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/slice_details.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/slices.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/slices.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/slices_post.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/slices_post.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/sliver.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/sliver.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/slivers.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/slivers.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/status200_ok_no_content.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/status200_ok_no_content_data.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/status200_ok_paginated.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/status200_ok_paginated.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/status200_ok_single.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/status400_bad_request.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/status400_bad_request_errors.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/status401_unauthorized.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/status401_unauthorized_errors.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/status403_forbidden.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/status403_forbidden_errors.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/status404_not_found.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/status404_not_found_errors.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/status500_internal_server_error.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/status500_internal_server_error_errors.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/version.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/version.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/models/version_data.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/models/version_data.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/response/authorization_controller.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/response/authorization_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/response/constants.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/response/constants.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/response/cors_response.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/response/cors_response.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/response/poas_controller.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/response/poas_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/response/resources_controller.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/response/resources_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/response/slices_controller.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/response/slices_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/response/slivers_controller.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/response/slivers_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/response/utils.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/response/utils.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/response/version_controller.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/response/version_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/swagger/swagger.yaml` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/swagger/swagger.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -387,14 +387,97 @@
         description: Slice Name
         required: true
         style: form
         explode: true
         schema:
           minLength: 3
           type: string
+      - name: ssh_key
+        in: query
+        description: User SSH Key
+        required: true
+        style: form
+        explode: true
+        schema:
+          type: string
+      - name: lease_end_time
+        in: query
+        description: Lease End Time for the Slice
+        required: false
+        style: form
+        explode: true
+        schema:
+          type: string
+      requestBody:
+        $ref: '#/components/requestBodies/Request'
+      responses:
+        "200":
+          description: OK
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/slivers'
+        "400":
+          description: Bad Request
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/status_400_bad_request'
+        "401":
+          description: Unauthorized
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/status_401_unauthorized'
+        "403":
+          description: Forbidden
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/status_403_forbidden'
+        "404":
+          description: Not Found
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/status_404_not_found'
+        "500":
+          description: Internal Server Error
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/status_500_internal_server_error'
+      security:
+      - bearerAuth: []
+      x-openapi-router-controller: fabric_cf.orchestrator.swagger_server.controllers.slices_controller
+  /slices/creates:
+    post:
+      tags:
+      - slices
+      summary: Create slice
+      description: "Request to create slice as described in the request. Request would\
+        \ be a graph ML describing the requested resources. Resources may be requested\
+        \ to be created now or in future. On success, one or more slivers are allocated,\
+        \ containing resources satisfying the request, and assigned to the given slice.\
+        \ This API returns list and description of the resources reserved for the\
+        \ slice in the form of Graph ML. Orchestrator would also trigger provisioning\
+        \ of these resources asynchronously on the appropriate sites either now or\
+        \ in the future as requested. Experimenter can invoke get slice API to get\
+        \ the latest state of the requested resources. \n"
+      operationId: slices_creates_post
+      parameters:
+      - name: name
+        in: query
+        description: Slice Name
+        required: true
+        style: form
+        explode: true
+        schema:
+          minLength: 3
+          type: string
       - name: lease_end_time
         in: query
         description: Lease End Time for the Slice
         required: false
         style: form
         explode: true
         schema:
@@ -1467,14 +1550,20 @@
           items:
             $ref: '#/components/schemas/poa_post_data_vcpu_cpu_map'
         node_set:
           type: array
           items:
             type: string
   requestBodies:
+    Request:
+      content:
+        text/plain:
+          schema:
+            type: string
+      required: true
     payload_slices_modify:
       description: Modify a Slice
       content:
         text/plain:
           schema:
             type: string
       required: true
```

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/test/test_poas_controller.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/test/test_poas_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/test/test_resources_controller.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/test/test_resources_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/test/test_slices_controller.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/test/test_slices_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,21 +22,39 @@
     """SlicesController integration test stubs"""
 
     def test_slices_create_post(self):
         """Test case for slices_create_post
 
         Create slice
         """
-        body = SlicesPost()
+        body = 'body_example'
         query_string = [('name', 'name_example'),
+                        ('ssh_key', 'ssh_key_example'),
                         ('lease_end_time', 'lease_end_time_example')]
         response = self.client.open(
             '//slices/create',
             method='POST',
             data=json.dumps(body),
+            content_type='text/plain',
+            query_string=query_string)
+        self.assert200(response,
+                       'Response body is : ' + response.data.decode('utf-8'))
+
+    def test_slices_creates_post(self):
+        """Test case for slices_creates_post
+
+        Create slice
+        """
+        body = SlicesPost()
+        query_string = [('name', 'name_example'),
+                        ('lease_end_time', 'lease_end_time_example')]
+        response = self.client.open(
+            '//slices/creates',
+            method='POST',
+            data=json.dumps(body),
             content_type='application/json',
             query_string=query_string)
         self.assert200(response,
                        'Response body is : ' + response.data.decode('utf-8'))
 
     def test_slices_delete_delete(self):
         """Test case for slices_delete_delete
```

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/test/test_slivers_controller.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/test/test_slivers_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/test/test_version_controller.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/test/test_version_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/type_util.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/type_util.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/swagger_server/util.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/swagger_server/util.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/test/orchestrator.py` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/test/orchestrator.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/test/test.yaml` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/test/test.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/fabric_cf/orchestrator/update_swagger_stub.sh` & `fabric_cf-1.5.1rc0/fabric_cf/orchestrator/update_swagger_stub.sh`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/images/am-pod.png` & `fabric_cf-1.5.1rc0/images/am-pod.png`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/images/am.png` & `fabric_cf-1.5.1rc0/images/am.png`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/images/broker-pod.png` & `fabric_cf-1.5.1rc0/images/broker-pod.png`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/images/broker.png` & `fabric_cf-1.5.1rc0/images/broker.png`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/images/cf.png` & `fabric_cf-1.5.1rc0/images/cf.png`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/images/orchestrator-pod.png` & `fabric_cf-1.5.1rc0/images/orchestrator-pod.png`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/images/orchestrator.png` & `fabric_cf-1.5.1rc0/images/orchestrator.png`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/neo4j/AL2S.graphml` & `fabric_cf-1.5.1rc0/neo4j/AL2S.graphml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/neo4j/LBNL-ad.graphml` & `fabric_cf-1.5.1rc0/neo4j/LBNL-ad.graphml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/neo4j/Network-ad.graphml` & `fabric_cf-1.5.1rc0/neo4j/Network-ad.graphml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/neo4j/RENCI-ad.graphml` & `fabric_cf-1.5.1rc0/neo4j/RENCI-ad.graphml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/neo4j/UKY-ad.graphml` & `fabric_cf-1.5.1rc0/neo4j/UKY-ad.graphml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/neo4j/UKY2.graphml` & `fabric_cf-1.5.1rc0/neo4j/UKY2.graphml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/neo4j/abqm.graphml` & `fabric_cf-1.5.1rc0/neo4j/abqm.graphml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/neo4j/certs/fullchain.pem` & `fabric_cf-1.5.1rc0/neo4j/certs/fullchain.pem`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/neo4j/certs/privkey.pem` & `fabric_cf-1.5.1rc0/neo4j/certs/privkey.pem`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/psql.upgrade` & `fabric_cf-1.5.1rc0/psql.upgrade`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/pyproject.toml` & `fabric_cf-1.5.1rc0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     "psycopg2-binary",
     "sqlalchemy",
     "waitress",
     "prometheus_client",
     "connexion",
     "swagger-ui-bundle",
     "PyYAML",
-    "fabric_fss_utils==1.5.0rc1",
-    "fabric-message-bus==1.5.0b6",
-    "fabric-fim==1.5.0"]
+    "fabric_fss_utils==1.5.0",
+    "fabric-message-bus==1.5.0",
+    "fabric-fim==1.5.2"]
 
 [project.optional-dependencies]
 test = ["pytest",
         "flask_testing",
         "coverage>=4.0.3",
         "nose>=1.3.7",
         "pluggy>=0.3.1",
```

### Comparing `fabric_cf-1.5.0b5/secrets/create-certs.sh` & `fabric_cf-1.5.1rc0/secrets/create-certs.sh`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/tools/audit.py` & `fabric_cf-1.5.1rc0/tools/audit.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/tools/db_cli.py` & `fabric_cf-1.5.1rc0/tools/db_cli.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b5/PKG-INFO` & `fabric_cf-1.5.1rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric_cf
-Version: 1.5.0b5
+Version: 1.5.1rc0
 Summary: Fabric Control Framework
 Keywords: Swagger,Fabric Control Framework
 Author-email: Komal Thareja <kthare10@renci.org>, Ilya Baldin <ibaldin@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -14,17 +14,17 @@
 Requires-Dist: psycopg2-binary
 Requires-Dist: sqlalchemy
 Requires-Dist: waitress
 Requires-Dist: prometheus_client
 Requires-Dist: connexion
 Requires-Dist: swagger-ui-bundle
 Requires-Dist: PyYAML
-Requires-Dist: fabric_fss_utils==1.5.0rc1
-Requires-Dist: fabric-message-bus==1.5.0b6
-Requires-Dist: fabric-fim==1.5.0
+Requires-Dist: fabric_fss_utils==1.5.0
+Requires-Dist: fabric-message-bus==1.5.0
+Requires-Dist: fabric-fim==1.5.2
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: flask_testing ; extra == "test"
 Requires-Dist: coverage>=4.0.3 ; extra == "test"
 Requires-Dist: nose>=1.3.7 ; extra == "test"
 Requires-Dist: pluggy>=0.3.1 ; extra == "test"
 Requires-Dist: py>=1.4.31 ; extra == "test"
 Requires-Dist: randomize>=0.13 ; extra == "test"
```

