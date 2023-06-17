# Comparing `tmp/bittrade_huobi_websocket-0.3.5.tar.gz` & `tmp/bittrade_huobi_websocket-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bittrade_huobi_websocket-0.3.5.tar", max compression
+gzip compressed data, was "bittrade_huobi_websocket-0.3.6.tar", max compression
```

## Comparing `bittrade_huobi_websocket-0.3.5.tar` & `bittrade_huobi_websocket-0.3.6.tar`

### file list

```diff
@@ -1,78 +1,80 @@
--rw-r--r--   0        0        0     4517 2023-02-24 07:56:06.033242 bittrade_huobi_websocket-0.3.5/README.md
--rw-r--r--   0        0        0       23 2023-03-04 04:42:56.386093 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/__init__.py
--rw-r--r--   0        0        0      242 2023-04-11 02:30:39.951828 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/channels/__init__.py
--rw-r--r--   0        0        0     3054 2023-04-24 00:39:48.547550 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/channels/account_change.py
--rw-r--r--   0        0        0      123 2023-03-01 01:35:04.540753 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/channels/message.py
--rw-r--r--   0        0        0     1346 2023-03-04 09:18:11.423398 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/channels/open_orders.py
--rw-r--r--   0        0        0     1078 2023-02-24 08:03:57.919608 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/channels/orderbook.py
--rw-r--r--   0        0        0     2152 2023-03-01 01:35:04.540753 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/channels/subscribe.py
--rw-r--r--   0        0        0     1011 2023-04-10 19:43:51.859465 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/channels/trade.py
--rw-r--r--   0        0        0      430 2023-02-25 03:55:26.874992 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/connection/__init__.py
--rw-r--r--   0        0        0      954 2023-02-24 07:24:04.186610 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/connection/connection_operators.py
--rw-r--r--   0        0        0     4111 2023-02-27 08:09:14.102981 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/connection/generic.py
--rw-r--r--   0        0        0     2100 2023-04-24 01:37:44.729096 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/connection/http.py
--rw-r--r--   0        0        0      992 2023-02-25 07:03:33.346951 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/connection/private.py
--rw-r--r--   0        0        0      873 2023-02-25 06:59:58.870179 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/connection/public.py
--rw-r--r--   0        0        0     3556 2023-02-25 02:44:54.351056 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/connection/reconnect.py
--rw-r--r--   0        0        0     1762 2023-02-25 03:10:50.509972 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/connection/request_response.py
--rw-r--r--   0        0        0       65 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/events/__init__.py
--rw-r--r--   0        0        0      179 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/events/ids.py
--rw-r--r--   0        0        0       21 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/events/models/__init__.py
--rw-r--r--   0        0        0      152 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/events/models/order.py
--rw-r--r--   0        0        0      158 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/framework/__init__.py
--rw-r--r--   0        0        0     1307 2023-02-25 03:54:35.352674 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/framework/context_manager.py
--rw-r--r--   0        0        0     4635 2023-04-24 01:58:07.228765 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/framework/framework.py
--rw-r--r--   0        0        0     1153 2023-02-24 07:59:56.611168 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/framework/sign.py
--rw-r--r--   0        0        0        0 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/messages/__init__.py
--rw-r--r--   0        0        0        0 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/messages/filters/__init__.py
--rw-r--r--   0        0        0      586 2023-03-01 01:35:04.540753 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/messages/filters/kind.py
--rw-r--r--   0        0        0      197 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/messages/heartbeat.py
--rw-r--r--   0        0        0      709 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/messages/json.py
--rw-r--r--   0        0        0      240 2023-02-25 04:06:59.856936 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/messages/listen.py
--rw-r--r--   0        0        0      831 2023-03-04 07:50:43.218214 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/__init__.py
--rw-r--r--   0        0        0      303 2023-03-04 06:16:54.503353 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/book.py
--rw-r--r--   0        0        0      428 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/currency_networks.py
--rw-r--r--   0        0        0     1431 2023-04-24 01:19:55.645024 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/endpoints.py
--rw-r--r--   0        0        0      379 2023-03-01 01:35:04.540753 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/enhanced_websocket.py
--rw-r--r--   0        0        0     3007 2023-04-24 01:57:43.927837 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/framework.py
--rw-r--r--   0        0        0     2249 2023-04-24 02:14:05.599846 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/order.py
--rw-r--r--   0        0        0      426 2023-03-08 06:14:48.036979 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/request.py
--rw-r--r--   0        0        0      847 2023-02-27 08:47:00.172425 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/response_message.py
--rw-r--r--   0        0        0     1319 2023-03-04 09:29:47.688964 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/rest/__init__.py
--rw-r--r--   0        0        0     1594 2023-02-25 09:23:56.764266 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/rest/account_account_history.py
--rw-r--r--   0        0        0      199 2023-02-27 01:13:32.590437 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/rest/account_accounts.py
--rw-r--r--   0        0        0      724 2023-04-24 01:18:04.451364 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/rest/asset_transfer.py
--rw-r--r--   0        0        0      685 2023-02-27 01:13:32.590437 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/rest/cancel_order.py
--rw-r--r--   0        0        0      721 2023-02-27 01:16:44.366830 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/rest/cancel_orders_batch.py
--rw-r--r--   0        0        0     1151 2023-05-25 00:02:23.689738 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/rest/create_order.py
--rw-r--r--   0        0        0      287 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/rest/create_withdrawal.py
--rw-r--r--   0        0        0      214 2023-03-08 05:33:04.915323 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/rest/get_account_balance.py
--rw-r--r--   0        0        0     1033 2023-02-27 01:13:32.590437 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/rest/get_all_open_orders.py
--rw-r--r--   0        0        0      652 2023-03-04 06:16:27.482221 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/rest/market_depth.py
--rw-r--r--   0        0        0      400 2023-03-04 09:29:50.858964 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/rest/order_details.py
--rw-r--r--   0        0        0      171 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/trade.py
--rw-r--r--   0        0        0     1428 2023-04-11 07:58:23.790213 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/user_balance.py
--rw-r--r--   0        0        0      213 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/withdrawal.py
--rw-r--r--   0        0        0       16 2023-02-25 04:07:25.277920 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/operators/__init__.py
--rw-r--r--   0        0        0      740 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/operators/orderbook/__init__.py
--rw-r--r--   0        0        0     1059 2023-03-08 09:46:54.414602 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/operators/stream/response_messages.py
--rw-r--r--   0        0        0      119 2023-02-25 03:53:49.531897 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/rest/__init__.py
--rw-r--r--   0        0        0      877 2023-02-25 08:44:55.803604 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/rest/account_account_history.py
--rw-r--r--   0        0        0      767 2023-02-27 01:13:32.590437 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/rest/account_accounts.py
--rw-r--r--   0        0        0      682 2023-04-24 01:20:13.815024 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/rest/asset_transfer.py
--rw-r--r--   0        0        0     1045 2023-02-27 01:13:32.590437 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/rest/cancel_order.py
--rw-r--r--   0        0        0     1227 2023-02-27 06:51:17.226045 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/rest/cancel_orders_batch.py
--rw-r--r--   0        0        0     2661 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/rest/close_position.py
--rw-r--r--   0        0        0      687 2023-02-27 01:13:32.590437 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/rest/create_order.py
--rw-r--r--   0        0        0     3683 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/rest/create_order_list.py
--rw-r--r--   0        0        0      813 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/rest/create_withdrawal.py
--rw-r--r--   0        0        0     1229 2023-03-08 06:18:19.564301 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/rest/get_account_balance.py
--rw-r--r--   0        0        0     1877 2023-03-22 07:22:53.744353 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/rest/get_all_open_orders.py
--rw-r--r--   0        0        0     1610 2023-04-24 00:39:48.557550 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/rest/get_book.py
--rw-r--r--   0        0        0      513 2023-04-24 01:20:07.645024 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/rest/get_uid.py
--rw-r--r--   0        0        0      842 2023-03-08 06:15:17.067967 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/rest/http_factory_decorator.py
--rw-r--r--   0        0        0      377 2023-03-04 09:26:18.240876 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/rest/order_details.py
--rw-r--r--   0        0        0      163 2023-02-25 03:53:20.251161 bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/rest/user_balance.py
--rw-r--r--   0        0        0     1756 2023-05-25 00:02:57.450676 bittrade_huobi_websocket-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     6097 1970-01-01 00:00:00.000000 bittrade_huobi_websocket-0.3.5/setup.py
--rw-r--r--   0        0        0     5727 1970-01-01 00:00:00.000000 bittrade_huobi_websocket-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     4517 2023-02-24 07:56:06.033242 bittrade_huobi_websocket-0.3.6/README.md
+-rw-r--r--   0        0        0       23 2023-03-04 04:42:56.386093 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/__init__.py
+-rw-r--r--   0        0        0      242 2023-04-11 02:30:39.951828 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/channels/__init__.py
+-rw-r--r--   0        0        0     3054 2023-04-24 00:39:48.547550 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/channels/account_change.py
+-rw-r--r--   0        0        0      123 2023-03-01 01:35:04.540753 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/channels/message.py
+-rw-r--r--   0        0        0     1346 2023-03-04 09:18:11.423398 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/channels/open_orders.py
+-rw-r--r--   0        0        0     1078 2023-02-24 08:03:57.919608 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/channels/orderbook.py
+-rw-r--r--   0        0        0     2152 2023-03-01 01:35:04.540753 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/channels/subscribe.py
+-rw-r--r--   0        0        0     1011 2023-04-10 19:43:51.859465 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/channels/trade.py
+-rw-r--r--   0        0        0      430 2023-02-25 03:55:26.874992 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/connection/__init__.py
+-rw-r--r--   0        0        0      954 2023-02-24 07:24:04.186610 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/connection/connection_operators.py
+-rw-r--r--   0        0        0     4111 2023-02-27 08:09:14.102981 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/connection/generic.py
+-rw-r--r--   0        0        0     2100 2023-04-24 01:37:44.729096 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/connection/http.py
+-rw-r--r--   0        0        0      992 2023-02-25 07:03:33.346951 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/connection/private.py
+-rw-r--r--   0        0        0      873 2023-02-25 06:59:58.870179 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/connection/public.py
+-rw-r--r--   0        0        0     3556 2023-02-25 02:44:54.351056 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/connection/reconnect.py
+-rw-r--r--   0        0        0     1762 2023-02-25 03:10:50.509972 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/connection/request_response.py
+-rw-r--r--   0        0        0       65 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/events/__init__.py
+-rw-r--r--   0        0        0      179 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/events/ids.py
+-rw-r--r--   0        0        0       21 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/events/models/__init__.py
+-rw-r--r--   0        0        0      152 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/events/models/order.py
+-rw-r--r--   0        0        0      158 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/framework/__init__.py
+-rw-r--r--   0        0        0     1307 2023-02-25 03:54:35.352674 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/framework/context_manager.py
+-rw-r--r--   0        0        0     4830 2023-06-17 03:20:20.835124 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/framework/framework.py
+-rw-r--r--   0        0        0     1153 2023-02-24 07:59:56.611168 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/framework/sign.py
+-rw-r--r--   0        0        0        0 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/messages/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/messages/filters/__init__.py
+-rw-r--r--   0        0        0      586 2023-03-01 01:35:04.540753 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/messages/filters/kind.py
+-rw-r--r--   0        0        0      197 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/messages/heartbeat.py
+-rw-r--r--   0        0        0      709 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/messages/json.py
+-rw-r--r--   0        0        0      240 2023-02-25 04:06:59.856936 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/messages/listen.py
+-rw-r--r--   0        0        0      831 2023-03-04 07:50:43.218214 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/__init__.py
+-rw-r--r--   0        0        0      303 2023-03-04 06:16:54.503353 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/book.py
+-rw-r--r--   0        0        0      428 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/currency_networks.py
+-rw-r--r--   0        0        0     1495 2023-06-17 03:15:06.694595 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/endpoints.py
+-rw-r--r--   0        0        0      379 2023-03-01 01:35:04.540753 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/enhanced_websocket.py
+-rw-r--r--   0        0        0     3277 2023-06-17 03:20:02.834113 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/framework.py
+-rw-r--r--   0        0        0     2249 2023-04-24 02:14:05.599846 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/order.py
+-rw-r--r--   0        0        0      426 2023-03-08 06:14:48.036979 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/request.py
+-rw-r--r--   0        0        0      847 2023-02-27 08:47:00.172425 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/response_message.py
+-rw-r--r--   0        0        0     1319 2023-03-04 09:29:47.688964 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/rest/__init__.py
+-rw-r--r--   0        0        0     1594 2023-02-25 09:23:56.764266 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/rest/account_account_history.py
+-rw-r--r--   0        0        0      199 2023-02-27 01:13:32.590437 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/rest/account_accounts.py
+-rw-r--r--   0        0        0      724 2023-04-24 01:18:04.451364 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/rest/asset_transfer.py
+-rw-r--r--   0        0        0      685 2023-02-27 01:13:32.590437 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/rest/cancel_order.py
+-rw-r--r--   0        0        0      721 2023-02-27 01:16:44.366830 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/rest/cancel_orders_batch.py
+-rw-r--r--   0        0        0     1151 2023-05-25 00:02:23.689738 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/rest/create_order.py
+-rw-r--r--   0        0        0      287 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/rest/create_withdrawal.py
+-rw-r--r--   0        0        0      214 2023-03-08 05:33:04.915323 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/rest/get_account_balance.py
+-rw-r--r--   0        0        0     1033 2023-02-27 01:13:32.590437 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/rest/get_all_open_orders.py
+-rw-r--r--   0        0        0      249 2023-06-17 03:18:45.392109 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/rest/get_current_fee_rate.py
+-rw-r--r--   0        0        0      652 2023-03-04 06:16:27.482221 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/rest/market_depth.py
+-rw-r--r--   0        0        0      400 2023-03-04 09:29:50.858964 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/rest/order_details.py
+-rw-r--r--   0        0        0      171 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/trade.py
+-rw-r--r--   0        0        0     1428 2023-04-11 07:58:23.790213 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/user_balance.py
+-rw-r--r--   0        0        0      213 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/withdrawal.py
+-rw-r--r--   0        0        0       16 2023-02-25 04:07:25.277920 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/operators/__init__.py
+-rw-r--r--   0        0        0      740 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/operators/orderbook/__init__.py
+-rw-r--r--   0        0        0     1059 2023-03-08 09:46:54.414602 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/operators/stream/response_messages.py
+-rw-r--r--   0        0        0      119 2023-02-25 03:53:49.531897 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/rest/__init__.py
+-rw-r--r--   0        0        0      877 2023-02-25 08:44:55.803604 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/rest/account_account_history.py
+-rw-r--r--   0        0        0      767 2023-02-27 01:13:32.590437 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/rest/account_accounts.py
+-rw-r--r--   0        0        0      682 2023-04-24 01:20:13.815024 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/rest/asset_transfer.py
+-rw-r--r--   0        0        0     1045 2023-02-27 01:13:32.590437 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/rest/cancel_order.py
+-rw-r--r--   0        0        0     1227 2023-02-27 06:51:17.226045 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/rest/cancel_orders_batch.py
+-rw-r--r--   0        0        0     2661 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/rest/close_position.py
+-rw-r--r--   0        0        0      687 2023-02-27 01:13:32.590437 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/rest/create_order.py
+-rw-r--r--   0        0        0     3683 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/rest/create_order_list.py
+-rw-r--r--   0        0        0      813 2023-02-24 07:24:04.196610 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/rest/create_withdrawal.py
+-rw-r--r--   0        0        0     1229 2023-03-08 06:18:19.564301 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/rest/get_account_balance.py
+-rw-r--r--   0        0        0     1877 2023-03-22 07:22:53.744353 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/rest/get_all_open_orders.py
+-rw-r--r--   0        0        0     1610 2023-04-24 00:39:48.557550 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/rest/get_book.py
+-rw-r--r--   0        0        0      484 2023-06-17 03:24:23.958340 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/rest/get_current_fee_rate.py
+-rw-r--r--   0        0        0      513 2023-04-24 01:20:07.645024 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/rest/get_uid.py
+-rw-r--r--   0        0        0      842 2023-03-08 06:15:17.067967 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/rest/http_factory_decorator.py
+-rw-r--r--   0        0        0      377 2023-03-04 09:26:18.240876 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/rest/order_details.py
+-rw-r--r--   0        0        0      163 2023-02-25 03:53:20.251161 bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/rest/user_balance.py
+-rw-r--r--   0        0        0     1757 2023-06-17 03:35:20.050777 bittrade_huobi_websocket-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     6097 1970-01-01 00:00:00.000000 bittrade_huobi_websocket-0.3.6/setup.py
+-rw-r--r--   0        0        0     5727 1970-01-01 00:00:00.000000 bittrade_huobi_websocket-0.3.6/PKG-INFO
```

### Comparing `bittrade_huobi_websocket-0.3.5/README.md` & `bittrade_huobi_websocket-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/channels/account_change.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/channels/account_change.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/channels/open_orders.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/channels/open_orders.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/channels/orderbook.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/channels/orderbook.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/channels/subscribe.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/channels/subscribe.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/channels/trade.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/channels/trade.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/connection/connection_operators.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/connection/connection_operators.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/connection/generic.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/connection/generic.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/connection/http.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/connection/http.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/connection/private.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/connection/private.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/connection/public.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/connection/public.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/connection/reconnect.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/connection/reconnect.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/connection/request_response.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/connection/request_response.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/framework/context_manager.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/framework/context_manager.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/framework/framework.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/framework/framework.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 )
 from bittrade_huobi_websocket.rest.account_accounts import (
     get_account_accounts_http_factory,
 )
 from bittrade_huobi_websocket.rest.asset_transfer import asset_transfer_http_factory
 from bittrade_huobi_websocket.rest.cancel_order import cancel_order_http_factory
 from bittrade_huobi_websocket.rest.create_order import create_order_http_factory
