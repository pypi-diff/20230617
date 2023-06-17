# Comparing `tmp/hrin_msb-0.2.81.tar.gz` & `tmp/hrin_msb-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hrin_msb-0.2.81.tar", max compression
+gzip compressed data, was "hrin_msb-0.2.9.tar", max compression
```

## Comparing `hrin_msb-0.2.81.tar` & `hrin_msb-0.2.9.tar`

### file list

```diff
@@ -1,108 +1,104 @@
--rw-r--r--   0        0        0     1486 2023-05-31 20:49:08.557401 hrin_msb-0.2.81/hrin_msb.py
--rw-r--r--   0        0        0     1092 2022-11-10 09:38:13.921857 hrin_msb-0.2.81/LICENSE
--rw-r--r--   0        0        0        0 2023-05-12 14:16:03.936144 hrin_msb-0.2.81/msb/__init__.py
--rw-r--r--   0        0        0      173 2023-05-16 07:20:35.977782 hrin_msb-0.2.81/msb/apis/__init__.py
--rw-r--r--   0        0        0     2810 2023-06-03 12:27:27.338404 hrin_msb-0.2.81/msb/apis/api_view.py
--rw-r--r--   0        0        0     5112 2023-06-13 10:03:26.212428 hrin_msb-0.2.81/msb/apis/api_viewset.py
--rw-r--r--   0        0        0      945 2023-05-12 14:13:45.851874 hrin_msb-0.2.81/msb/apis/constants.py
--rw-r--r--   0        0        0      995 2023-05-12 14:13:45.852970 hrin_msb-0.2.81/msb/apis/errors.py
--rw-r--r--   0        0        0      576 2023-05-12 14:20:43.764046 hrin_msb-0.2.81/msb/apis/exceptions.py
--rw-r--r--   0        0        0     3005 2023-06-10 20:14:52.906312 hrin_msb-0.2.81/msb/apis/funcs.py
--rw-r--r--   0        0        0      234 2023-05-16 08:48:53.311194 hrin_msb-0.2.81/msb/auth/__init__.py
--rw-r--r--   0        0        0      769 2023-05-12 14:06:51.061452 hrin_msb-0.2.81/msb/auth/authenticators.py
--rw-r--r--   0        0        0     3061 2023-06-13 08:39:24.048824 hrin_msb-0.2.81/msb/auth/constants.py
--rw-r--r--   0        0        0     1317 2023-05-16 16:57:04.977122 hrin_msb-0.2.81/msb/auth/decorators.py
--rw-r--r--   0        0        0     2801 2023-05-12 14:06:51.071513 hrin_msb-0.2.81/msb/auth/defaults.py
--rw-r--r--   0        0        0      989 2023-06-13 08:39:24.050145 hrin_msb-0.2.81/msb/auth/exceptions.py
--rw-r--r--   0        0        0     4682 2023-06-15 04:56:16.718830 hrin_msb-0.2.81/msb/auth/permissions.py
--rw-r--r--   0        0        0     1188 2023-05-12 14:06:51.079054 hrin_msb-0.2.81/msb/auth/results.py
--rw-r--r--   0        0        0     2860 2023-05-12 14:20:43.803305 hrin_msb-0.2.81/msb/auth/serializers.py
--rw-r--r--   0        0        0     3510 2023-05-17 05:39:38.891297 hrin_msb-0.2.81/msb/auth/session.py
--rw-r--r--   0        0        0     1791 2023-05-12 14:20:43.992065 hrin_msb-0.2.81/msb/auth/token.py
--rw-r--r--   0        0        0     2143 2023-06-13 08:39:24.051152 hrin_msb-0.2.81/msb/auth/users.py
--rw-r--r--   0        0        0     2417 2023-05-12 14:20:44.239821 hrin_msb-0.2.81/msb/auth/validators.py
--rw-r--r--   0        0        0       28 2023-05-12 14:06:51.097760 hrin_msb-0.2.81/msb/cipher/__init__.py
--rw-r--r--   0        0        0       34 2023-05-12 14:06:51.101177 hrin_msb-0.2.81/msb/cipher/asymmetric_cipher.py
--rw-r--r--   0        0        0     1720 2023-06-14 05:57:15.439365 hrin_msb-0.2.81/msb/cipher/cipher.py
--rw-r--r--   0        0        0        0 2023-05-12 14:06:51.105803 hrin_msb-0.2.81/msb/cipher/constants.py
--rw-r--r--   0        0        0      160 2023-05-12 14:20:44.164359 hrin_msb-0.2.81/msb/cipher/exceptions.py
--rw-r--r--   0        0        0      714 2023-05-12 14:06:51.110798 hrin_msb-0.2.81/msb/cipher/symmetric_cipher.py
--rw-r--r--   0        0        0      295 2023-06-02 20:58:49.315841 hrin_msb-0.2.81/msb/dataclasses/__init__.py
--rw-r--r--   0        0        0     1760 2023-06-02 19:42:50.982112 hrin_msb-0.2.81/msb/dataclasses/_email.py
--rw-r--r--   0        0        0      928 2023-05-12 14:06:51.146614 hrin_msb-0.2.81/msb/dataclasses/_singleton.py
--rw-r--r--   0        0        0      759 2023-05-15 03:37:05.173290 hrin_msb-0.2.81/msb/dataclasses/_wrappers.py
--rw-r--r--   0        0        0     1840 2023-06-13 08:41:25.981898 hrin_msb-0.2.81/msb/dataclasses/notification.py
--rw-r--r--   0        0        0     4546 2023-06-15 04:56:16.719835 hrin_msb-0.2.81/msb/dataclasses/search_parameter.py
--rw-r--r--   0        0        0      354 2023-05-12 14:06:51.155774 hrin_msb-0.2.81/msb/datetime/__init__.py
--rw-r--r--   0        0        0      370 2023-05-12 14:06:51.157773 hrin_msb-0.2.81/msb/datetime/constants.py
--rw-r--r--   0        0        0     2419 2023-05-12 14:06:51.162421 hrin_msb-0.2.81/msb/datetime/wrappers.py
--rw-r--r--   0        0        0      107 2023-05-12 14:06:51.165268 hrin_msb-0.2.81/msb/db/__init__.py
--rw-r--r--   0        0        0     1231 2023-05-12 14:06:51.167268 hrin_msb-0.2.81/msb/db/config_model.py
--rw-r--r--   0        0        0      672 2023-05-12 14:06:51.170760 hrin_msb-0.2.81/msb/db/constants.py
--rw-r--r--   0        0        0     2558 2023-05-12 14:20:43.606453 hrin_msb-0.2.81/msb/db/logging_models.py
--rw-r--r--   0        0        0      767 2023-05-29 11:46:57.420750 hrin_msb-0.2.81/msb/db/metafields.py
--rw-r--r--   0        0        0     1294 2023-05-17 06:49:20.059584 hrin_msb-0.2.81/msb/db/model_fields.py
--rw-r--r--   0        0        0      506 2023-05-12 14:06:51.179818 hrin_msb-0.2.81/msb/db/models.py
--rw-r--r--   0        0        0     5219 2023-06-16 14:20:13.866342 hrin_msb-0.2.81/msb/db/msb_model.py
--rw-r--r--   0        0        0     1127 2023-06-13 10:03:26.229400 hrin_msb-0.2.81/msb/db/msb_model_manager.py
--rw-r--r--   0        0        0     3747 2023-05-12 14:06:51.186333 hrin_msb-0.2.81/msb/db/routers.py
--rw-r--r--   0        0        0      198 2023-05-31 18:36:21.245373 hrin_msb-0.2.81/msb/devtools/__init__.py
--rw-r--r--   0        0        0      752 2023-05-12 14:06:51.191331 hrin_msb-0.2.81/msb/devtools/constants.py
--rw-r--r--   0        0        0     1928 2023-05-29 14:43:55.586902 hrin_msb-0.2.81/msb/devtools/dataclasses.py
--rw-r--r--   0        0        0     3426 2023-06-16 21:16:22.116725 hrin_msb-0.2.81/msb/devtools/django.py
--rw-r--r--   0        0        0     2256 2023-05-31 18:35:40.294116 hrin_msb-0.2.81/msb/devtools/funcs.py
--rw-r--r--   0        0        0     4392 2023-06-16 21:16:22.110725 hrin_msb-0.2.81/msb/devtools/tasks.py
--rw-r--r--   0        0        0       54 2023-05-12 14:06:51.203450 hrin_msb-0.2.81/msb/env/__init__.py
--rw-r--r--   0        0        0     2764 2023-05-12 14:06:51.204447 hrin_msb-0.2.81/msb/env/config.py
--rw-r--r--   0        0        0     6232 2023-06-13 10:22:58.123081 hrin_msb-0.2.81/msb/env/constants.py
--rw-r--r--   0        0        0     1444 2023-05-12 14:06:51.210143 hrin_msb-0.2.81/msb/env/core.py
--rw-r--r--   0        0        0      382 2023-05-12 14:20:43.895202 hrin_msb-0.2.81/msb/env/exceptions.py
--rw-r--r--   0        0        0     8215 2023-06-17 06:12:09.443365 hrin_msb-0.2.81/msb/env/settings.py
--rw-r--r--   0        0        0      117 2023-05-14 14:48:41.231493 hrin_msb-0.2.81/msb/exceptions/__init__.py
--rw-r--r--   0        0        0     1271 2023-05-12 14:06:51.223030 hrin_msb-0.2.81/msb/exceptions/_exception.py
--rw-r--r--   0        0        0      488 2023-06-05 17:52:51.927226 hrin_msb-0.2.81/msb/exceptions/handlers.py
--rw-r--r--   0        0        0      132 2023-05-12 14:06:51.229616 hrin_msb-0.2.81/msb/files/__init__.py
--rw-r--r--   0        0        0      951 2023-05-12 14:06:51.232121 hrin_msb-0.2.81/msb/files/core.py
--rw-r--r--   0        0        0     1052 2023-05-12 14:06:51.233508 hrin_msb-0.2.81/msb/files/csv.py
--rw-r--r--   0        0        0      181 2023-05-12 14:06:51.236030 hrin_msb-0.2.81/msb/files/dataclasses.py
--rw-r--r--   0        0        0     1397 2023-05-12 14:06:51.239032 hrin_msb-0.2.81/msb/files/docx.py
--rw-r--r--   0        0        0      604 2023-05-12 14:20:44.215958 hrin_msb-0.2.81/msb/files/exceptions.py
--rw-r--r--   0        0        0      329 2023-05-12 14:06:51.244037 hrin_msb-0.2.81/msb/files/factory.py
--rw-r--r--   0        0        0      198 2023-05-12 14:06:51.246557 hrin_msb-0.2.81/msb/files/messages.py
--rw-r--r--   0        0        0     1064 2023-05-12 14:06:51.248559 hrin_msb-0.2.81/msb/files/pdf.py
--rw-r--r--   0        0        0      515 2023-05-12 14:06:51.250559 hrin_msb-0.2.81/msb/http/__init__.py
--rw-r--r--   0        0        0     6420 2023-06-05 17:55:40.665585 hrin_msb-0.2.81/msb/http/client.py
--rw-r--r--   0        0        0      692 2023-06-02 19:43:19.683341 hrin_msb-0.2.81/msb/http/constants.py
--rw-r--r--   0        0        0     6833 2023-05-12 14:20:44.040630 hrin_msb-0.2.81/msb/http/dataclasses.py
--rw-r--r--   0        0        0      988 2023-05-16 17:36:31.238160 hrin_msb-0.2.81/msb/http/exceptions.py
--rw-r--r--   0        0        0     1491 2023-05-12 14:06:51.268257 hrin_msb-0.2.81/msb/http/request.py
--rw-r--r--   0        0        0     3390 2023-05-14 14:58:56.287230 hrin_msb-0.2.81/msb/http/response.py
--rw-r--r--   0        0        0      776 2023-05-12 14:20:44.257502 hrin_msb-0.2.81/msb/http/utils.py
--rw-r--r--   0        0        0     4809 2023-05-12 14:20:43.975540 hrin_msb-0.2.81/msb/http/wrappers.py
--rw-r--r--   0        0        0      169 2023-05-12 14:06:51.278279 hrin_msb-0.2.81/msb/logging/__init__.py
--rw-r--r--   0        0        0     5280 2023-05-12 14:20:43.838792 hrin_msb-0.2.81/msb/logging/config.py
--rw-r--r--   0        0        0     1440 2023-05-12 14:06:51.286888 hrin_msb-0.2.81/msb/logging/constants.py
--rw-r--r--   0        0        0      593 2023-05-12 14:06:51.288884 hrin_msb-0.2.81/msb/logging/handlers.py
--rw-r--r--   0        0        0      229 2023-06-02 20:57:57.869626 hrin_msb-0.2.81/msb/services/__init__.py
--rw-r--r--   0        0        0     5338 2023-06-13 11:22:59.399524 hrin_msb-0.2.81/msb/services/api_service.py
--rw-r--r--   0        0        0     1784 2023-06-02 21:11:10.148401 hrin_msb-0.2.81/msb/services/exceptions.py
--rw-r--r--   0        0        0      183 2023-05-12 14:20:43.823999 hrin_msb-0.2.81/msb/services/isr_service.py
--rw-r--r--   0        0        0      702 2023-06-02 19:45:16.385275 hrin_msb-0.2.81/msb/services/msb_service.py
--rw-r--r--   0        0        0     1658 2023-06-05 17:53:20.383625 hrin_msb-0.2.81/msb/services/notification_service.py
--rw-r--r--   0        0        0     2112 2023-06-06 06:11:01.066173 hrin_msb-0.2.81/msb/services/queue_service.py
--rw-r--r--   0        0        0       25 2023-05-12 14:06:51.290883 hrin_msb-0.2.81/msb/testing/__init__.py
--rw-r--r--   0        0        0     4639 2023-05-12 14:06:51.293121 hrin_msb-0.2.81/msb/testing/api_test.py
--rw-r--r--   0        0        0      450 2023-05-12 14:06:51.294654 hrin_msb-0.2.81/msb/testing/constants.py
--rw-r--r--   0        0        0     1983 2023-05-12 14:06:51.296663 hrin_msb-0.2.81/msb/testing/core.py
--rw-r--r--   0        0        0     3665 2023-05-12 14:20:44.104907 hrin_msb-0.2.81/msb/testing/testdata.py
--rw-r--r--   0        0        0      476 2023-05-12 14:06:51.306644 hrin_msb-0.2.81/msb/testing/unit_test.py
--rw-r--r--   0        0        0      632 2023-06-10 19:41:17.443696 hrin_msb-0.2.81/msb/validation/__init__.py
--rw-r--r--   0        0        0     1297 2023-06-10 18:17:00.285496 hrin_msb-0.2.81/msb/validation/decorators.py
--rw-r--r--   0        0        0     1065 2023-06-10 19:44:50.671677 hrin_msb-0.2.81/msb/validation/exceptions.py
--rw-r--r--   0        0        0     1059 2023-05-12 14:06:51.319957 hrin_msb-0.2.81/msb/validation/rules.py
--rw-r--r--   0        0        0     6480 2023-05-12 14:06:51.321953 hrin_msb-0.2.81/msb/validation/schema.py
--rw-r--r--   0        0        0     2931 2023-06-10 19:47:24.804476 hrin_msb-0.2.81/msb/validation/utils.py
--rw-r--r--   0        0        0      854 2023-06-16 21:13:56.272218 hrin_msb-0.2.81/pyproject.toml
--rw-r--r--   0        0        0     8669 2023-05-12 14:06:51.011419 hrin_msb-0.2.81/README.md
--rw-r--r--   0        0        0    10015 1970-01-01 00:00:00.000000 hrin_msb-0.2.81/setup.py
--rw-r--r--   0        0        0     9455 1970-01-01 00:00:00.000000 hrin_msb-0.2.81/PKG-INFO
+-rw-r--r--   0        0        0     1092 2022-11-10 09:38:13.921857 hrin_msb-0.2.9/LICENSE
+-rw-r--r--   0        0        0        2 2022-11-10 12:43:54.445000 hrin_msb-0.2.9/msb_apis/__init__.py
+-rw-r--r--   0        0        0       40 2022-11-10 11:17:06.989000 hrin_msb-0.2.9/msb_apis/services/__init__.py
+-rw-r--r--   0        0        0     1029 2022-12-07 19:03:28.340580 hrin_msb-0.2.9/msb_apis/services/_exceptions.py
+-rw-r--r--   0        0        0     3111 2023-03-13 09:53:02.720486 hrin_msb-0.2.9/msb_apis/services/api_services.py
+-rw-r--r--   0        0        0      188 2023-02-10 17:26:36.415902 hrin_msb-0.2.9/msb_apis/views/__init__.py
+-rw-r--r--   0        0        0     1946 2023-03-13 09:25:43.917431 hrin_msb-0.2.9/msb_apis/views/_api_view.py
+-rw-r--r--   0        0        0     5905 2023-03-14 09:04:19.508866 hrin_msb-0.2.9/msb_apis/views/_api_viewset.py
+-rw-r--r--   0        0        0     1456 2023-03-04 14:46:50.717490 hrin_msb-0.2.9/msb_apis/views/_constants.py
+-rw-r--r--   0        0        0      973 2022-12-07 06:59:33.253000 hrin_msb-0.2.9/msb_apis/views/_errors.py
+-rw-r--r--   0        0        0      736 2022-12-09 05:28:51.263454 hrin_msb-0.2.9/msb_apis/views/_exceptions.py
+-rw-r--r--   0        0        0      183 2023-02-11 17:31:28.341440 hrin_msb-0.2.9/msb_apis/views/_view.py
+-rw-r--r--   0        0        0      234 2023-02-11 17:08:46.861530 hrin_msb-0.2.9/msb_auth/__init__.py
+-rw-r--r--   0        0        0     1292 2023-02-12 02:06:52.299167 hrin_msb-0.2.9/msb_auth/_constants.py
+-rw-r--r--   0        0        0     2828 2023-02-10 15:14:40.575484 hrin_msb-0.2.9/msb_auth/_defaults.py
+-rw-r--r--   0        0        0       75 2023-02-10 15:14:40.593500 hrin_msb-0.2.9/msb_auth/permissions/__init__.py
+-rw-r--r--   0        0        0      519 2023-02-10 15:14:40.603008 hrin_msb-0.2.9/msb_auth/permissions/_base_permission.py
+-rw-r--r--   0        0        0      769 2023-02-10 15:14:40.612271 hrin_msb-0.2.9/msb_auth/results.py
+-rw-r--r--   0        0        0      223 2023-02-11 17:08:46.851570 hrin_msb-0.2.9/msb_auth/users/__init__.py
+-rw-r--r--   0        0        0     1755 2023-02-11 17:08:46.885320 hrin_msb-0.2.9/msb_auth/users/_auth_token.py
+-rw-r--r--   0        0        0      519 2023-02-10 15:14:40.631191 hrin_msb-0.2.9/msb_auth/users/_datastructures.py
+-rw-r--r--   0        0        0     1270 2023-02-10 15:14:40.635549 hrin_msb-0.2.9/msb_auth/users/_token_user.py
+-rw-r--r--   0        0        0       52 2023-02-10 15:14:40.641073 hrin_msb-0.2.9/msb_auth/validators/__init__.py
+-rw-r--r--   0        0        0     1125 2023-02-10 15:14:40.645182 hrin_msb-0.2.9/msb_auth/validators/jwt_token_validator.py
+-rw-r--r--   0        0        0      126 2023-02-10 17:26:36.471242 hrin_msb-0.2.9/msb_cipher/__init__.py
+-rw-r--r--   0        0        0       40 2023-01-17 10:59:15.812138 hrin_msb-0.2.9/msb_cipher/_asymmetric_cipher.py
+-rw-r--r--   0        0        0        0 2023-01-17 10:56:12.278079 hrin_msb-0.2.9/msb_cipher/_constants.py
+-rw-r--r--   0        0        0      160 2023-01-17 11:05:09.496048 hrin_msb-0.2.9/msb_cipher/_exceptions.py
+-rw-r--r--   0        0        0      712 2023-02-10 17:26:36.404709 hrin_msb-0.2.9/msb_cipher/_symmetric_cipher.py
+-rw-r--r--   0        0        0     1095 2023-02-10 17:26:36.167302 hrin_msb-0.2.9/msb_cipher/cipher.py
+-rw-r--r--   0        0        0      102 2023-02-10 17:26:36.302955 hrin_msb-0.2.9/msb_config/__init__.py
+-rw-r--r--   0        0        0      222 2023-02-10 17:26:36.217757 hrin_msb-0.2.9/msb_config/_constants.py
+-rw-r--r--   0        0        0     1441 2023-02-10 17:26:36.448126 hrin_msb-0.2.9/msb_config/_core.py
+-rw-r--r--   0        0        0      380 2022-12-16 15:07:23.828654 hrin_msb-0.2.9/msb_config/_exceptions.py
+-rw-r--r--   0        0        0     1684 2022-12-07 06:59:03.505322 hrin_msb-0.2.9/msb_config/_var.py
+-rw-r--r--   0        0        0     1078 2023-03-01 23:28:59.608011 hrin_msb-0.2.9/msb_config/main.py
+-rw-r--r--   0        0        0      167 2023-02-10 19:05:35.800763 hrin_msb-0.2.9/msb_const/__init__.py
+-rw-r--r--   0        0        0      992 2023-03-01 23:26:15.764767 hrin_msb-0.2.9/msb_const/names.py
+-rw-r--r--   0        0        0     1638 2023-02-12 02:35:40.088594 hrin_msb-0.2.9/msb_const/paths.py
+-rw-r--r--   0        0        0      200 2023-02-10 17:00:14.017572 hrin_msb-0.2.9/msb_const/regex.py
+-rw-r--r--   0        0        0      278 2023-02-10 17:26:36.292843 hrin_msb-0.2.9/msb_dataclasses/__init__.py
+-rw-r--r--   0        0        0     2077 2022-12-07 06:59:03.498282 hrin_msb-0.2.9/msb_dataclasses/_email.py
+-rw-r--r--   0        0        0      928 2022-12-07 06:59:03.499079 hrin_msb-0.2.9/msb_dataclasses/_singleton.py
+-rw-r--r--   0        0        0      759 2022-12-22 10:46:31.942723 hrin_msb-0.2.9/msb_dataclasses/_wrappers.py
+-rw-r--r--   0        0        0     3058 2023-03-14 09:09:15.392571 hrin_msb-0.2.9/msb_dataclasses/search_parameter.py
+-rw-r--r--   0        0        0      356 2022-12-07 06:59:03.539003 hrin_msb-0.2.9/msb_datetime/__init__.py
+-rw-r--r--   0        0        0      370 2022-12-14 08:56:16.383990 hrin_msb-0.2.9/msb_datetime/_constants.py
+-rw-r--r--   0        0        0     2519 2023-02-10 17:26:36.588823 hrin_msb-0.2.9/msb_datetime/_datetime.py
+-rw-r--r--   0        0        0      107 2022-12-22 10:51:56.369719 hrin_msb-0.2.9/msb_db/__init__.py
+-rw-r--r--   0        0        0      672 2023-03-04 14:51:33.047339 hrin_msb-0.2.9/msb_db/_constants.py
+-rw-r--r--   0        0        0     3750 2023-02-10 17:26:36.198174 hrin_msb-0.2.9/msb_db/_routers.py
+-rw-r--r--   0        0        0      653 2023-02-10 17:26:36.482580 hrin_msb-0.2.9/msb_db/models/__init__.py
+-rw-r--r--   0        0        0     1178 2022-12-07 11:37:03.118588 hrin_msb-0.2.9/msb_db/models/_fields.py
+-rw-r--r--   0        0        0      744 2023-02-10 17:26:36.067375 hrin_msb-0.2.9/msb_db/models/_metafields.py
+-rw-r--r--   0        0        0     3758 2023-03-14 10:22:15.638183 hrin_msb-0.2.9/msb_db/models/_model.py
+-rw-r--r--   0        0        0      960 2023-02-10 17:26:36.558552 hrin_msb-0.2.9/msb_db/models/_model_manager.py
+-rw-r--r--   0        0        0     1141 2023-02-10 17:26:36.101739 hrin_msb-0.2.9/msb_db/models/config_model.py
+-rw-r--r--   0        0        0     2559 2023-02-10 17:26:36.521206 hrin_msb-0.2.9/msb_db/models/logging_models.py
+-rw-r--r--   0        0        0      413 2023-02-11 17:08:46.894398 hrin_msb-0.2.9/msb_devtools/__init__.py
+-rw-r--r--   0        0        0      582 2023-02-10 17:11:44.655700 hrin_msb-0.2.9/msb_devtools/_constants.py
+-rw-r--r--   0        0        0     4050 2023-02-11 17:08:46.825121 hrin_msb-0.2.9/msb_devtools/_django.py
+-rw-r--r--   0        0        0     2078 2023-02-11 17:12:08.156349 hrin_msb-0.2.9/msb_devtools/_dto.py
+-rw-r--r--   0        0        0      977 2023-02-11 09:28:41.800808 hrin_msb-0.2.9/msb_devtools/_funcs.py
+-rw-r--r--   0        0        0     3259 2023-02-11 09:45:38.752873 hrin_msb-0.2.9/msb_devtools/_tasks.py
+-rw-r--r--   0        0        0      103 2022-12-07 06:59:03.517872 hrin_msb-0.2.9/msb_exceptions/__init__.py
+-rw-r--r--   0        0        0      958 2022-12-09 08:38:22.198372 hrin_msb-0.2.9/msb_exceptions/_exception.py
+-rw-r--r--   0        0        0      243 2022-12-07 06:59:03.519197 hrin_msb-0.2.9/msb_exceptions/_handlers.py
+-rw-r--r--   0        0        0      130 2022-12-07 06:59:03.528914 hrin_msb-0.2.9/msb_files/__init__.py
+-rw-r--r--   0        0        0     1050 2023-02-10 17:26:36.327884 hrin_msb-0.2.9/msb_files/_csv.py
+-rw-r--r--   0        0        0     1396 2023-02-10 17:26:36.314833 hrin_msb-0.2.9/msb_files/_docx.py
+-rw-r--r--   0        0        0      332 2023-02-10 17:26:36.089635 hrin_msb-0.2.9/msb_files/_main.py
+-rw-r--r--   0        0        0     1064 2023-02-10 17:26:36.037136 hrin_msb-0.2.9/msb_files/_pdf.py
+-rw-r--r--   0        0        0      261 2022-12-07 06:59:03.533708 hrin_msb-0.2.9/msb_files/core/__init__.py
+-rw-r--r--   0        0        0      949 2023-02-10 17:26:36.341929 hrin_msb-0.2.9/msb_files/core/_base.py
+-rw-r--r--   0        0        0      604 2022-12-07 06:59:33.785432 hrin_msb-0.2.9/msb_files/core/_exceptions.py
+-rw-r--r--   0        0        0      181 2022-12-07 06:59:03.536239 hrin_msb-0.2.9/msb_files/core/_generated_file.py
+-rw-r--r--   0        0        0      198 2022-12-07 06:59:03.537001 hrin_msb-0.2.9/msb_files/core/_messages.py
+-rw-r--r--   0        0        0      251 2023-02-11 17:23:55.748778 hrin_msb-0.2.9/msb_http/__init__.py
+-rw-r--r--   0        0        0     2274 2023-02-11 17:06:14.573054 hrin_msb-0.2.9/msb_http/_client.py
+-rw-r--r--   0        0        0       49 2023-02-11 17:29:26.506776 hrin_msb-0.2.9/msb_http/_constants.py
+-rw-r--r--   0        0        0      893 2023-02-11 17:06:14.579051 hrin_msb-0.2.9/msb_http/_endpoint.py
+-rw-r--r--   0        0        0     1959 2023-02-11 17:06:14.583112 hrin_msb-0.2.9/msb_http/_host.py
+-rw-r--r--   0        0        0     1497 2023-02-11 17:06:14.587308 hrin_msb-0.2.9/msb_http/_request.py
+-rw-r--r--   0        0        0     1525 2023-02-11 17:06:15.028992 hrin_msb-0.2.9/msb_http/_request_wrapper.py
+-rw-r--r--   0        0        0     2719 2023-02-11 17:29:30.937884 hrin_msb-0.2.9/msb_http/_response.py
+-rw-r--r--   0        0        0      172 2022-12-07 06:59:03.507078 hrin_msb-0.2.9/msb_logging/__init__.py
+-rw-r--r--   0        0        0     5283 2023-02-10 17:26:36.119256 hrin_msb-0.2.9/msb_logging/_config.py
+-rw-r--r--   0        0        0     1440 2022-12-07 06:59:03.508630 hrin_msb-0.2.9/msb_logging/_constants.py
+-rw-r--r--   0        0        0      594 2022-12-07 06:59:03.509280 hrin_msb-0.2.9/msb_logging/_handlers.py
+-rw-r--r--   0        0        0       27 2023-02-01 11:12:25.337362 hrin_msb-0.2.9/msb_testing/__init__.py
+-rw-r--r--   0        0        0      447 2023-02-01 11:32:20.869417 hrin_msb-0.2.9/msb_testing/_constants.py
+-rw-r--r--   0        0        0     1984 2023-02-01 11:18:04.612159 hrin_msb-0.2.9/msb_testing/_core.py
+-rw-r--r--   0        0        0     4640 2023-02-10 17:26:36.276023 hrin_msb-0.2.9/msb_testing/api_test.py
+-rw-r--r--   0        0        0     3665 2023-02-10 17:26:36.573027 hrin_msb-0.2.9/msb_testing/testdata.py
+-rw-r--r--   0        0        0      477 2023-02-10 17:26:36.435186 hrin_msb-0.2.9/msb_testing/unit_test.py
+-rw-r--r--   0        0        0      552 2023-02-10 17:26:36.458951 hrin_msb-0.2.9/msb_validation/__init__.py
+-rw-r--r--   0        0        0     4694 2023-02-11 17:33:20.648161 hrin_msb-0.2.9/msb_validation/_decorators.py
+-rw-r--r--   0        0        0     1023 2023-03-13 11:39:18.804251 hrin_msb-0.2.9/msb_validation/_exceptions.py
+-rw-r--r--   0        0        0     1061 2023-03-13 11:37:52.468507 hrin_msb-0.2.9/msb_validation/_rules.py
+-rw-r--r--   0        0        0     6480 2022-12-31 11:24:42.573587 hrin_msb-0.2.9/msb_validation/_schema.py
+-rw-r--r--   0        0        0     1210 2023-03-14 10:23:02.476193 hrin_msb-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     6382 2023-03-14 10:23:26.105369 hrin_msb-0.2.9/README.md
+-rw-r--r--   0        0        0     7705 1970-01-01 00:00:00.000000 hrin_msb-0.2.9/setup.py
+-rw-r--r--   0        0        0     7111 1970-01-01 00:00:00.000000 hrin_msb-0.2.9/PKG-INFO
```

### Comparing `hrin_msb-0.2.81/LICENSE` & `hrin_msb-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.81/msb/apis/api_view.py` & `hrin_msb-0.2.9/msb_apis/views/_api_view.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,95 +1,72 @@
-from typing import Union
+from rest_framework import (viewsets, serializers)
 
-from django.db.models import QuerySet
-from msb.auth import (TokenUser, SessionData, Permissions)
-from msb.cipher import Cipher
-from msb.http import (ApiResponse, RequestInfo, RequestHeaders)
-from rest_framework import (viewsets, serializers, exceptions as drf_exceptions)
-from django.utils.functional import cached_property
+from msb_auth import TokenUser, LoginRequiredPermission
+from ._constants import DEFAULT_LOGGER_NAME
+from msb_http import (ApiResponse, RequestInfo, RequestHeaders)
 
-from .constants import DEFAULT_LOGGER_NAME
+from typing import Union
 
 
 def api_details(request=None, ver='', name=''):
 	return ApiResponse.success(
 		data=dict(method=request.method, version=ver, name=name)
 	)
 
 
 class ApiView(viewsets.GenericViewSet):
-	permission_classes = (Permissions.Authenticated,)
+	permission_classes = (LoginRequiredPermission,)
 	serializer_class = serializers.Serializer
 	default_logger: str = DEFAULT_LOGGER_NAME
 
-	@property
-	def cipher(self) -> Cipher:
-		return Cipher
-
-	@property
-	def exceptions(self):
-		return drf_exceptions
+	"""
+	TODO : implement following code :
+	
+	@staticmethod
+	@renderer_classes((JSONRenderer))
+	def my_exception_handler(exc, context):
+		# response = exception_handler(exc, context)  # <-- this is the default exception_handler
+		import logging
+		logging.exception(exc)
+		return ApiResponse.internal_server_error()
 
-	def handle_exception(self, exc):
-		"""
-		override parent exception handler, to send custom error messages as a response
-		"""
-		try:
-			_auth_exceptions = (self.exceptions.NotAuthenticated, self.exceptions.AuthenticationFailed)
-			if isinstance(exc, _auth_exceptions):
-				if (auth_header := self.get_authenticate_header(self.request)) is not None:
-					return self.api_response.authentication_failed()
-				else:
-					return self.api_response.forbidden()
-
-			return self.api_response.formatted_error_response(super().handle_exception(exc=exc))
-		except Exception as e:
-			return self.api_response.exception(e)
-
-	def api_not_found(self, request, *args, **kwargs):
-		return self.api_response.not_found()
-
-	@classmethod
-	def route(cls, method: str, url: str, action: str):
-		return path(url, cls.as_view(actions={method: action}))
+	def get_exception_handler(self):
+		return self.my_exception_handler
+	"""
 
 	@property
 	def request_info(self) -> RequestInfo:
 		return RequestInfo(meta=self.request.META)
 
 	@property
 	def request_headers(self) -> RequestHeaders:
 		return RequestHeaders(headers=self.request.headers)
 
 	@property
 	def user(self) -> TokenUser:
 		return self.request.user
 
 	@property