+from bittrade_huobi_websocket.rest.get_current_fee_rate import (
+    get_current_fee_rate_http_factory,
+)
 from bittrade_huobi_websocket.rest.get_uid import get_uid_http_factory
 from bittrade_huobi_websocket.rest.order_details import order_details_http_factory
 from bittrade_huobi_websocket.rest.get_account_balance import (
     get_account_balance_http_factory,
 )
 from bittrade_huobi_websocket.rest.get_book import get_book_http
 from bittrade_huobi_websocket.rest.cancel_orders_batch import (
@@ -97,14 +100,15 @@
         cancel_all_http=cancel_orders_batch_http_factory(add_token_http),
         cancel_order_http=cancel_order_http_factory(add_token_http),
         create_order_http=create_order_http_factory(add_token_http),
         get_book_http=get_book_http,
         get_uid_http=get_uid_http_factory(add_token_http),
         get_account_balance_http=get_account_balance_http_factory(add_token_http),
         get_accounts_http=get_account_accounts_http_factory(add_token_http),
+        get_current_fee_rate_http=get_current_fee_rate_http_factory(add_token_http),
         exchange=exchange,
         load_all_open_orders=functools.partial(
             load_all_open_orders, get_all_open_orders_http
         ),
         open_orders_http=get_all_open_orders_http,
         order_details_http=order_details_http_factory(add_token_http),
         public_socket_connection=public_sockets,
```

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/framework/sign.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/framework/sign.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/messages/filters/kind.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/messages/filters/kind.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/messages/json.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/messages/json.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/__init__.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/endpoints.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/endpoints.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     MARKET_TRADE = "/market/trade"
     ORDER_HISTORY = "/v1/api/order_history"
     ORDER_INFO = "/v1/api/order_info"
     TICKER_DETAIL = "/v1/market/detail"
 
     # v2 endpoints
     V2_ACCOUNT_BALANCE = "/v2/account/balance"
+    V2_GET_CURRENT_FEE_RATE = "/v2/reference/transact-fee-rate"
     V2_GET_UID = "/v2/user/uid"
     V2_ORDER_CREATE = "/v2/order/orders/place"
     V2_ORDER_CANCEL = "/v2/order/orders/{order_id}/submitcancel"
     V2_ORDER_DETAILS = "/v2/order/orders/{order_id}"
     V2_ORDER_MATCH_RESULTS = "/v2/order/matchresults"
     V2_ORDER_HISTORY = "/v2/order/history"
     V2_WITHDRAW_CREATE = "/v2/account/withdraw"
```

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/framework.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/framework.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,16 +23,20 @@
     CancelOrdersBatchParams,
 )
 from bittrade_huobi_websocket.models.rest.create_order import (
     OrderCreateParams,
     OrderCreateResponse,
 )
 from bittrade_huobi_websocket.models.rest.cancel_order import CancelOrderParams