-	def session(self) -> SessionData:
-		return self.user.session
-
-	@cached_property
 	def payload(self) -> dict | list:
-		_payload = self.request.data.dict() if hasattr(self.request.data, 'dict') else self.request.data
-		return _payload if type(_payload) in [list, dict] else {}
+		return self.request.data if type(self.request.data) in [list, dict] else {}
 
 	@property
-	def params(self) -> dict:
+	def params(self)->dict:
 		return self.request.query_params.dict()
 
 	@property
 	def logger(self):
 		import logging
 		return logging.getLogger(self.default_logger)
 
 	@property
 	def api_response(self):
 		return ApiResponse
 
-	def serializer(self, data: list | dict | QuerySet = None) -> Union[list, dict]:
+	def serializer(self, data: Union[list, dict] = None) -> Union[list, dict]:
+		from django.db.models import QuerySet
 		if isinstance(data, dict):
 			return data
 
 		return (
 			[item.dict() if hasattr(item, 'dict') else item for item in data]
 		) if (type(data) in [list, QuerySet]) else []
```

### Comparing `hrin_msb-0.2.81/msb/apis/api_viewset.py` & `hrin_msb-0.2.9/msb_apis/views/_api_viewset.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,125 +1,143 @@
+from msb_dataclasses import SearchParameter
+from msb_http import (RestResponse)
+from msb_validation import DefaultRules, validate_against, InvalidPayloadException, ValidationSchema
 from django.db.models import QuerySet
 
-from msb.auth import (Permissions, api_permissions)
-from msb.dataclasses import SearchParameter
-from msb.http import (RestResponse)
-from msb.services import ApiService
-from msb.validation import DefaultRules
-from .api_view import ApiView
-from .constants import (CrudActions, CRUD_URL_PK_NAME)
-from .funcs import ApiCrudRoutes
+from ._api_view import ApiView
+from ._constants import (CRUD_MAPPINGS, BULK_MAPPINGS, CrudActions, CRUD_URL_PK_NAME)
+from ._exceptions import CrudApiExceptions
+from ..services import ApiService
 
 
-class ApiViewset(ApiView, ApiCrudRoutes):
+class ApiViewset(ApiView):
 	service_class: ApiService = None
 	validation_schema_class = None
 	search_parameter_class: SearchParameter = SearchParameter
 	pk_name: str = CRUD_URL_PK_NAME
 
-	def dispatch(self, request, *args, **kwargs):
+	def __validate_crud_request(self, action: str, inp=None, unknown=True, bulk=False, rule=None):
+		if self.validation_schema_class is None:
+			raise CrudApiExceptions.SchemaValidationClassNotDefined
+		default_validation_rule = rule if isinstance(rule, ValidationSchema) else ValidationSchema()
+		rule = self.validation_schema_class.get(action, default=default_validation_rule)
+		if (validation_errors := validate_against(schema=rule, inp=inp, unknown=unknown, bulk=bulk)) is not None:
+			raise InvalidPayloadException(errors=validation_errors)
+
+	@classmethod
+	def crud_routes(cls, actions: list = CrudActions.all, **kwargs):
+		try:
+			from django.urls import path, include
+
+			pk_name = cls.pk_name or CRUD_URL_PK_NAME
+			allowed_actions = actions if isinstance(actions, list) else []
+			single_operation_mappings, bulk_operation_mappings = (dict(), dict())
+
+			for single_mapping in CRUD_MAPPINGS.keys():
+				if single_mapping in allowed_actions and single_mapping not in [CrudActions.create]:
+					single_operation_mappings.update(CRUD_MAPPINGS.get(single_mapping))
+
+			for bulk_mapping in BULK_MAPPINGS.keys():
+				if bulk_mapping in allowed_actions:
+					bulk_operation_mappings.update(BULK_MAPPINGS.get(bulk_mapping))
+
+			return [
+				path("", cls.as_view(actions=bulk_operation_mappings)),
+				path(f"/<str:{pk_name}>", cls.as_view(actions=single_operation_mappings))
+			]
 
-		if (pk := kwargs.get(self.pk_name, None)) is not None:
-			kwargs.update({self.pk_name: self.cipher.decipher(pk), })
-		return super().dispatch(request, *args, **kwargs)
+		except Exception as e:
+			return None
 
-	@api_permissions(Permissions.Management, override=False)
 	def create(self, *args, **kwargs) -> RestResponse:
 		try:
 			is_bulk = not isinstance(self.payload, dict)
-			self._validate_api_input(CrudActions.create, inp=self.payload, unknown=False, bulk=is_bulk)
+			self.__validate_crud_request(CrudActions.create, inp=self.payload, unknown=False, bulk=is_bulk)
 			_create_payload = [self.payload] if not is_bulk else self.payload
 
-			self.service_class.create(*_create_payload, user_id=self.user.id)
+			if not (result := self.service_class.create(*_create_payload)):
+				raise CrudApiExceptions.CreateOperationFailed
 			return self.api_response.success()
 
 		except Exception as e:
 			return self.api_response.exception(e)
 
-	@api_permissions(Permissions.Management, override=False)
 	def retrieve(self, *args, **kwargs) -> RestResponse:
 		try:
-			self._validate_api_input(CrudActions.retrieve, inp=kwargs)
+			self.__validate_crud_request(CrudActions.retrieve, inp=kwargs)
 			_pk = kwargs.get(self.pk_name)
-			result = self.service_class.retrieve(pk=_pk, silent=False)
-			if type(result) not in [list, dict]:
-				result = result.dict() if hasattr(result, "dict") else []
-			return self.api_response.success(data=result)
+			result = self.service_class.retrieve(pk=_pk)
+			return self.api_response.success(data=self.serializer(data=[result]))
 		except Exception as e:
 			return self.api_response.exception(e=e)
 
-	@api_permissions(Permissions.Management, override=False)
 	def list(self, *args, **kwargs) -> RestResponse:
 		try:
 			limit = self.params.get('limit')
 			offset = self.params.get('offset')
 			query_data = self.service_class.list(limit=limit, offset=offset)
-			_data = []
 			if isinstance(query_data, QuerySet):
-				_data = [data.list_fields for data in query_data if hasattr(data, 'list_fields')]
-			else:
-				_data = query_data
-			return self.api_response.success(data=_data)
+				query_data = [data.list_fields for data in query_data]
+
+			return self.api_response.success(data=query_data)
 		except Exception as e:
 			return self.api_response.exception(e=e)
 
-	@api_permissions(Permissions.Management, override=False)
 	def update(self, *args, **kwargs) -> RestResponse:
 		try:
 			_rule = DefaultRules.pk_validation_rule(self.pk_name)
 			_pk = kwargs.get(self.pk_name)
 			_update_data = self.payload
-			self._validate_api_input(CrudActions.update, inp=kwargs, rule=_rule)
-			self._validate_api_input(CrudActions.update, inp=_update_data)
-			self.service_class.update(pk=_pk, user_id=self.user.id, **_update_data)
+			self.__validate_crud_request(CrudActions.update, inp=kwargs, rule=_rule)
+			self.__validate_crud_request(CrudActions.update, inp=_update_data)
+			result = self.service_class.update(pk=_pk, **_update_data)
+			if not (result):
+				raise CrudApiExceptions.UpdateOperationFailed
 			return self.api_response.success()
 		except Exception as e:
 			return self.api_response.exception(e=e)
 
-	@api_permissions(Permissions.Management, override=False)
 	def bulk_update(self, *args, **kwargs) -> RestResponse:
 		try:
 			_payload_list = [self.payload] if isinstance(self.payload, dict) else self.payload
-			self._validate_api_input(CrudActions.update, inp=_payload_list, bulk=True)
+			self.__validate_crud_request(CrudActions.update, inp=_payload_list, bulk=True)
 			for _payload in _payload_list:
 				if (_pk := _payload.get(self.pk_name)) is not None:
 					del _payload[self.pk_name]
-					self.service_class.update(pk=_pk, user_id=self.user.id, **_payload)
+					self.service_class.update(pk=_pk, **_payload)
 			return self.api_response.success()
 		except Exception as e:
 			return self.api_response.exception(e=e)
 
-	@api_permissions(Permissions.Management, override=False)
 	def delete(self, *args, **kwargs) -> RestResponse:
 		try:
 			_rule = DefaultRules.pk_validation_rule(self.pk_name)
 			_pk = kwargs.get(self.pk_name)
-			self._validate_api_input(CrudActions.delete, inp=kwargs, rule=_rule)
-			self.service_class.delete(pk=_pk, user_id=self.user.id)
+			self.__validate_crud_request(CrudActions.delete, inp=kwargs, rule=_rule)
+			if not (result := self.service_class.delete(pk=_pk)):
+				raise CrudApiExceptions.DeleteOperationFailed
 			return self.api_response.success()
 		except Exception as e:
 			return self.api_response.exception(e=e)
 
-	@api_permissions(Permissions.Management, override=False)
 	def bulk_delete(self, *args, **kwargs) -> RestResponse:
 		try:
 			_rule = DefaultRules.pk_validation_rule(self.pk_name)
 			_payload = [self.payload] if isinstance(self.payload, dict) else self.payload
-			self._validate_api_input(CrudActions.delete, inp=_payload, rule=_rule, bulk=True)
+			self.__validate_crud_request(CrudActions.delete, inp=_payload, rule=_rule, bulk=True)
 			for pk_details in _payload:
 				_pk = pk_details.get(self.pk_name)
-				self.service_class.delete(pk=_pk, user_id=self.user.id)
+				self.service_class.delete(pk=_pk)
 			return self.api_response.success()
 		except Exception as e:
 			return self.api_response.exception(e=e)
 
-	@api_permissions(Permissions.Management, override=False)
 	def search(self, *args, **kwargs):
 		try:
 			_rule = DefaultRules.search_validation_rule()
-			self._validate_api_input(CrudActions.search, inp=self.payload, rule=_rule)
+			self.__validate_crud_request(CrudActions.search, inp=self.payload, rule=_rule)
 
 			_search_parameters = self.search_parameter_class(**self.payload)
 			result = self.service_class.search(params=_search_parameters)
-			return self.api_response.success(data=result)
+			return self.api_response.success(data=self.serializer(data=result))
 		except Exception as e:
 			return self.api_response.exception(e)
```

### Comparing `hrin_msb-0.2.81/msb/apis/errors.py` & `hrin_msb-0.2.9/msb_apis/views/_errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,29 @@
+
+
+
 class ErrorViews:
 
 	@staticmethod
 	def __render(request, template_name, context):
 		from django.shortcuts import render
 		return render(request=request, template_name='errors/error_bad_request.html', context={})
 
 	@staticmethod
 	def error_400_handler(request, exception):
 		return ErrorViews.__render(request=request, template_name='errors/error_bad_request.html', context={})
 
 	@staticmethod
 	def error_403_handler(request, exception):
 		return ErrorViews.__render(request=request, template_name='errors/error_permission_denied.html',
-		                           context={})
+		              context={})
 
 	@staticmethod
 	def error_404_handler(request, exception):
 		from django.http import HttpResponseNotFound
 		content_type = 'text/html'
 		return HttpResponseNotFound("no found", content_type=content_type)
 
 	@staticmethod
 	def error_500_handler(request):
 		return ErrorViews.__render(request=request, template_name='errors/error_internal_server.html',
-		                           context={})
+		              context={})
```

### Comparing `hrin_msb-0.2.81/msb/auth/defaults.py` & `hrin_msb-0.2.9/msb_auth/_defaults.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import timedelta
 
-from .constants import MSB_JWT_TOKEN_VALIDATOR, DefaultJwtConfig
-from .users import TokenUser
+from msb_auth.users._token_user import TokenUser
+from ._constants import MSB_JWT_TOKEN_VALIDATOR, DefaultJwtConfig
 
 
 def jwt_user_auth_rule(user: TokenUser):
 	return user
 
 
 class DefaultJwtAuthSettings:
@@ -28,15 +28,15 @@
 		self.blacklist_after_rotation = opt.get(
 			'blacklist_after_rotation') or DefaultJwtConfig.blacklist_after_rotation
 		self.audience = opt.get('audience') or DefaultJwtConfig.audience
 		self.issuer = opt.get('issuer') or DefaultJwtConfig.audience
 
 	@property
 	def authentication_classes(self):
-		return [MSB_JWT_TOKEN_VALIDATOR]
+		return [MSB_JWT_TOKEN_VALIDATOR, ]
 
 	@property
 	def for_token_validation(self) -> dict:
 		return {
 			'TOKEN_USER_CLASS': self.token_user_class,
 			'USER_ID_CLAIM': self.user_id_claim,
 			'USER_AUTHENTICATION_RULE': self.user_authentication_rule,
@@ -57,7 +57,9 @@
 			'ROTATE_REFRESH_TOKENS': self.rotate_refresh_tokens,
 			'BLACKLIST_AFTER_ROTATION': self.blacklist_after_rotation,
 			'ACCESS_TOKEN_LIFETIME': timedelta(minutes=self.access_token_lifetime),
 			'REFRESH_TOKEN_LIFETIME': timedelta(minutes=self.refresh_token_lifetime),
 			'AUDIENCE': self.audience,
 			'ISSUER': self.issuer,
 		}
+
+
```

### Comparing `hrin_msb-0.2.81/msb/cipher/symmetric_cipher.py` & `hrin_msb-0.2.9/msb_cipher/_symmetric_cipher.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 		if self.key is not None:
 			try:
 				if isinstance(data, bytes):
 					data = str(data).encode()
 				return Fernet(key=self.key).decrypt(data).decode()
 			except Exception:
 				pass
-		return data
+		return data
```

### Comparing `hrin_msb-0.2.81/msb/dataclasses/_email.py` & `hrin_msb-0.2.9/msb_dataclasses/_email.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
 
-class EmailConfig(object):
+class EmailConfigData(object):
 	_smtp_host: str = 'localhost'
 	_smtp_port: int = 25
 	_smtp_user: str = ''
 	_smtp_password: str = ''
 	_smtp_use_tls: bool = False
 	_smtp_use_ssl: bool = False
 	_smtp_timeout: int = 0
@@ -60,7 +60,16 @@
 		return self._smtp_ssl_keyfile
 
 	@property
 	def ssl_cert(self):
 		return self._smtp_ssl_certfile
 
 
+class EmailConfig():
+	__config = dict()
+
+	def __init__(self, *namespace_list):
+		for namespace in namespace_list:
+			self.__config[str(namespace).lower()] = EmailConfigData(namespace=namespace)
+
+	def get(self, namespace: str = 'default') -> EmailConfigData:
+		return self.__config.get(namespace.lower())
```

### Comparing `hrin_msb-0.2.81/msb/dataclasses/_singleton.py` & `hrin_msb-0.2.9/msb_dataclasses/_singleton.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-00000000: 6465 6620 7369 6e67 6c65 746f 6e28 636c  def singleton(cl
-00000010: 6173 735f 293a 0d0a 0969 6e73 7461 6e63  ass_):...instanc
-00000020: 6573 203d 207b 7d0d 0a0d 0a09 6465 6620  es = {}.....def 
-00000030: 6765 7469 6e73 7461 6e63 6528 2a61 7267  getinstance(*arg
-00000040: 732c 202a 2a6b 7761 7267 7329 3a0d 0a09  s, **kwargs):...
-00000050: 0969 6620 636c 6173 735f 206e 6f74 2069  .if class_ not i
-00000060: 6e20 696e 7374 616e 6365 733a 0d0a 0909  n instances:....
-00000070: 0969 6e73 7461 6e63 6573 5b63 6c61 7373  .instances[class
-00000080: 5f5d 203d 2063 6c61 7373 5f28 2a61 7267  _] = class_(*arg
-00000090: 732c 202a 2a6b 7761 7267 7329 0d0a 0909  s, **kwargs)....
-000000a0: 7265 7475 726e 2069 6e73 7461 6e63 6573  return instances
-000000b0: 5b63 6c61 7373 5f5d 0d0a 0d0a 0972 6574  [class_].....ret
-000000c0: 7572 6e20 6765 7469 6e73 7461 6e63 650d  urn getinstance.
-000000d0: 0a0d 0a0d 0a63 6c61 7373 2053 696e 676c  .....class Singl
-000000e0: 6574 6f6e 2874 7970 6529 3a0d 0a09 5f69  eton(type):..._i
-000000f0: 6e73 7461 6e63 6573 203d 207b 7d0d 0a0d  nstances = {}...
-00000100: 0a09 6465 6620 5f5f 6361 6c6c 5f5f 2863  ..def __call__(c
-00000110: 6c73 2c20 2a61 7267 732c 202a 2a6b 7761  ls, *args, **kwa
-00000120: 7267 7329 3a0d 0a09 0969 6620 636c 7320  rgs):....if cls 
-00000130: 6e6f 7420 696e 2063 6c73 2e5f 696e 7374  not in cls._inst
-00000140: 616e 6365 733a 0d0a 0909 0963 6c73 2e5f  ances:.....cls._
-00000150: 696e 7374 616e 6365 735b 636c 735d 203d  instances[cls] =
-00000160: 2073 7570 6572 2853 696e 676c 6574 6f6e   super(Singleton
-00000170: 2c20 636c 7329 2e5f 5f63 616c 6c5f 5f28  , cls).__call__(
-00000180: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
-00000190: 0d0a 0909 7265 7475 726e 2063 6c73 2e5f  ....return cls._
-000001a0: 696e 7374 616e 6365 735b 636c 735d 0d0a  instances[cls]..
+00000000: 0d0a 6465 6620 7369 6e67 6c65 746f 6e28  ..def singleton(
+00000010: 636c 6173 735f 293a 0d0a 0969 6e73 7461  class_):...insta
+00000020: 6e63 6573 203d 207b 7d0d 0a0d 0a09 6465  nces = {}.....de
+00000030: 6620 6765 7469 6e73 7461 6e63 6528 2a61  f getinstance(*a
+00000040: 7267 732c 202a 2a6b 7761 7267 7329 3a0d  rgs, **kwargs):.
+00000050: 0a09 0969 6620 636c 6173 735f 206e 6f74  ...if class_ not
+00000060: 2069 6e20 696e 7374 616e 6365 733a 0d0a   in instances:..
+00000070: 0909 0969 6e73 7461 6e63 6573 5b63 6c61  ...instances[cla
+00000080: 7373 5f5d 203d 2063 6c61 7373 5f28 2a61  ss_] = class_(*a
+00000090: 7267 732c 202a 2a6b 7761 7267 7329 0d0a  rgs, **kwargs)..
+000000a0: 0909 7265 7475 726e 2069 6e73 7461 6e63  ..return instanc
+000000b0: 6573 5b63 6c61 7373 5f5d 0d0a 0d0a 0972  es[class_].....r
+000000c0: 6574 7572 6e20 6765 7469 6e73 7461 6e63  eturn getinstanc
+000000d0: 650d 0a0d 0a0d 0a63 6c61 7373 2053 696e  e......class Sin
+000000e0: 676c 6574 6f6e 2874 7970 6529 3a0d 0a09  gleton(type):...
+000000f0: 5f69 6e73 7461 6e63 6573 203d 207b 7d0d  _instances = {}.
+00000100: 0a0d 0a09 6465 6620 5f5f 6361 6c6c 5f5f  ....def __call__
+00000110: 2863 6c73 2c20 2a61 7267 732c 202a 2a6b  (cls, *args, **k
+00000120: 7761 7267 7329 3a0d 0a09 0969 6620 636c  wargs):....if cl
+00000130: 7320 6e6f 7420 696e 2063 6c73 2e5f 696e  s not in cls._in
+00000140: 7374 616e 6365 733a 0d0a 0909 0963 6c73  stances:.....cls
+00000150: 2e5f 696e 7374 616e 6365 735b 636c 735d  ._instances[cls]
+00000160: 203d 2073 7570 6572 2853 696e 676c 6574   = super(Singlet
+00000170: 6f6e 2c20 636c 7329 2e5f 5f63 616c 6c5f  on, cls).__call_
+00000180: 5f28 2a61 7267 732c 202a 2a6b 7761 7267  _(*args, **kwarg
+00000190: 7329 0d0a 0909 7265 7475 726e 2063 6c73  s)....return cls
+000001a0: 2e5f 696e 7374 616e 6365 735b 636c 735d  ._instances[cls]
 000001b0: 0d0a 0d0a 636c 6173 7320 5669 7274 7561  ....class Virtua
 000001c0: 6c44 6174 6143 6c61 7373 3a0d 0a09 5f5f  lDataClass:...__
 000001d0: 6669 656c 6473 3a20 6469 6374 203d 2064  fields: dict = d
 000001e0: 6963 7428 290d 0a09 5f72 6571 7565 7374  ict()..._request
 000001f0: 5f64 6174 613a 2064 6963 7420 3d20 6469  _data: dict = di
 00000200: 6374 2829 0d0a 095f 7265 736f 7572 6365  ct()..._resource
 00000210: 5f66 756e 6374 696f 6e20 3d20 4e6f 6e65  _function = None
```

### Comparing `hrin_msb-0.2.81/msb/dataclasses/_wrappers.py` & `hrin_msb-0.2.9/msb_dataclasses/_wrappers.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.81/msb/dataclasses/search_parameter.py` & `hrin_msb-0.2.9/msb_dataclasses/search_parameter.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,113 +1,69 @@
 from dataclasses import dataclass
-from typing import (AnyStr, Tuple, List, Dict)
 
-from msb.cipher import Cipher
-from msb.db.constants import (DEFAULT_QUERY_OFFSET, DEFAULT_QUERY_LIMIT)
+from msb_cipher import Cipher
+from msb_db._constants import (DEFAULT_QUERY_OFFSET, DEFAULT_QUERY_LIMIT)
 
 
 @dataclass
 class SearchParameter:
-	# this is what goes to the search
-	_model_filters: Dict
-	_fields: List
-	_order_by: AnyStr
-	_limit: int
-	_offset: int
-	_order_field: str
-	# this is what we recieve from payload
-	_raw_filters: Dict
-
-	# this is what we is declared beforehand
-	_model_filter_map: Dict
-	_auto_decrypt_filters: List
+	_model_filters: dict
+	_fields: list = None
+	_order_by: str = None
+	_limit: int = None
+	_offset: int = None
+	_order_field: str = None
+	_filters = dict()
+	_model_filter_map = dict()
+	_auto_decrypt_filters = list()
 
 	def get_query(self, for_model=None):
-		try:
-			self._init_model_filters(model=for_model)
-			_filter_list, _filter_dict = self.compound_filters, self.filters
-			_query_fields, _query_properties = self._extract_query_fields_and_properties(for_model)
-
-			query_set = for_model.objects.from_all
-
-			if len(_filter_list) > 0:
-				query_set = query_set.filter(*_filter_list, **_filter_dict)
-			else:
-				query_set = query_set.filter(**_filter_dict)
-
-			if len(_query_fields) > 0:
-				query_set = query_set.only(*_query_fields)
-
-			if len(_query_properties) > 0:
-				for_model.add_query_properties(*_query_properties)
-
-			if self.order_field:
-				query_set = query_set.order_by(self.order_field)
-			return query_set
-		except Exception as e:
-			raise e
+		self._init_model_filters(model=for_model)
+		query_set = for_model.objects.filter(**self.filters)
+		if self.fields:
+			query_set = query_set.only(*self.fields)
+		if self.order_field:
+			query_set = query_set.order_by(self.order_field)
+		return query_set
 
 	def _init_model_filters(self, model=None):
-		for key, value in self._raw_filters.items():
-			if value is None: continue
+		for key, value in self._filters.items():
 			value = self.__parse_value(key=key, value=value, model=model)
-
-			if key in self.model_filter_map.keys():
-				self.add_filters(self.model_filter_map[key], value)
+			if key in self._model_filter_map.keys():
+				self.add_filters(self._model_filter_map[key], value)
 			elif hasattr(model, key):
 				self.add_filters(key, value)
 
-	def _extract_query_fields_and_properties(self, model=None):
-		_model_fields, _model_properties = [], []
-		if self.fields:
-			for f in self.fields:
-				if isinstance(getattr(model, f, None), property):
-					_model_properties.append(f)
-				else:
-					_model_fields.append(f)
-
-		return _model_fields, _model_properties
-
 	def __parse_value(self, key, value, model):
-		return Cipher.decipher(value) if key in self.auto_decrypt_fields_list(model) else value
+		if key in self.auto_decrypt_fields_list(model):
+			return Cipher.decrypt_list_items(*value) if isinstance(value, list) else Cipher.decrypt(value)
+		return value
 
 	def __init__(self, **kwargs):
 		self._model_filters = dict()
-		self._fields = kwargs.get('fields', [])
-		self._order_by = kwargs.get('order_by', 'ASC')
-		self._limit = kwargs.get('limit', DEFAULT_QUERY_LIMIT)
-		self._offset = kwargs.get('offset', DEFAULT_QUERY_OFFSET)
-		self._order_field = kwargs.get('order_field', None)
-		self._raw_filters = kwargs.get('filters', {})
+		self._fields = kwargs.get('fields') or []
+		self._order_by = kwargs.get('order_by') or 'ASC'
+		self._limit = kwargs.get('limit') or DEFAULT_QUERY_LIMIT
+		self._offset = kwargs.get('offset') or DEFAULT_QUERY_OFFSET
+		self.order_field = kwargs.get('order_field')
+		self._filters = kwargs.get('filters') or dict()
 
 	def add_filters(self, key: str, value):
-		if key and value not in ['', None, []]:
+		if (isinstance(key, str) and value is not None) or (isinstance(value, list) and len(value) > 0):
 			self._model_filters[key] = value
 
 	def auto_decrypt_fields_list(self, model):
-		_secure_field_list = self.auto_decrypt_filters
+		_secure_field_list = self._auto_decrypt_filters if isinstance(self._auto_decrypt_filters, list) else []
 		_secure_field_list.append(model._meta.pk.attname)
 		_private_fields = getattr(model, "_private_fields", [])
 		if isinstance(_private_fields, list):
 			_secure_field_list.extend(_private_fields)
 		return _secure_field_list
 
 	@property
-	def compound_filters(self) -> List | Tuple:
-		return []
-
-	@property
-	def model_filter_map(self) -> dict:
-		return getattr(self, "_model_filter_map", dict())
-
-	@property
-	def auto_decrypt_filters(self) -> list:
-		return getattr(self, "_auto_decrypt_filters", list())
-
-	@property
 	def filters(self) -> dict:
 		return self._model_filters
 
 	@property
 	def fields(self) -> list:
 		return self._fields if isinstance(self._fields, list) and len(self._fields) > 0 else None
 
@@ -127,28 +83,16 @@
 		try:
 			return int(self._offset) if int(self._offset) >= 0 else DEFAULT_QUERY_OFFSET
 		except Exception:
 			return 0
 
 	@property
 	def order_field(self) -> str:
-		if self._order_field is not None:
-			return f"-{self._order_field}" if str(self.order_by).upper() != 'ASC' else self._order_field
-		return None
+		return self._order_field
 
-
-@dataclass
-class SearchParameterRequest:
-	fields: List
-	filters: Dict
-	limit: int
-	offset: int
-	order_field: str | None
-	order_by: str | None
-
-	def __init__(self, **kwargs):
-		self.fields = kwargs.get('fields') or []
-		self.filters = kwargs.get('filters') or dict()
-		self.limit = kwargs.get('limit') or DEFAULT_QUERY_LIMIT
-		self.offset = kwargs.get('offset') or DEFAULT_QUERY_OFFSET
-		self.order_field = kwargs.get('order_field')
-		self.order_by = kwargs.get('order_by')
+	@order_field.setter
+	def order_field(self, value):
+		if value is not None:
+			if self.order_by != 'ASC':
+				self._order_field = f"-{value}"
+			else:
+				self._order_field = value
```

### Comparing `hrin_msb-0.2.81/msb/datetime/wrappers.py` & `hrin_msb-0.2.9/msb_datetime/_datetime.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 import logging
 from datetime import datetime, timedelta
 
 import pytz
 
-from .constants import *
+from . import _constants as DT_CONST
 
 
-def current_time(frmt=DEFAULT_TIME_FORMAT):
+def current_time(frmt=DT_CONST.DEFAULT_TIME_FORMAT):
 	return datetime.now().time().strftime(frmt)
 
 
-def current_date(frmt=DEFAULT_DATE_FORMAT):
+def current_date(frmt=DT_CONST.DEFAULT_DATE_FORMAT):
 	return datetime.now().date().strftime(frmt)
 
 
-def current_timestamp(frmt=TIMESTAMP_FORMAT):
+def current_timestamp(frmt=DT_CONST.TIMESTAMP_FORMAT):
 	return datetime.now().strftime(frmt)
 
 
 def timestamp_diff(latest=None, old=None, return_in='sec|min|hr|day'):
 	diff_data = dict(sec=0, min=0, hr=0, day=0)
 	return_in = 'sec' if return_in not in ['sec', 'min', 'hr', 'day'] else return_in
 	try:
-		latest = datetime.strptime(latest, TIMESTAMP_FORMAT)
-		old = datetime.strptime(old, TIMESTAMP_FORMAT)
+		latest = datetime.strptime(latest, DT_CONST.TIMESTAMP_FORMAT)
+		old = datetime.strptime(old, DT_CONST.TIMESTAMP_FORMAT)
 		diff = (latest - old)
 		diff_data['sec'] = diff.total_seconds()
 		diff_data['min'] = (diff_data.get('sec') / 60)
 		diff_data['hr'] = (diff_data.get('min') / 60)
 		diff_data['day'] = diff.days
 	# print (diff_data)
 	except Exception as e:
 		logging.exception(e)
 	return diff_data.get(return_in)
 
 
-def create_datetime(inp_dtime=None, hours=0, mins=0, secs=0, days=0, inp_fmt=TIMESTAMP_FORMAT, out_fmt=None):
+def create_datetime(
+	inp_dtime=None, hours=0, mins=0, secs=0, days=0, inp_fmt=DT_CONST.TIMESTAMP_FORMAT,
+	out_fmt=None
+):
 	try:
 		out_fmt = inp_fmt if out_fmt is None else out_fmt
 		inp_dtime = str(datetime.now().strftime(inp_fmt)) if inp_dtime is None else inp_dtime
 		return (
 			datetime.strptime(inp_dtime, inp_fmt) +
 			timedelta(
 				hours=hours, days=days,
@@ -47,25 +50,25 @@
 				seconds=secs
 			)
 		).strftime(out_fmt)
 	except Exception as e:
 		print(e)
 
 
-def parse_datetime(inp_dtime=None, inp_fmt=TIMESTAMP_FORMAT):
+def parse_datetime(inp_dtime=None, inp_fmt=DT_CONST.TIMESTAMP_FORMAT):
 	result = None
 	try:
 		result = datetime.strptime(str(inp_dtime), inp_fmt)
 
 	except Exception as e:
 		logging.exception(e)
 	return result
 
 
-def convert_to_utc(inp_dtime=None, inp_fmt=TIMESTAMP_FORMAT, out_fmt=None, ist_time_diff='0:00'):
+def convert_to_utc(inp_dtime=None, inp_fmt=DT_CONST.TIMESTAMP_FORMAT, out_fmt=None, ist_time_diff='0:00'):
 	try:
 		out_fmt = inp_fmt if out_fmt is None else out_fmt
 		dt = parse_datetime(str(inp_dtime), inp_fmt=inp_fmt)
 		hour_diff, mins_diff = ist_time_diff.split(":")
 		utc_time = create_datetime(
 			dt.__str__(), hours=-int(hour_diff), mins=-int(mins_diff),
 			inp_fmt=inp_fmt
@@ -73,14 +76,14 @@
 		return parse_datetime(utc_time, inp_fmt=inp_fmt).strftime(out_fmt)
 
 
 	except Exception as e:
 		logging.exception(e)
 
 
-def timezone_offset(timezone=DEFAULT_TIMEZONE):
+def timezone_offset(timezone=DT_CONST.DEFAULT_TIMEZONE):
 	offset = 0
 	try:
 		offset = (datetime.now(pytz.timezone(timezone)).utcoffset().total_seconds() / 3600)
 	except Exception as e:
 		logging.exception(e)
 	return offset
```

### Comparing `hrin_msb-0.2.81/msb/db/config_model.py` & `hrin_msb-0.2.9/msb_db/models/config_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 from django.db import models
 
-from .model_fields import EncryptedString
-from .msb_model import MsbModel
-from .msb_model import MsbModelManager
+from ._fields import EncryptedString
+from ._model import MsbModel
+from ._model import MsbModelManager
 
 
 class ConfigurationModelManager(MsbModelManager):
 
-	def get_config(self, name: str, map_to=None):
+	def get_config(self, name: str, map_to= None):
 		_config_list = []
 		try:
 			_config_list = self.get_queryset().filter(name=name).all()
 		except Exception:
 			pass
 		return map_to(*_config_list) if callable(map_to) else _config_list
 
 
 # Configuration model
 class Configuration(MsbModel):
-	_list_field_names = ["name", "label", "value"]
-	_identifier_field = "name"
-
 	# meta data
 	class Meta:
 		abstract = True
 		indexes = [models.Index(fields=['name', 'key'])]
 		unique_together = ("name", "key")
 
 	# Model fields
```

### Comparing `hrin_msb-0.2.81/msb/db/constants.py` & `hrin_msb-0.2.9/msb_db/_constants.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.81/msb/db/logging_models.py` & `hrin_msb-0.2.9/msb_db/models/logging_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 
 from django.db.models import (manager, DateTimeField, IntegerField, CharField, TextField)
 
-from msb.logging import (
+from msb_logging import (
 	LOG_DB, LOG_TABLE, CHOICES_LOG_LEVELS, DEFAULT_DBLOG_COLUMN_MAPPINGS,
 	SYSTEM_DBLOG_COLUMN_MAPPINGS
 )
-from .models import (MsbModel)
+from ..models import (MsbModel)
 
 
 class LoggingModelManager(manager.Manager):
 	log_db = LOG_DB
 
 	def get_queryset(self):
 		return super(LoggingModelManager, self).get_queryset().using(self.log_db)
```

### Comparing `hrin_msb-0.2.81/msb/db/metafields.py` & `hrin_msb-0.2.9/msb_db/models/_metafields.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from django.db import models
 
-from .constants import (
+from ._model import MsbModel
+from .._constants import (
 	COLUMN_NAME_DELETED, COLUMN_NAME_CREATED_AT, COLUMN_NAME_UPDATED_AT,
 	COLUMN_NAME_CREATED_BY, COLUMN_NAME_UPDATED_BY
 )
-from .msb_model import MsbModel
 
 
 class MsbModelMetaFields(MsbModel):
 	class Meta:
 		abstract = True
 
-	updated_at = models.DateTimeField(db_column=COLUMN_NAME_UPDATED_AT, auto_now=True, null=True)
+	updated_at = models.DateTimeField(db_column=COLUMN_NAME_UPDATED_AT, auto_now=True)
 	updated_by = models.IntegerField(db_column=COLUMN_NAME_UPDATED_BY, null=True, default=None)
-	created_at = models.DateTimeField(db_column=COLUMN_NAME_CREATED_AT, auto_now_add=True, null=True)
+	created_at = models.DateTimeField(db_column=COLUMN_NAME_CREATED_AT, auto_now_add=True)
 	created_by = models.IntegerField(db_column=COLUMN_NAME_CREATED_BY, null=True, default=None)
 	is_deleted = models.BooleanField(db_column=COLUMN_NAME_DELETED, default=False, null=False)
```

### Comparing `hrin_msb-0.2.81/msb/db/model_fields.py` & `hrin_msb-0.2.9/msb_db/models/_fields.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 from django.db.models import (TextField, BigAutoField)
 
-from msb.cipher import Cipher
+from msb_cipher import Cipher
 
 
 class EncryptedDatabaseField(TextField):
 	description = "Encrypted Field Holds Private Data"
 	_type = str
 
-
 	def __init__(self, *args, **kwargs):
 		kwargs['blank'] = True
 		kwargs['null'] = True
 		super().__init__(*args, **kwargs)
 
 	def deconstruct(self):
 		name, path, args, kwargs = super().deconstruct()
 		del kwargs["blank"]
 		del kwargs["null"]
 		return name, path, args, kwargs
 
 	def get_prep_value(self, value):
-		return Cipher.encrypt(data=super().get_prep_value(value)) if value not in [None,''] else value
+		return Cipher.encrypt(data=super().get_prep_value(value))
 
 	def from_db_value(self, value, expression, connection):
-		return Cipher.decrypt(data=value) if value not in [None,''] else value
+		return Cipher.decrypt(data=value)
 
 	def to_python(self, value):
-		return self._type((Cipher.decrypt(data=value) if value not in [None,''] else value ))
+		return self._type(Cipher.decrypt(data=value))
 
 
 class EncryptedInteger(EncryptedDatabaseField):
 	_type = int
 
 
 class EncryptedString(EncryptedDatabaseField):
```

### Comparing `hrin_msb-0.2.81/msb/db/msb_model.py` & `hrin_msb-0.2.9/msb_db/models/_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,163 +1,124 @@
-from functools import cache
-
-from django.conf import settings
 from django.core.serializers import serialize
 from django.db import models as Models
-from django.utils.functional import cached_property
 
-from msb.cipher import Cipher
-from .constants import (COLUMN_NAME_DELETED, COLUMN_NAME_DELETED_BY)
-from .msb_model_manager import MsbModelManager
+from msb_cipher import Cipher
+from ._model_manager import MsbModelManager
+from .._constants import (COLUMN_NAME_DELETED, COLUMN_NAME_DELETED_BY)
+from django.conf import settings
+
+DB_ENCRYPT_PRIVATE_FIELDS = getattr(settings, 'DB_ENCRYPT_PRIVATE_FIELDS', False)
+DB_PK_IS_PRIVATE_FIELD = getattr(settings, 'DB_PK_IS_PRIVATE_FIELD', False)
 
 
 class MsbModel(Models.Model):
 	_private_fields: list = []
-	_protected_fields: list = []
 	_list_field_names: list = []
 	_identifier_field: str = ""
-
-	_encrypt_private_fields: bool = settings.MSB_DB_ENCRYPT_PRIVATE_FIELDS
-	_encrypt_protected_fields: bool = settings.MSB_DB_ENCRYPT_PROTECTED_FIELDS
-	_pk_is_private_fields: bool = settings.MSB_DB_PK_IS_PRIVATE_FIELD
-	_hidden_fields: list = []
-	_query_properties: list = []
+	_encrypt_private_fields: bool = DB_ENCRYPT_PRIVATE_FIELDS
+	_pk_is_private_fields: bool = DB_PK_IS_PRIVATE_FIELD
 
 	class Meta:
 		abstract = True
 
 	@property
-	def pk_name(self):
-		return self._meta.pk.attname
-
-	@property
-	def pk_value(self):
-		return getattr(self, self.pk_name) if self.pk_name is not None else ""
-
-	@property
-	def identifier(self):
-		return f"{getattr(self, self.identifier_field_name)}" if hasattr(self, self.identifier_field_name) else ""
-
-	@property
-	def rows(self):
-		return self.objects
-
-	@classmethod
-	def add_query_properties(cls, *properties):
-		cls._query_properties.extend(properties)
-
-	objects = MsbModelManager()
-
-	@property
-	def serialized(self):
-		return serialize('python', [self])
-
-	def delete(self, deleted_by=None, using=None, keep_parents=False):
-		if hasattr(self, COLUMN_NAME_DELETED):
-			setattr(self, COLUMN_NAME_DELETED, True)
-
-		if hasattr(self, COLUMN_NAME_DELETED_BY):
-			setattr(self, COLUMN_NAME_DELETED_BY, deleted_by)
-		self.save()
-		return True
-
-	def recover(self):
-		if hasattr(self, COLUMN_NAME_DELETED):
-			setattr(self, COLUMN_NAME_DELETED, False)
-		self.save()
-		return True
-
-	@property
-	def encrypted_fields(self) -> list:
+	def secure_fields(self):
 		_secure_fields = self._private_fields if isinstance(self._private_fields, list) else []
 		if self._pk_is_private_fields:
 			_secure_fields.append(self._meta.pk.attname)
 		return _secure_fields
 
 	@property
-	def encoded_fields(self) -> list:
-		return self._protected_fields if isinstance(self._protected_fields, list) else []
-
-	@property
 	def identifier_field_name(self):
 		if isinstance(self._identifier_field, str) and len(self._identifier_field) > 0:
 			return self._identifier_field
 		return ''
 
+	def _get_field_value(self, field_name: str, encrypt: bool = False, default=None):
+		try:
+			if "." in field_name:
+				field_name, relation_name, *_ = field_name.split(".")
+				local_field_value = getattr(self, field_name, None)
+				field_value = local_field_value._get_field_value(relation_name, default=None)
+			else:
+				field_value = getattr(self, field_name, default)
+				if isinstance(field_value, MsbModel):
+					field_value = field_value._get_field_value(field_value.pk_name)
+
+		except Exception as e:
+			field_value = None
+		finally:
+
+			if (field_name in self.secure_fields) and (encrypt or self._encrypt_private_fields):
+				return Cipher.encrypt(field_value)
+			return field_value
+
+
 	@property
 	def related_fields(self):
 		fields = []
 		for field in self._meta.fields:
-			if field.get_internal_type() in ['ForeignKey', 'ManyToManyField']:
+			if field.get_internal_type() in ['ForeignKey']:
 				fields.append(field.name)
 		return fields
 
 	@property
-	def list_fields(self) -> dict:
-		return self._get_field_values(
-			*[self.pk_name, *self._list_field_names] if isinstance(self._list_field_names, list) else []
-		)
-
-	def __formatted_field_value(self, field_name: str, field_value: str, force_encrypt: bool = False):
-		if field_name in self.encrypted_fields and (force_encrypt or self._encrypt_private_fields):
-			return Cipher.encrypt(field_value)
-		elif field_name in self.encoded_fields and (force_encrypt or self._encrypt_protected_fields):
-			return Cipher.encode_base64(field_value)
-		else:
-			return field_value
+	def pk_name(self):
+		return self._meta.pk.attname
 
-	def _field_value(self, field_name: str, default=None):
-		try:
-			if "." in field_name:
-				field_name, relation_name, *_ = field_name.split(".")
-				local_field_value = getattr(self, field_name, default)
-				field_value = local_field_value._get_field_value(relation_name, default=None)
-			else:
-				field_value = getattr(self, field_name, default)
-				if isinstance(field_value, MsbModel):
-					field_value = field_value._field_value(field_value.pk_name)
+	@property
+	def pk_value(self):
+		return getattr(self, self.pk_name) if self.pk_name is not None else ""
 
-		except Exception as e:
-			field_value = default
-		return field_value
+	@property
+	def identifier(self):
+		return f"{getattr(self, self.identifier_field_name)}" if hasattr(self, self.identifier_field_name) else ""
 
-	@cache
-	def __should_fetch_field(self, field_name: str, include_properties: bool) -> bool:
-		_should_fetch = not any([
-			field_name.startswith('_'),
-			field_name in self._hidden_fields,
-			(isinstance(field_name, property) and not include_properties),
-		])
-		return _should_fetch
+	@property
+	def list_field_names(self) -> list:
+		return [self.pk_name, *self._list_field_names] if isinstance(self._list_field_names, list) else None
 
-	def _get_field_values(
-			self, *field_names, default=None, force_encrypt: bool = False, include_properties: bool = False):
+	def dict(self, encrypted: bool = False):
+		encrypted = encrypted or self._encrypt_private_fields
 		try:
 			return {
-				field_name.replace('.', '_'): self.__formatted_field_value(
-					field_name, self._field_value(field_name, default), force_encrypt
-				) for field_name in field_names
-				if self.__should_fetch_field(field_name, include_properties)
+				k: v if (k not in self.secure_fields or not encrypted) else Cipher.encrypt(v)
+				for k, v in super().__dict__.items()
+				if not k.startswith('__') and not k.startswith('_') and not callable(k)
 			}
-		except Exception as e:
+
+		except Exception:
 			return dict()
 
-	def dict(self, encrypted: bool = False, include_properties: bool = False) -> dict:
-		_model_fields = [*self.__dict__.keys(), *getattr(self, '_query_properties', [])]
-		return self._get_field_values(*_model_fields, force_encrypt=encrypted, include_properties=include_properties)
+	@property
+	def list_fields(self) -> dict:
+		if len(self.list_field_names) > 0:
+			return {field_name.replace('.', '_'): self._get_field_value(field_name) for field_name in self.list_field_names}
+		return None
+
+	@property
+	def serialized(self):
+		return serialize('python', [self])
+
+	def delete(self, deleted_by=None, using=None, keep_parents=False):
+		if hasattr(self, COLUMN_NAME_DELETED):
+			setattr(self, COLUMN_NAME_DELETED, True)
+
+		if hasattr(self, COLUMN_NAME_DELETED_BY):
+			setattr(self, COLUMN_NAME_DELETED_BY, deleted_by)
+		self.save()
+		return True
 
 	def __str__(self):
 		return f"<{self.__class__.__name__} [{self.pk_value}]: {self.identifier}>"
 
 	def __unicode__(self):
 		return self.__str__()
 
 	def __repr__(self):
 		return self.__str__()
 
-	@classmethod
-	def has_model_field(cls, field_name: str) -> bool:
-		return all([
-			hasattr(cls, field_name),
-			type(getattr(cls, field_name, None)) not in [property, cached_property],
-			not field_name.startswith('_'),
-		])
+	@property
+	def rows(self):
+		return self.objects
+
+	objects = MsbModelManager()
```

### Comparing `hrin_msb-0.2.81/msb/db/msb_model_manager.py` & `hrin_msb-0.2.9/msb_db/models/_model_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 from django.db import models
-from msb.cipher import Cipher
 
-from .constants import (COLUMN_NAME_DELETED)
+from msb_cipher import Cipher
+from .._constants import (COLUMN_NAME_DELETED)
 
 
 class MsbModelManager(models.Manager):
 	_default_filters = {}
 
 	def _get_filtered_queryset(self, **filters):
 		_query_set = super(MsbModelManager, self).get_queryset()
 		query_filters = {}
 		for filtername, filtervalue in filters.items():
 			if hasattr(self.model, filtername):
 				query_filters[filtername] = filtervalue
 		return _query_set.filter(**query_filters)
 
-	def retrieve(self, *args, **kwargs):
-		return super(MsbModelManager, self).get(*args, **kwargs)
-
 	def get(self, *args, **kwargs):
-		pk = kwargs.get('pk')
 		filters = {**kwargs}
+		pk = kwargs.get('pk')
 		if pk is not None and isinstance(pk, str):
-			filters['pk'] = int(Cipher.decipher(pk))
-		return self.retrieve(*args, **filters)
+			filters['pk'] = int(Cipher.decrypt(pk))
+		return super(MsbModelManager, self).get(*args, **filters)
 
 	@property
 	def deleted(self):
 		return self._get_filtered_queryset(**{COLUMN_NAME_DELETED: True})
 
-	@property
-	def from_all(self):
-		return super(MsbModelManager, self).get_queryset()
-
 	def get_queryset(self):
 		return self._get_filtered_queryset(**{COLUMN_NAME_DELETED: False, **self._default_filters})
 
+
+
```

### Comparing `hrin_msb-0.2.81/msb/db/routers.py` & `hrin_msb-0.2.9/msb_db/_routers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import (abstractmethod, ABC)
 
-from .constants import (
+from ._constants import (
 	DEFAULT_MIGRATION_DATABASE,
 	DEFAULT_DATABASE_NAME, DEFAULT_APP_LABLES_TO_ROUTE
 )
 
 
 class DjangoDatabaseRouterInterface(ABC):
 	OP_LIST = ('write', 'read', 'relation', 'migration')
@@ -93,8 +93,9 @@
 			_migrate = mapped_db == db
 
 		# check if we should even try to route
 		elif app_label in self.db_allowed_app_labels:
 			# Allow app model to migrate on the database
 			_migrate = db in self.db_to_migrate_to
 
+
 		return _migrate
```

### Comparing `hrin_msb-0.2.81/msb/devtools/dataclasses.py` & `hrin_msb-0.2.9/msb_devtools/_dto.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from dataclasses import dataclass
 
-from msb.env import NameConst
+import msb_const
 
 
 @dataclass
 class DbVendorConfig:
 	query_to_list_tables: str
 	query_to_drop_table: str
 	excluded_tables: list
@@ -17,26 +17,27 @@
 				if table[0] not in self.excluded_tables and self.query_to_drop_table.strip(" ") != "":
 					_drop_table_queries.append(self.query_to_drop_table.format(table_name=table[0]))
 		return _drop_table_queries
 
 
 class DjangoMigrationConfig:
 	_is_local_env: bool = False
+	_remove_migration_files: bool = False
 	_drop_tables_from_db: bool = False
 	_db_to_drop_tables_from: list = list()
 	_apps_to_migrate: list = list()
 	_dbs_to_migrate: list = list()
 
 	@property
 	def is_local_env(self) -> bool:
 		return self._is_local_env
 
 	@property
 	def remove_migration_files(self) -> bool:
-		return False
+		return self._remove_migration_files
 
 	@property
 	def drop_tables_from_db(self) -> bool:
 		return self._drop_tables_from_db
 
 	@property
 	def db_to_drop_tables_from(self) -> tuple:
@@ -56,18 +57,20 @@
 	def set_dbs_to_migrate(self, *db_list):
 		self._dbs_to_migrate = db_list
 
 	def __init__(self, env: str, **kwargs):
 
 		if isinstance(env, str):
 
-			self._is_local_env = env.lower() == NameConst.LOCAL_ENV_NAME
+			self._is_local_env = env.lower() == msb_const.names.LOCAL_ENV_NAME
 
 			if self.is_local_env:
+				self._remove_migration_files = kwargs.get("remove_migration_files") == True
 				self._drop_tables_from_db = kwargs.get("drop_tables_from_db") == True
-				self._db_to_drop_tables_from = kwargs.get("db_to_drop_tables_from") or [NameConst.DEFAULT_DATABASE_NAME]
+				self._db_to_drop_tables_from = kwargs.get("db_to_drop_tables_from") or [
+					msb_const.names.DEFAULT_DATABASE_NAME]
 		else:
 			logging.warning("Invalid or empty environment name.")
 
 
 class DjangoFixtureDirs:
 	pass
```

### Comparing `hrin_msb-0.2.81/msb/env/core.py` & `hrin_msb-0.2.9/msb_config/_core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 import logging
 import os
 from pathlib import Path
 
-from .constants import NameConst
-from .exceptions import MsbConfigException
+from ._constants import (DOT_ENV_FILE, ENV_LOAD_STATUS_KEY)
+from ._exceptions import MsbConfigException
 
 
 def __get_config_file_type(config_file):
 	return os.path.basename(config_file)
 
 
 def __get_environment_file(config_path: str, main_file: str, local_file: str):
 	if not os.path.isdir(config_path):
-		raise MsbConfigException.BaseDirDoesNotExists(config_path, desc=config_path)
+		raise MsbConfigException.BaseDirDoesNotExists(config_path,desc=config_path)
 
 	local_config_file = Path(config_path).joinpath(local_file)
 	main_config_file = Path(config_path).joinpath(main_file)
 
 	if local_config_file.exists():
 		return local_config_file.__str__()
 	elif main_config_file.exists():
 		return main_config_file.__str__()
 	else:
 		raise MsbConfigException.ConfigFileDoesNotExist(local_config_file, main_config_file)
 
 
 def __load_configuration_file(config_file: str):
-	if NameConst.DOT_ENV_FILE_NAME in config_file:
+	if DOT_ENV_FILE in config_file:
 		from dotenv import load_dotenv
 		return load_dotenv(config_file, verbose=True)
 
 
 def load_config(env_path: str = '', main_file: str = '', local_file: str = ''):
 	try:
 		config_file = __get_environment_file(config_path=env_path, main_file=main_file, local_file=local_file)
 		load_config = __load_configuration_file(config_file=config_file)
 
 		if load_config:
-			os.environ[NameConst.ENV_LOAD_STATUS_KEY_NAME] = '1'
+			os.environ[ENV_LOAD_STATUS_KEY] = '1'
 		else:
 			raise MsbConfigException.ConfigurationLoadingFailed(config_file)
 	except Exception as e:
 		logging.error(e)
 		exit()
```

### Comparing `hrin_msb-0.2.81/msb/exceptions/_exception.py` & `hrin_msb-0.2.9/msb_exceptions/_exception.py`

 * *Files 21% similar despite different names*

```diff
@@ -30,15 +30,7 @@
 		import logging
 		logging.exception(self)
 
 
 class ApiException(AppException):
 	def __init__(self, message: str = None, desc: str = None, errors: dict = None):
 		super().__init__(message=message, errors=errors, desc=desc)
-
-
-class CrudApiException(ApiException):
-	_message: str = "Failed to process the {resource} data."
-
-	def __init__(self, resource: str, desc: str = None, errors: dict = None):
-		message = self._message.format(resource=(resource or "requested"))
-		super().__init__(message=message, errors=errors, desc=desc)
```

### Comparing `hrin_msb-0.2.81/msb/files/core.py` & `hrin_msb-0.2.9/msb_files/core/_base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 from abc import ABC, abstractmethod
 
-from .dataclasses import GeneratedFile
+from ._generated_file import GeneratedFile
 
 
 class FileInterface(ABC):
 	"""Save Function will generate the file to the path given during function call"""
-
 	@abstractmethod
 	def save(self, filename: str, location: str) -> GeneratedFile:
 		pass
 
 	"""set_content() Function will store the content values that will used to save within the file"""
-
 	@abstractmethod
 	def set_content(self, content: str):
 		pass
 
 	"""set_file_overwrite() Function will be used if someone want to overwrite the existed file"""
-
 	@abstractmethod
 	def set_file_overwrite(self):
 		pass
 
 	@abstractmethod
 	def set_protection(self):
 		pass
```

### Comparing `hrin_msb-0.2.81/msb/files/csv.py` & `hrin_msb-0.2.9/msb_files/_csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		return self
 
 	def save(self, filename: str, location: str) -> GeneratedFile:
 		file = GeneratedFile()
 		try:
 			filename = filename
 			content = self.content
-			filepath = os.path.join(location, filename + self._extension)
+			filepath = os.path.join(location, filename+self._extension)
 
 			if os.path.exists(filepath) and self.file_overwrite is False:
 				raise FileExceptions.CsvException
 
 			Path(location).mkdir(parents=True, exist_ok=True)
 			dataframe = pd.DataFrame(content)
 			dataframe.to_csv(filepath, index=False)
```

### Comparing `hrin_msb-0.2.81/msb/files/docx.py` & `hrin_msb-0.2.9/msb_files/_docx.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import os
 from pathlib import Path
 
 from pdf2docx import Converter
 
+from ._pdf import PdfFile
 from .core import FileExceptions
 from .core import FileInterface, FileBase
 from .core import FileMessage
 from .core import GeneratedFile
-from .pdf import PdfFile
 
 
 class DocxFile(FileBase, FileInterface):
 	_extension = None
 
 	def __init__(self):
 		self._extension = ".docx"
 
 	def save(self, filename: str, location: str) -> GeneratedFile:
 		file = GeneratedFile()
 		try:
 			content = self.content
-			doc_filepath = os.path.join(location, filename + self._extension)
+			doc_filepath = os.path.join(location, filename+self._extension)
 			Path(location).mkdir(parents=True, exist_ok=True)
 			if os.path.exists(doc_filepath) and self.file_overwrite is False:
 				raise FileExceptions.DocxExistsException
 			"""Generate PDF"""
 			pdf = PdfFile().set_content(content)
 			if self.file_overwrite is True:
 				pdf.set_file_overwrite()
```

### Comparing `hrin_msb-0.2.81/msb/files/exceptions.py` & `hrin_msb-0.2.9/msb_files/core/_exceptions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from msb.exceptions import AppException
+from msb_exceptions import AppException
 
 
 class FileExceptions:
 	class DefaultException(AppException):
 		_message = "Something went wrong"
 
 	class PdfException(AppException):
```

### Comparing `hrin_msb-0.2.81/msb/files/pdf.py` & `hrin_msb-0.2.9/msb_files/_pdf.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.81/msb/http/request.py` & `hrin_msb-0.2.9/msb_http/_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,7 +61,10 @@
 
 	def __init__(self, headers=None):
 		self.__headers = headers
 
 	@property
 	def user_agent(self) -> str:
 		return self.__headers.get('User-Agent')
+
+
+
```

### Comparing `hrin_msb-0.2.81/msb/http/response.py` & `hrin_msb-0.2.9/msb_http/_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
-from msb.exceptions import AppException
-from msb.exceptions import MsbExceptionHandler
 from rest_framework import status
 from rest_framework.response import Response as RestResponse
 
+from msb_exceptions import AppException
+from msb_exceptions import CustomExceptionHandler
+
 
 class ApiResponse:
 	data_types = [list, dict]
 
 	@staticmethod
 	def _dispatch(data: dict = None, status=status.HTTP_200_OK) -> RestResponse:
 		headers = dict()
@@ -20,26 +21,26 @@
 		response_data = dict(
 			success=True, message=msg,
 			code=200, data=([] if type(data) not in ApiResponse.data_types else data)
 		)
 		return ApiResponse._dispatch(data=response_data)
 
 	@staticmethod
-	def error(msg: str = "Failure", err_code=600, data=None, http_code=status.HTTP_200_OK) -> RestResponse:
+	def error(msg: str = "Failure", err_code=600, data=None) -> RestResponse:
 		response_data = dict(
 			success=False,
 			message=msg,
 			code=err_code,
 			data=([] if type(data) not in ApiResponse.data_types else data)
 		)
-		return ApiResponse._dispatch(data=response_data, status=http_code)
+		return ApiResponse._dispatch(data=response_data)
 
 	@staticmethod
 	def exception(e: AppException | Exception = None, fallback: bool = True) -> RestResponse:
-		MsbExceptionHandler.handle_exception(e=e)
+		CustomExceptionHandler.handle_exception(e=e)
 		if not isinstance(e, AppException):
 			return ApiResponse.internal_server_error()
 
 		return ApiResponse.error(
 			msg=e.message if hasattr(e, 'message') else str(e),
 			data=e.errors if hasattr(e, 'errors') else [],
 			err_code=e.code if hasattr(e, 'code') else 500
@@ -47,20 +48,15 @@
 
 	@staticmethod
 	def not_found(msg: str = "Resource Not Found.", **kwargs):
 		response_data = dict(success=False, message=msg, code=404, data=[])
 		return ApiResponse._dispatch(data=response_data, status=status.HTTP_404_NOT_FOUND)
 
 	@staticmethod
-	def authentication_failed(msg: str = "Authentication Failed.", **kwargs):
-		response_data = dict(success=False, message=msg, code=401, data=[])
-		return ApiResponse._dispatch(data=response_data, status=status.HTTP_401_UNAUTHORIZED)
-
-	@staticmethod
-	def forbidden(msg: str = "Access Forbidden.", **kwargs):
+	def forbidden(msg: str = "Forbidden.", **kwargs):
 		response_data = dict(success=False, message=msg, code=403, data=[])
 		return ApiResponse._dispatch(data=response_data, status=status.HTTP_403_FORBIDDEN)
 
 	@staticmethod
 	def bad_request(msg: str = "Bad Request.", **kwargs):
 		response_data = dict(success=False, message=msg, code=400, data=[])
 		return ApiResponse._dispatch(data=response_data, status=status.HTTP_400_BAD_REQUEST)
@@ -73,15 +69,7 @@
 	@staticmethod
 	def internal_server_error(msg: str = "Internal Server Error", **kwargs):
 		response_data = dict(success=False, message=msg, code=500, data=[])
 		return ApiResponse._dispatch(
 			data=response_data,
 			status=status.HTTP_500_INTERNAL_SERVER_ERROR
 		)
-
-	@staticmethod
-	def formatted_error_response(response: RestResponse) -> RestResponse:
-		_code = response.status_code or None
-		_message = response.data.get('detail') or None
-		if _code is not None and _message is not None:
-			return ApiResponse.error(err_code=_code, msg=_message.replace('"', "'"), http_code=_code)
-		return ApiResponse.internal_server_error()
```

### Comparing `hrin_msb-0.2.81/msb/logging/config.py` & `hrin_msb-0.2.9/msb_logging/_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import logging
 import os
 from datetime import datetime
 
-from msb.env import (Config)
-from .constants import (
+from ._constants import (
 	LOG_DATETIME_FORMAT, SIMPLE_LOG_FORMAT,
 	DEFAULT_FILE_HANDLER_NAME, DEFAULT_CONSOLE_HANDLER_NAME
 )
 
 
 def make_log_file_name(dir: str = '', filename: str = None):
 	filename_prefix = f"{filename}-" if filename not in ['', None] else ''
@@ -20,15 +19,15 @@
 
 	def __init__(self, **kwargs):
 		self._default_log_level = kwargs.get('default_level') or logging.WARNING
 		self._default_format_str = None
 
 	@staticmethod
 	def init_default_config(logsdir: str, default_level: str = logging.INFO, emulate_prod=False):
-
+		from msb_config import Config
 		default_log_config = LogConfig(default_level=default_level)
 
 		console_log_handler = default_log_config.get_console_handler(
 			DEFAULT_CONSOLE_HANDLER_NAME,
 			level=logging.INFO,
 		)
 
@@ -109,15 +108,15 @@
 		init_kwargs = {}
 		return self.__build_log_handler(
 			name=name, log_handler=handler_class, init_kwargs=init_kwargs,
 			level=kwargs.get('level'), formatter=kwargs.get("formatter"), filters=kwargs.get('filters')
 		)
 
 	def get_database_handler(self, name, func, **kwargs):
-		from .handlers import DatabaseLogger
+		from ._handlers import DatabaseLogger
 		init_kwargs = dict(callback_func=func)
 		return self.__build_log_handler(
 			name=name, log_handler=DatabaseLogger, init_kwargs=init_kwargs,
 			level=kwargs.get('level'), formatter=kwargs.get("formatter"), filters=kwargs.get('filters')
 		)
 
 	def __build_log_handler(self, log_handler: logging.Handler, init_kwargs: dict = None, **kwargs):
```

### Comparing `hrin_msb-0.2.81/msb/logging/constants.py` & `hrin_msb-0.2.9/msb_logging/_constants.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.81/msb/logging/handlers.py` & `hrin_msb-0.2.9/msb_logging/_handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-from .constants import (SIMPLE_LOG_FORMAT)
+from ._constants import (SIMPLE_LOG_FORMAT)
 
 
 # custom log handler that emits to the database
 class DatabaseLogger(logging.Handler):
 	__log_callback_func = None
 
 	def __init__(self, callback_func=None, *args, **kwargs):
```

### Comparing `hrin_msb-0.2.81/msb/testing/api_test.py` & `hrin_msb-0.2.9/msb_testing/api_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from os import environ
 
 from rest_framework.test import APILiveServerTestCase
 
-from .core import (TestConfig, LiveServerThreadWithReuse, const)
+from ._core import (TestConfig, LiveServerThreadWithReuse, const)
 
 
 class ApiTestResult:
 	data = None
 	message: str = ''
 	code: int = 0
 	success: bool = False
```

### Comparing `hrin_msb-0.2.81/msb/testing/core.py` & `hrin_msb-0.2.9/msb_testing/_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from os import environ, path, listdir
 
 from django.conf import settings
 from django.core.servers.basehttp import WSGIServer
 from django.test.testcases import (LiveServerThread, QuietWSGIRequestHandler)
 
-from . import constants as const
+from . import _constants as const
 
 
 class LiveServerThreadWithReuse(LiveServerThread):
 	"""
 	This miniclass overrides _create_server to allow port reuse. This avoids creating
 	"address already in use" errors for tests that have been run subsequently.
 	"""
```

### Comparing `hrin_msb-0.2.81/msb/testing/testdata.py` & `hrin_msb-0.2.9/msb_testing/testdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime
 from random import randint
 
-from msb.datetime import (DEFAULT_DATE_FORMAT, DEFAULT_TIME_FORMAT, current_date, current_timestamp)
+from msb_datetime import (DEFAULT_DATE_FORMAT, DEFAULT_TIME_FORMAT, current_date, current_timestamp)
 
 _random_names = {
 	"female": ["Olivia", "Emma", "Charlotte", "Amelia", "Ava", "Sophia", "Isabella", "Mia", ],
 	"male": ["Kai", "Zion", "Jayden", "Luca", "Ezra", "Kayden", "Quinn", "Rowan", ],
 	"surnames": ["Anand", "Laghari", "Patel", "Reddy", "Acharya", "Agarwal", "Khatri", "Ahuja", ]
 
 }
```

### Comparing `hrin_msb-0.2.81/msb/validation/__init__.py` & `hrin_msb-0.2.9/msb_validation/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,16 @@
-from .decorators import (
-	validation_schema_wrapper, api_inputs,
-	validate_inp_parameters, validate_inp_payload
-)
-from .exceptions import *
-from .rules import (DefaultRules)
-from .schema import (RuleSchema, InputField, ValidationSchema)
-from .utils import validate_against
+from ._decorators import (validation_schema_wrapper, validate_access, validate_against, validate_request_data)
+from ._exceptions import *
+from ._rules import (DefaultRules)
+from ._schema import (RuleSchema, InputField, ValidationSchema)
 
 
 class Validate:
-	raw_input = validate_against
-	request_data = api_inputs
-	params = validate_inp_parameters
-	payload = validate_inp_payload
+	raw_schema = validate_against
+	request_data = validate_request_data
+	access = validate_access
 
 
 __all__ = [
-	"api_inputs", "validate_inp_parameters", "validate_inp_payload", "validate_against",
-	"validation_schema_wrapper", "RuleSchema", "InputField", "ValidationSchema", "DefaultRules",
+	"DefaultRules", "validation_schema_wrapper", "validate_access", "validate_against", "validate_request_data",
+	"RuleSchema", "InputField", "Validate", "ValidationSchema"
 ]
```

### Comparing `hrin_msb-0.2.81/msb/validation/exceptions.py` & `hrin_msb-0.2.9/msb_validation/_exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,33 @@
-from msb.exceptions import AppException
+from msb_exceptions import AppException
 
 
-class ValidationExceptions:
+class ValidatorExceptions:
 	class InvalidValidationSchema(AppException):
 		_message = 'Validation schema should be of type ValidationSchema.'
 
-	class InvalidValidationInputDict(AppException):
-		_message = 'Validation input should be of type dict.'
-
-	class InvalidValidationInputList(AppException):
-		_message = 'Validation input should be of type list.'
+	class InvalidValidationInput(AppException):
+		_message = 'Validation input should be of type dict or list.'
 
 	class SchemaValidationFailed(AppException):
 		_message = 'Failed to validate the input against the given schema.'
 
 	class ErrorFormattingFailed(AppException):
 		_message = 'Failed to format the validation errors.'
 
 	class ValidationFailed(AppException):
 		_message = 'Failed to validate the request data.'
 
-	class InvalidPayloadException(AppException):
-		_message = 'Invalid payload recieved.'
-
-	class InvalidParamsException(AppException):
-		_message = 'Invalid request parameters recieved.'
-
-	class InvalidPayloadFormat(AppException):
-		_message = 'Malformed request data recieved.'
-
 
+class InvalidPayloadException(AppException):
+	_message = 'Invalid payload recieved.'
 
 
+class InvalidParamsException(AppException):
+	_message = 'Invalid request parameters recieved.'
 
 
+class InvalidPayloadFormat(AppException):
+	_message = 'Malformed request data recieved.'
 
 
-__all__ = ["ValidationExceptions"]
+__all__ = ["ValidatorExceptions", "InvalidParamsException", "InvalidPayloadException", "InvalidPayloadFormat"]
```

### Comparing `hrin_msb-0.2.81/msb/validation/rules.py` & `hrin_msb-0.2.9/msb_validation/_rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from .decorators import ValidationSchema
-from .schema import InputField
+from ._decorators import ValidationSchema
+from ._schema import InputField
 
 
 class DefaultRules:
 	date = InputField.Date(regex="^\d{4}\-(0?[1-9]|1[012])\-(0?[1-9]|[12][0-9]|3[01])$")
 	pk = InputField.String(required=True)
 	gender = InputField.String(allowed=['M', 'F', 'O'])
```

### Comparing `hrin_msb-0.2.81/msb/validation/schema.py` & `hrin_msb-0.2.9/msb_validation/_schema.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.81/setup.py` & `hrin_msb-0.2.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['msb',
- 'msb.apis',
- 'msb.auth',
- 'msb.cipher',
- 'msb.dataclasses',
- 'msb.datetime',
- 'msb.db',
- 'msb.devtools',
- 'msb.env',
- 'msb.exceptions',
- 'msb.files',
- 'msb.http',
- 'msb.logging',
- 'msb.services',
- 'msb.testing',
- 'msb.validation']
+['msb_apis',
+ 'msb_apis.services',
+ 'msb_apis.views',
+ 'msb_auth',
+ 'msb_auth.permissions',
+ 'msb_auth.users',
+ 'msb_auth.validators',
+ 'msb_cipher',
+ 'msb_config',
+ 'msb_const',
+ 'msb_dataclasses',
+ 'msb_datetime',
+ 'msb_db',
+ 'msb_db.models',
+ 'msb_devtools',
+ 'msb_exceptions',
+ 'msb_files',
+ 'msb_files.core',
+ 'msb_http',
+ 'msb_logging',
+ 'msb_testing',
+ 'msb_validation']
 
 package_data = \
 {'': ['*']}
 
-modules = \
-['hrin_msb']
 install_requires = \
-['celery>=5.2.7,<6.0.0',
- 'cerberus>=1.3.4,<2.0.0',
+['cerberus>=1.3.4,<2.0.0',
  'cffi>=1.15.1,<2.0.0',
  'cryptography>=38.0.3,<39.0.0',
- 'django-celery-results>=2.5.1,<3.0.0',
- 'django-cors-headers>=4.0.0,<5.0.0',
  'django>=4.1.3,<5.0.0',
  'djangorestframework-simplejwt>=5.2.2,<6.0.0',
  'djangorestframework>=3.14.0,<4.0.0',
- 'pandas>=2.0.2,<3.0.0',
+ 'pandas>=1.5.1,<2.0.0',
  'pdf2docx>=0.5.6,<0.6.0',
  'python-dateutil>=2.8.2,<3.0.0',
  'python-dotenv>=0.21.0,<0.22.0',
  'requests>=2.28.1,<3.0.0',
  'xhtml2pdf>=0.2.8,<0.3.0']
 
 setup_kwargs = {
     'name': 'hrin-msb',
-    'version': '0.2.81',
+    'version': '0.2.9',
     'description': '',
-    'long_description': '# hrin-msb\n\n## Pre-requisites for setup\n\n1. `pip install poetry`\n\n## How To Build\n\n1. `poetry build`\n2. `poetry config http-basic.pypi __token__ <access-token>`\n3. `poetry publish`\n\n# Change Log\n\n### Version 0.1.1\n\n***\n\n### Version 0.1.2\n\n***\n\n### Version 0.1.3\n\n***\n\n1. Default serializer added to ApiView\n2. fixed incorrect import in _validators.py\n3. fixed msb_database_router\n4. fixed Config.is_local_env() not working\n5. moved devscripts -> devtools\n6. File Utils Added to utils/files\n7. "app_label" removed from "TestConfig" & "ApiTest" Classes\n8. Fixed Bug : \'LoggingModelManager\' object has no attribute \'_queryset_class\'\n9. Fixed : Logging Model not showing any records\n10. Fixed : str method for base model, & removed current_timestamp method from base model\n\n***\n\n## Version 0.1.4\n\n1. Fixed : ModuleNotFoundError: No module named \'pdf2docx\'\n2. Renamed “FileGenerator“ => “FileFactory”,\n3. Add `create_` Prefix in FileFactory methods\n4. Renamed MsbMetaModel -> MsbModelMetaFields\n5. Added validation decorators, and fixed bulk validation issuses\n6. Modified Logging Configuration Files\n7. removed utils package\n8. moved msb_core.wrappers.exceptions -> msb_exceptions\n9. Fixed : Base ApiViews and Crud Routes\n10. Searchparameter class refactored, search method added in ApiService Class\n\n***\n\n## Version 0.1.41\n\n1. Fixed: Crud operations not working with encrypted id\'s\n2. Package dependencies updated\n3. Validator test cases refactored\n\n***\n\n## Version 0.1.5x\n\n### -- Version 0.1.51\n\n1. dbrouter print statement removed\n2. datetime constants renamed (added _FORMAT to all fof them)\n3. Fixed the default argument in msb_exception which was causing "DESC :" to log even if desc was none\n4. Api service create methdhod not working correctly\n5. file logging handler is not registered in local env by default, we need to pass `emulate_prod=True` to add it\n6. SearchParameter class imported in package.__init__.py\n7. Fixed : test-cases are breaking because of logs databae\n8. added base unittest class, and modified unit_test to inherit djangoTestCase instead of unittest\n9. Added Validation Schema not defined exceptions\n10. Fixed init_django_app error, int datatype instead of str while setting environement variable.\n11. Added use_django decorator to use over classes/functions\n12. Fixed : MsbMetaModel not working\n13. MsbModel meta fields accessor added\n14. Poetry dependencies updated\n15. DMY_DATE_FORMAT added\n16. versioning changed\n\n### -- Version 0.1.52\n\n1. Fixed : MsbMetaFields not working\n2. Fixed : logging model lot of exceptions are thrown if table applicationlogs is not found\n3. Fixed : logging model exceptions file not found\n4. Fixed : db_migration throwing error if no migration dire is found\n5. renamed use_djnago -> use_django, default value for settinfs_dir is added to "app"\n6. renamend _query in msb_model to db_query\n7. field_type, and label added to configuration model\n8. unique_together constraint added to ConfigurationModel\n9. class DjangoMigration creates migration folder if it doesn\'t exists\n10. Added automatic fixture loading\n11. Fixed : msb_model.__str__() was not able to read the primary key value\n12. comma removed from msbMetamodels\n13. Cipher now supports encryption/decryption of list items\n14. SearchParameter modified to supoprt autmatic filter assignment\n15. Refactor `msb_auth` : TokenUser,AuthResult,Constants added\n16. Jwt Token Validation is strict now, it allows only same owner\n\n### -- Version 0.1.521\n\n1. Fixed improper import exception\n\n### -- Version 0.1.522\n\n1. Added Login Required to base viewset\n2. Added Config Object class to msb_dataclasses\n3. Added msb_http to the package\n4. Added MsbDatabaseRouter in init.py\n5. Fixed model.delete() is not working\n\n### -- Version 0.1.611\n\n1. Modified django migration script\n2. Aded devtools to msb_ext\n3. removed `use_django` decorator & added `requires_django` decorator\n4. added default values for metafields\n5. added InputFiled.time in validation schema types\n\n### -- Version 0.2.0\n\n1. Fixed Cipher.decrypt() returning bytes instead of str\n2. Changed `SearchParameter` class implementation.\n3. default offset & limit fixed in `SearchParameter` class\n\n### -- Version 0.2.2\n\n1. default values removed from model metafields\n2. Fixed `ModuleNotFoundError: No module named \'_asymmetric_cipher\'`\n3. Fixed fixtures loaded in wrong sequence\n4. Feature `api_response.exception()` now sends back internal server error for undefined exceptions.\n5. Fixed Token validation error\n6. Added `DefaultJwtAuthSettings()` class, to unify settings across the services\n7. Added automatic fixture loading for test cases.\n\n### -- Version 0.2.3\n\n1. msb_testing refactored\n2. added new package `msb_const`\n3. Optimized imports throughout\n4. Refactored `msb_devtools`, removed `msb_ext.devtools`\n5. `msb_devtools._exceptions` file removed\n6. Added constant to `mab_auth._constants`\n\n### -- Version 0.2.4\n\n1. Refactor : (Optimized Imports,Sonarlint warnings)\n2. Refactor : Moved msb_apis.wrappers -> msb_http\n\n### -- Version 0.2.5\n\n1. Refactor : removed `msb_ext`, as it served no purpose\n2. Fixed : token validation failing due to AUD & ISS claim\n3. Added default fixture paths to `msb_const.paths`\n\n### -- Version 0.2.6\n\n1. renamed the property `db_query` to `rows`, to make it easier to understand.\n2. added a mentod to deteremine if the current environment is either dev or test env\n3. CrudActions.all is now the default parameter value for `.as_view()` method.\n4. Crud routes not working for single fields\n5. Fixed `self.seriallizer` not working with `dict()`\n6. Implemented `list` Api, to return predefined db columns\n7. search parameter added in crud, searchparameters class refatored\n\n### -- Version 0.2.7\n\n1. Fixed : `_list_field_names` not working with properties & relations\n2. Added `search_validation_rules` in DefaultRules\n\n### -- Version 0.2.8\n\n1. Fixed : list api breaking for foreign keys\n2. Fixed : Search parameter not working with fields\n3. Fixed: automatic encryption of db provate fields, now you need to put `DB_ENCRYPT_PRIVATE_FIELDS = True` to achieve that.\n\n### -- Version 0.2.9\n\n1. Fixed: automatic encryption of db primary key fields, now you need to put `DB_PK_IS_PRIVATE_FIELD = True` to achieve\n   that.\n\n### -- Version 0.2.10\n\n1. Fixed : incorrect crud routes for [list,search]\n2. Refactored : msb_http\n3. Implemented : `MsbIntraServiceRequest` class\n4. Implemented : `ApiRouter` class\n\n### -- Version 0.2.11\n\n1. Fixed /<str:id> route not working\n2. Authentication is failing due to jwt-token owner mismatch\n\n### -- Version 0.2.12\n\n1. Fixed: Payload validation is failing for DELETE and UPDATE Request\n\n### -- Version 0.2.13\n\n1. Updated : dependencies\n2. Fixed : crud list was breaking if no list fields are found/declared in model\n3. Refactored : Added _list fields in ConfigurationModel\n\n### -- Version 0.2.14\n\n1. Fixed : env_setup->db_migration requires user input to run\n\n### -- Version 0.2.15\n\n1. Fixed : Crud list api is breaking with None\n\n### -- Version 0.2.16\n\n1. Refactored : owner verification in Jwt token can now be controlled through settings.py file, using following variables"\n   `MSB_JWT_TRUSTED_OWNERS = []`(skips validation for the mentioned ip\'s) and `MSB_JWT_VERIFY_OWNER = False` (turns on/off\n   the owner verification)\n2. Implemented : `MsbIntraServiceRequest` class in msb_http\n3. Update : `ApiService` now has `resource_name` attribute in the class, this helps in better exception messages from\n   default crud operations.\n4. Refactor : `MsbIntraServiceRequest`\n5. Update : default crud api\'s now returns detailed error messages\n6. Update : All api\'s now returns detailed error messages for any exceptions.\n\n### -- Version 0.2.17\n\n1. Update : `ApiService` now automatically takes the resource name if not provided.\n2. Fixed : `MsbIntraServiceRequest` not working through api-gateway\n\n### -- Version 0.2.18\n\n1. Fixed : query parameters not working in `MsbIntraServiceRequest`\n2. Fixed : search parameter query not working in `MsbIntraServiceRequest`\n3. Fixed : limit and offset not working in list Api\n4. Refactor: _dataclasses\n5. Refactor : modified api_view error handler\n\n### -- Version 0.2.19\n\n1. removed Self parameter, due to compatibility issue\n2. Fixed : list/retrieve api bug\n\n### -- Version 0.2.2xx\n\n1. Fixed : UserRole.__init__() got an unexpected keyword argument \'access_type\'\n2. Added: recover method in model\n3. Refactor : moved all constants to `msb_constants`\n',
+    'long_description': '# hrin-msb\n\n## Pre-requisites for setup\n1. `pip install poetry`\n\n## How To Build\n\n1. `poetry build`\n2. `poetry config http-basic.pypi __token__ <access-token>`\n3. `poetry publish`\n\n\n# Change Log\n ### Version 0.1.1\n***\n\n ### Version 0.1.2\n***\n\n ### Version 0.1.3\n***\n\n1.  Default serializer added to ApiView\n2. fixed incorrect import in _validators.py\n3. fixed msb_database_router\n4. fixed Config.is_local_env() not working\n5. moved devscripts -> devtools\n6. File Utils Added to utils/files\n7. "app_label" removed from "TestConfig" & "ApiTest" Classes\n8. Fixed Bug : \'LoggingModelManager\' object has no attribute \'_queryset_class\'\n9. Fixed : Logging Model not showing any records\n10. Fixed : str method for base model, & removed current_timestamp method from base model\n***\n\n ## Version 0.1.4\n1. Fixed : ModuleNotFoundError: No module named \'pdf2docx\'\n2. Renamed “FileGenerator“ => “FileFactory”,\n3. Add `create_` Prefix in FileFactory methods\n4. Renamed MsbMetaModel -> MsbModelMetaFields\n5. Added validation decorators, and fixed bulk validation issuses\n6. Modified Logging Configuration Files\n7. removed utils package\n8. moved msb_core.wrappers.exceptions -> msb_exceptions\n9. Fixed : Base ApiViews and Crud Routes\n10. Searchparameter class refactored, search method added in ApiService Class\n***\n\n## Version 0.1.41\n1. Fixed: Crud operations not working with encrypted id\'s\n2. Package dependencies updated\n3. Validator test cases refactored\n***\n## Version 0.1.5x\n ### -- Version 0.1.51\n1. dbrouter print statement removed\n2. datetime constants renamed (added _FORMAT to all fof them)\n3. Fixed the default argument in msb_exception  which was causing "DESC :" to log even if desc was none\n4. Api service create methdhod not working correctly\n5. file logging handler is not registered in local env by default, we need to pass `emulate_prod=True` to add it \n6. SearchParameter class imported in package.__init__.py \n7. Fixed : test-cases are breaking because of logs databae\n8. added base unittest class, and modified unit_test to inherit djangoTestCase instead of unittest\n9. Added Validation Schema not defined exceptions\n10. Fixed init_django_app error, int datatype instead of str while setting environement variable.\n11. Added use_django decorator to use over classes/functions\n12. Fixed : MsbMetaModel not working\n13. MsbModel meta fields accessor added\n14. Poetry dependencies updated\n15. DMY_DATE_FORMAT added\n16. versioning changed\n\n  ### -- Version 0.1.52\n1. Fixed : MsbMetaFields not working \n2. Fixed : logging model lot of exceptions are thrown if table applicationlogs is not found\n3. Fixed : logging model exceptions file not found\n4. Fixed : db_migration throwing error if no migration dire is found\n5. renamed use_djnago -> use_django, default value for settinfs_dir is added to "app"\n6. renamend _query in msb_model to db_query\n7. field_type, and label added to configuration model\n8. unique_together constraint added to ConfigurationModel\n9. class DjangoMigration creates migration folder if it doesn\'t exists\n10. Added automatic fixture loading\n11. Fixed : msb_model.__str__() was not able to read the primary key value \n12. comma removed from msbMetamodels\n13. Cipher now supports encryption/decryption of list items \n14. SearchParameter modified to supoprt autmatic filter assignment \n15. Refactor `msb_auth` : TokenUser,AuthResult,Constants added\n16. Jwt Token Validation is strict now, it allows only same owner\n  \n### -- Version 0.1.521\n1. Fixed improper import exception\n\n  \n### -- Version 0.1.522\n1. Added Login Required to base viewset\n2. Added Config Object class to msb_dataclasses \n3. Added msb_http to the package\n4. Added MsbDatabaseRouter in init.py\n5. Fixed model.delete() is not working\n\n### -- Version 0.1.611\n1. Modified django migration script\n2. Aded devtools to msb_ext\n3. removed `use_django` decorator & added `requires_django` decorator\n4. added default values for metafields\n5. added InputFiled.time in validation schema types\n\n\n### -- Version 0.2.0\n1. Fixed Cipher.decrypt() returning bytes instead of str\n2. Changed `SearchParameter` class implementation.\n3. default offset & limit fixed in `SearchParameter` class\n\n### -- Version 0.2.2\n1. default values removed from model metafields\n2. Fixed `ModuleNotFoundError: No module named \'_asymmetric_cipher\'`\n3. Fixed fixtures loaded in wrong sequence\n4. Feature `api_response.exception()` now sends back internal server error for undefined exceptions.\n5. Fixed Token validation error\n6. Added `DefaultJwtAuthSettings()` class, to unify settings across the services\n7. Added automatic fixture loading for test cases.\n\n\n### -- Version 0.2.3\n1. msb_testing refactored \n2. added new package `msb_const`\n3. Optimized imports throughout\n4. Refactored `msb_devtools`, removed `msb_ext.devtools`\n5. `msb_devtools._exceptions` file removed\n6. Added constant to `mab_auth._constants`\n\n### -- Version 0.2.4\n1. Refactor : (Optimized Imports,Sonarlint warnings)\n2. Refactor : Moved msb_apis.wrappers -> msb_http\n\n### -- Version 0.2.5\n1. Refactor : removed `msb_ext`, as it served no purpose\n2. Fixed : token validation failing due to AUD & ISS claim\n3. Added default fixture paths to `msb_const.paths`\n\n### -- Version 0.2.6\n1. renamed the property `db_query` to `rows`, to make it easier to understand.\n2. added a mentod to deteremine if the current environment is either dev or test env\n3. CrudActions.all is now the default parameter value for `.as_view()` method.\n4. Crud routes not working for single fields\n5. Fixed `self.seriallizer` not working with `dict()`\n6. Implemented `list` Api, to return predefined db columns \n7. search parameter added in crud, searchparameters class refatored\n\n### -- Version 0.2.7\n1. Fixed : `_list_field_names` not working with properties & relations \n2. Added `search_validation_rules` in DefaultRules\n\n### -- Version 0.2.8\n1. Fixed : list api breaking for foreign keys\n2. Fixed : Search parameter not working with fields\n3. Fixed: automatic encryption of db provate fields, now you need to put `DB_ENCRYPT_PRIVATE_FIELDS = True` to achieve that.\n\n### -- Version 0.2.9\n1. Fixed: automatic encryption of db primary key fields, now you need to put `DB_PK_IS_PRIVATE_FIELD = True` to achieve \n   that.',
     'author': 'Prakash Mishra',
     'author_email': 'prakash.mishra@intimetec.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
-    'py_modules': modules,
     'install_requires': install_requires,
     'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `hrin_msb-0.2.81/PKG-INFO` & `hrin_msb-0.2.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,277 +1,185 @@
 Metadata-Version: 2.1
 Name: hrin-msb
-Version: 0.2.81
+Version: 0.2.9
 Summary: 
 Author: Prakash Mishra
 Author-email: prakash.mishra@intimetec.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: celery (>=5.2.7,<6.0.0)
 Requires-Dist: cerberus (>=1.3.4,<2.0.0)
 Requires-Dist: cffi (>=1.15.1,<2.0.0)
 Requires-Dist: cryptography (>=38.0.3,<39.0.0)
 Requires-Dist: django (>=4.1.3,<5.0.0)
-Requires-Dist: django-celery-results (>=2.5.1,<3.0.0)
-Requires-Dist: django-cors-headers (>=4.0.0,<5.0.0)
 Requires-Dist: djangorestframework (>=3.14.0,<4.0.0)
 Requires-Dist: djangorestframework-simplejwt (>=5.2.2,<6.0.0)
-Requires-Dist: pandas (>=2.0.2,<3.0.0)
+Requires-Dist: pandas (>=1.5.1,<2.0.0)
 Requires-Dist: pdf2docx (>=0.5.6,<0.6.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: xhtml2pdf (>=0.2.8,<0.3.0)
 Description-Content-Type: text/markdown
 
 # hrin-msb
 
 ## Pre-requisites for setup
-
 1. `pip install poetry`
 
 ## How To Build
 
 1. `poetry build`
 2. `poetry config http-basic.pypi __token__ <access-token>`
 3. `poetry publish`
 
-# Change Log
-
-### Version 0.1.1
 
+# Change Log
+ ### Version 0.1.1
 ***
 
-### Version 0.1.2
-
+ ### Version 0.1.2
 ***
 
-### Version 0.1.3
-
+ ### Version 0.1.3
 ***
 
-1. Default serializer added to ApiView
+1.  Default serializer added to ApiView
 2. fixed incorrect import in _validators.py
 3. fixed msb_database_router
 4. fixed Config.is_local_env() not working
 5. moved devscripts -> devtools
 6. File Utils Added to utils/files
 7. "app_label" removed from "TestConfig" & "ApiTest" Classes
 8. Fixed Bug : 'LoggingModelManager' object has no attribute '_queryset_class'
 9. Fixed : Logging Model not showing any records
 10. Fixed : str method for base model, & removed current_timestamp method from base model
-
 ***
 
-## Version 0.1.4
-
+ ## Version 0.1.4
 1. Fixed : ModuleNotFoundError: No module named 'pdf2docx'
 2. Renamed “FileGenerator“ => “FileFactory”,
 3. Add `create_` Prefix in FileFactory methods
 4. Renamed MsbMetaModel -> MsbModelMetaFields
 5. Added validation decorators, and fixed bulk validation issuses
 6. Modified Logging Configuration Files
 7. removed utils package
 8. moved msb_core.wrappers.exceptions -> msb_exceptions
 9. Fixed : Base ApiViews and Crud Routes
 10. Searchparameter class refactored, search method added in ApiService Class
-
 ***
 
 ## Version 0.1.41
-
 1. Fixed: Crud operations not working with encrypted id's
 2. Package dependencies updated
 3. Validator test cases refactored
-
 ***
-
 ## Version 0.1.5x
-
-### -- Version 0.1.51
-
+ ### -- Version 0.1.51
 1. dbrouter print statement removed
 2. datetime constants renamed (added _FORMAT to all fof them)
-3. Fixed the default argument in msb_exception which was causing "DESC :" to log even if desc was none
+3. Fixed the default argument in msb_exception  which was causing "DESC :" to log even if desc was none
 4. Api service create methdhod not working correctly
-5. file logging handler is not registered in local env by default, we need to pass `emulate_prod=True` to add it
-6. SearchParameter class imported in package.__init__.py
+5. file logging handler is not registered in local env by default, we need to pass `emulate_prod=True` to add it 
+6. SearchParameter class imported in package.__init__.py 
 7. Fixed : test-cases are breaking because of logs databae
 8. added base unittest class, and modified unit_test to inherit djangoTestCase instead of unittest
 9. Added Validation Schema not defined exceptions
 10. Fixed init_django_app error, int datatype instead of str while setting environement variable.
 11. Added use_django decorator to use over classes/functions
 12. Fixed : MsbMetaModel not working
 13. MsbModel meta fields accessor added
 14. Poetry dependencies updated
 15. DMY_DATE_FORMAT added
 16. versioning changed
 
-### -- Version 0.1.52
-
-1. Fixed : MsbMetaFields not working
+  ### -- Version 0.1.52
+1. Fixed : MsbMetaFields not working 
 2. Fixed : logging model lot of exceptions are thrown if table applicationlogs is not found
 3. Fixed : logging model exceptions file not found
 4. Fixed : db_migration throwing error if no migration dire is found
 5. renamed use_djnago -> use_django, default value for settinfs_dir is added to "app"
 6. renamend _query in msb_model to db_query
 7. field_type, and label added to configuration model
 8. unique_together constraint added to ConfigurationModel
 9. class DjangoMigration creates migration folder if it doesn't exists
 10. Added automatic fixture loading
-11. Fixed : msb_model.__str__() was not able to read the primary key value
+11. Fixed : msb_model.__str__() was not able to read the primary key value 
 12. comma removed from msbMetamodels
-13. Cipher now supports encryption/decryption of list items
-14. SearchParameter modified to supoprt autmatic filter assignment
+13. Cipher now supports encryption/decryption of list items 
+14. SearchParameter modified to supoprt autmatic filter assignment 
 15. Refactor `msb_auth` : TokenUser,AuthResult,Constants added
 16. Jwt Token Validation is strict now, it allows only same owner
-
+  
 ### -- Version 0.1.521
-
 1. Fixed improper import exception
 
+  
 ### -- Version 0.1.522
-
 1. Added Login Required to base viewset
-2. Added Config Object class to msb_dataclasses
+2. Added Config Object class to msb_dataclasses 
 3. Added msb_http to the package
 4. Added MsbDatabaseRouter in init.py
 5. Fixed model.delete() is not working
 
 ### -- Version 0.1.611
-
 1. Modified django migration script
 2. Aded devtools to msb_ext
 3. removed `use_django` decorator & added `requires_django` decorator
 4. added default values for metafields
 5. added InputFiled.time in validation schema types
 
-### -- Version 0.2.0
 
+### -- Version 0.2.0
 1. Fixed Cipher.decrypt() returning bytes instead of str
 2. Changed `SearchParameter` class implementation.
 3. default offset & limit fixed in `SearchParameter` class
 
 ### -- Version 0.2.2
-
 1. default values removed from model metafields
 2. Fixed `ModuleNotFoundError: No module named '_asymmetric_cipher'`
 3. Fixed fixtures loaded in wrong sequence
 4. Feature `api_response.exception()` now sends back internal server error for undefined exceptions.
 5. Fixed Token validation error
 6. Added `DefaultJwtAuthSettings()` class, to unify settings across the services
 7. Added automatic fixture loading for test cases.
 
-### -- Version 0.2.3
 
-1. msb_testing refactored
+### -- Version 0.2.3
+1. msb_testing refactored 
 2. added new package `msb_const`
 3. Optimized imports throughout
 4. Refactored `msb_devtools`, removed `msb_ext.devtools`
 5. `msb_devtools._exceptions` file removed
 6. Added constant to `mab_auth._constants`
 
 ### -- Version 0.2.4
-
 1. Refactor : (Optimized Imports,Sonarlint warnings)
 2. Refactor : Moved msb_apis.wrappers -> msb_http
 
 ### -- Version 0.2.5
-
 1. Refactor : removed `msb_ext`, as it served no purpose
 2. Fixed : token validation failing due to AUD & ISS claim
 3. Added default fixture paths to `msb_const.paths`
 
 ### -- Version 0.2.6
-
 1. renamed the property `db_query` to `rows`, to make it easier to understand.
 2. added a mentod to deteremine if the current environment is either dev or test env
 3. CrudActions.all is now the default parameter value for `.as_view()` method.
 4. Crud routes not working for single fields
 5. Fixed `self.seriallizer` not working with `dict()`
-6. Implemented `list` Api, to return predefined db columns
+6. Implemented `list` Api, to return predefined db columns 
 7. search parameter added in crud, searchparameters class refatored
 
 ### -- Version 0.2.7
-
-1. Fixed : `_list_field_names` not working with properties & relations
+1. Fixed : `_list_field_names` not working with properties & relations 
 2. Added `search_validation_rules` in DefaultRules
 
 ### -- Version 0.2.8
-
 1. Fixed : list api breaking for foreign keys
 2. Fixed : Search parameter not working with fields
 3. Fixed: automatic encryption of db provate fields, now you need to put `DB_ENCRYPT_PRIVATE_FIELDS = True` to achieve that.
 
 ### -- Version 0.2.9
-
-1. Fixed: automatic encryption of db primary key fields, now you need to put `DB_PK_IS_PRIVATE_FIELD = True` to achieve
+1. Fixed: automatic encryption of db primary key fields, now you need to put `DB_PK_IS_PRIVATE_FIELD = True` to achieve 
    that.
-
-### -- Version 0.2.10
-
-1. Fixed : incorrect crud routes for [list,search]
-2. Refactored : msb_http
-3. Implemented : `MsbIntraServiceRequest` class
-4. Implemented : `ApiRouter` class
-
-### -- Version 0.2.11
-
-1. Fixed /<str:id> route not working
-2. Authentication is failing due to jwt-token owner mismatch
-
-### -- Version 0.2.12
-
-1. Fixed: Payload validation is failing for DELETE and UPDATE Request
-
-### -- Version 0.2.13
-
-1. Updated : dependencies
-2. Fixed : crud list was breaking if no list fields are found/declared in model
-3. Refactored : Added _list fields in ConfigurationModel
-
-### -- Version 0.2.14
-
-1. Fixed : env_setup->db_migration requires user input to run
-
-### -- Version 0.2.15
-
-1. Fixed : Crud list api is breaking with None
-
-### -- Version 0.2.16
-
-1. Refactored : owner verification in Jwt token can now be controlled through settings.py file, using following variables"
-   `MSB_JWT_TRUSTED_OWNERS = []`(skips validation for the mentioned ip's) and `MSB_JWT_VERIFY_OWNER = False` (turns on/off
-   the owner verification)
-2. Implemented : `MsbIntraServiceRequest` class in msb_http
-3. Update : `ApiService` now has `resource_name` attribute in the class, this helps in better exception messages from
-   default crud operations.
-4. Refactor : `MsbIntraServiceRequest`
-5. Update : default crud api's now returns detailed error messages
-6. Update : All api's now returns detailed error messages for any exceptions.
-
-### -- Version 0.2.17
-
-1. Update : `ApiService` now automatically takes the resource name if not provided.
-2. Fixed : `MsbIntraServiceRequest` not working through api-gateway
-
-### -- Version 0.2.18
-
-1. Fixed : query parameters not working in `MsbIntraServiceRequest`
-2. Fixed : search parameter query not working in `MsbIntraServiceRequest`
-3. Fixed : limit and offset not working in list Api
-4. Refactor: _dataclasses
-5. Refactor : modified api_view error handler
-
-### -- Version 0.2.19
-
-1. removed Self parameter, due to compatibility issue
-2. Fixed : list/retrieve api bug
-
-### -- Version 0.2.2xx
-
-1. Fixed : UserRole.__init__() got an unexpected keyword argument 'access_type'
-2. Added: recover method in model
-3. Refactor : moved all constants to `msb_constants`
-
```