+from bittrade_huobi_websocket.models.rest.get_current_fee_rate import FeeRateResponse
 from bittrade_huobi_websocket.models.user_balance import AccountUpdateData
 from bittrade_huobi_websocket.rest import asset_transfer
+from bittrade_huobi_websocket.rest.get_current_fee_rate import (
+    get_current_fee_rate_http_factory,
+)
 
 
 class BookConfig(NamedTuple):
     pair: str
     depth: int
 
 
@@ -50,14 +54,15 @@
     create_order_http: Callable[
         [OrderCreateParams],
         Observable[OrderCreateResponse],
     ]
     get_book_http: Callable[[market_depth.MarketDepthParams], Observable[HttpResponse]]
     get_account_balance_http: Callable[[str], Observable[HttpResponse]]
     get_accounts_http: Callable[[], Observable[HttpResponse]]
+    get_current_fee_rate_http: Callable[[], Observable[FeeRateResponse]]
     get_uid_http: Callable[[], Observable[HttpResponse]]
     exchange: huobi
     load_all_open_orders: Callable[
         [get_all_open_orders.AllOpenOrdersParams],
         Observable[list[get_all_open_orders.AllOpenOrder]],
     ]
     public_socket_connection: ConnectableObservable[models.WebsocketBundle]
```

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/order.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/order.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/response_message.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/response_message.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/rest/__init__.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/rest/account_account_history.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/rest/account_account_history.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/rest/asset_transfer.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/rest/asset_transfer.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/rest/cancel_order.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/rest/cancel_order.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/rest/cancel_orders_batch.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/rest/cancel_orders_batch.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/rest/create_order.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/rest/create_order.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/rest/get_all_open_orders.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/rest/get_all_open_orders.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/rest/market_depth.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/rest/market_depth.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/models/user_balance.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/models/user_balance.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/operators/orderbook/__init__.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/operators/orderbook/__init__.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/operators/stream/response_messages.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/operators/stream/response_messages.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/rest/account_account_history.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/rest/account_account_history.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/rest/account_accounts.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/rest/account_accounts.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/rest/asset_transfer.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/rest/asset_transfer.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/rest/cancel_order.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/rest/cancel_order.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/rest/cancel_orders_batch.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/rest/cancel_orders_batch.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/rest/close_position.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/rest/close_position.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/rest/create_order.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/rest/create_order.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/rest/create_order_list.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/rest/create_order_list.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/rest/create_withdrawal.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/rest/create_withdrawal.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/rest/get_account_balance.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/rest/get_account_balance.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/rest/get_all_open_orders.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/rest/get_all_open_orders.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/rest/get_book.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/rest/get_book.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/rest/get_uid.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/rest/get_uid.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/bittrade_huobi_websocket/rest/http_factory_decorator.py` & `bittrade_huobi_websocket-0.3.6/bittrade_huobi_websocket/rest/http_factory_decorator.py`

 * *Files identical despite different names*

### Comparing `bittrade_huobi_websocket-0.3.5/pyproject.toml` & `bittrade_huobi_websocket-0.3.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bittrade-huobi-websocket"
-version = "0.3.5"
+version = "0.3.6"
 description = "Reactive Websocket for Huboi"
 authors = ["mat <matt@techspace.asia>"]
 readme = "README.md"
 repository = "https://github.com/TechSpaceAsia/bittrade-huobi-websocket"
 homepage = "https://github.com/TechSpaceAsia/bittrade-huobi-websocket"
 license = "MIT"
 classifiers = [
@@ -50,14 +50,15 @@
 
 
 
 
 
 
 
+
 
 
 
 
 
 [tool.poetry.group.rich.dependencies]
 fire = "^0.5.0"
```

### Comparing `bittrade_huobi_websocket-0.3.5/setup.py` & `bittrade_huobi_websocket-0.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
  'requests>=2.28.2,<3.0.0',
  'returns>=0.19.0,<0.20.0',
  'websocket-client>=1.4.2,<2.0.0',
  'websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'bittrade-huobi-websocket',
-    'version': '0.3.5',
+    'version': '0.3.6',
     'description': 'Reactive Websocket for Huboi',
     'long_description': '# Crypto.com Websocket\n\n[NOT RELEASED] This is very much a work in progress, despite being on pypi.\nMost things might be wrongly documented; API **will** change\n\n## Features\n\n- Reconnect with incremental backoff \n- Respond to ping\n- request/response factories e.g. `add_order_factory` make websocket events feel like calling an API\n- ... but provides more info than a simple request/response; \n  for instance, `add_order` goes through each stage submitted->pending->open or canceled, \n  emitting a notification at each stage\n\n## Installing\n\n`pip install bittrade-cryptodotcom-websocket` or `poetry add bittrade-cryptodotcom-websocket`\n\n## General considerations\n\n### Observables/Reactivex\n\nThe whole library is build with [Reactivex](https://rxpy.readthedocs.io/en/latest/).\n\nThough Observables seem complicated at first, they are the best way to handle - and (synchronously) test - complex situations that arise over time, like an invalid sequence of messages or socket disconnection and backoff reconnects.\n\nFor simple use cases, they are also rather easy to use as shown in the [examples](./examples) folder or in the Getting Started below\n\n### Concurrency\n\nInternally the library uses threads.\nFor your main program you don\'t have to worry about threads; you can block the main thread.\n\n## Getting started\n\n### Connect to the public feeds\n\n```python\nfrom bittrade_huobi_websocket import public_websocket_connection, subscribe_ticker\nfrom bittrade_huobi_websocket.operators import keep_messages_only, filter_new_socket_only\n\n# Prepare connection - note, this is a ConnectableObservable, so it will only trigger connection when we call its ``connect`` method\nsocket_connection = public_websocket_connection()\n# Prepare a feed with only "real" messages, dropping things like status update, heartbeat, etc…\nmessages = socket_connection.pipe(\n    keep_messages_only(),\n)\nsocket_connection.pipe(\n    filter_new_socket_only(),\n    subscribe_ticker(\'USDT/USD\', messages)\n).subscribe(\n    print, print, print  # you can do anything with the messages; here we simply print them out\n)\nsocket_connection.connect()\n```\n\n_(This script is complete, it should run "as is")_\n\n\n## Logging\n\nWe use Python\'s standard logging.\nYou can modify what logs you see as follows:\n\n```\nlogging.getLogger(\'bittrade_huobi_websocket\').addHandler(logging.StreamHandler())\n```\n\nIn addition, two special logger logs every message sent/received from the socket (except heartbeat) at the `DEBUG` level: `bittrade_huobi_websocket.raw_socket.sent` and `bittrade_huobi_websocket.raw_socket.received`\n\nTo view a full, timestamped history of the socket exchanges use\n\n```\nhandler = FileHandler("logs/raw_socket.log")\nhandler.setLevel(DEBUG)\nlogger = logging.getLogger("bittrade_huobi_websocket.raw_socket.sent")\nformatter = logging.Formatter("%(asctime)s.%(msecs)03d <== %(message)s", datefmt="%H:%M:%S")\nhandler.setFormatter(formatter)\nlogger.addHandler(handler)\nhandler = FileHandler("logs/raw_socket.log")\nhandler.setLevel(DEBUG)\nlogger = logging.getLogger("bittrade_huobi_websocket.raw_socket.received")\nformatter = logging.Formatter("%(asctime)s.%(msecs)03d --> %(message)s", datefmt="%H:%M:%S")\nhandler.setFormatter(formatter)\nlogger.addHandler(handler)\n```\n\n## Private feeds\n\nSimilar to [bittrade-kraken-rest](https://github.com/TechSpaceAsia/bittrade-kraken-rest), this library attempts to get as little access to sensitive information as possible.\n\nThis means that you\'ll need to implement the signature token yourself. The library never has access to your API secret.\n\nSee `examples/private_subscription.py` for an example of implementation but it is generally as simple as:\n\n```python\nauthenticated_sockets = connection.pipe(\n    filter_new_socket_only(),\n    operators.map(add_token),\n    operators.share(),\n)\n```\n\n# Development guidelines\n\n## `*_http` methods\n\nREST functions over http should be suffixed with `_http` e.g. `get_book_http`.\nThey should return an Observable containing the *full* json body; this is easily achieved via `prepare_request` and `send_request`.\n\nWhere possible models should be defined to describe the *raw* result and *parsed result* if available/useful.\n\nReactive operators may be provided for parsing, but they should never be included in the *raw* functionality of the `*_http` function, only optional.\n\nAny operator that maps to CCXT types should be suffixed with `_ccxt` e.g. `parse_book_ccxt`.',
     'author': 'mat',
     'author_email': 'matt@techspace.asia',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/TechSpaceAsia/bittrade-huobi-websocket',
```

### Comparing `bittrade_huobi_websocket-0.3.5/PKG-INFO` & `bittrade_huobi_websocket-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bittrade-huobi-websocket
-Version: 0.3.5
+Version: 0.3.6
 Summary: Reactive Websocket for Huboi
 Home-page: https://github.com/TechSpaceAsia/bittrade-huobi-websocket
 License: MIT
 Author: mat
 Author-email: matt@techspace.asia
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
```

