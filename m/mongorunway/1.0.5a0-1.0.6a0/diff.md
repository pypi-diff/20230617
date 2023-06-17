# Comparing `tmp/mongorunway-1.0.5a0.tar.gz` & `tmp/mongorunway-1.0.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongorunway-1.0.5a0.tar", max compression
+gzip compressed data, was "mongorunway-1.0.6a0.tar", max compression
```

## Comparing `mongorunway-1.0.5a0.tar` & `mongorunway-1.0.6a0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0   114798 2023-05-16 15:05:04.927930 mongorunway-1.0.5a0/assets/logo.jpg
--rw-r--r--   0        0        0     1083 2023-04-30 10:29:59.339256 mongorunway-1.0.5a0/LICENSE
--rw-r--r--   0        0        0     2141 2023-06-12 15:17:38.242879 mongorunway-1.0.5a0/mongorunway/__init__.py
--rw-r--r--   0        0        0    10084 2023-06-10 15:04:53.374709 mongorunway-1.0.5a0/mongorunway/api.py
--rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.634932 mongorunway-1.0.5a0/mongorunway/application/__init__.py
--rw-r--r--   0        0        0    16117 2023-06-12 12:11:31.173474 mongorunway-1.0.5a0/mongorunway/application/applications.py
--rw-r--r--   0        0        0     4711 2023-06-12 12:11:31.188916 mongorunway-1.0.5a0/mongorunway/application/config.py
--rw-r--r--   0        0        0     6627 2023-06-12 15:17:35.125378 mongorunway-1.0.5a0/mongorunway/application/event_manager.py
--rw-r--r--   0        0        0     1869 2023-06-10 22:12:16.143444 mongorunway-1.0.5a0/mongorunway/application/filesystem.py
--rw-r--r--   0        0        0     3754 2023-06-10 22:12:16.090515 mongorunway-1.0.5a0/mongorunway/application/output.py
--rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.653020 mongorunway-1.0.5a0/mongorunway/application/ports/__init__.py
--rw-r--r--   0        0        0     2367 2023-05-29 13:10:46.336291 mongorunway-1.0.5a0/mongorunway/application/ports/auditlog_journal.py
--rw-r--r--   0        0        0     1668 2023-06-03 08:16:22.923990 mongorunway-1.0.5a0/mongorunway/application/ports/config_reader.py
--rw-r--r--   0        0        0     1533 2023-05-29 12:25:19.814965 mongorunway-1.0.5a0/mongorunway/application/ports/filename_strategy.py
--rw-r--r--   0        0        0     3015 2023-06-03 06:50:09.695978 mongorunway-1.0.5a0/mongorunway/application/ports/repository.py
--rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.628311 mongorunway-1.0.5a0/mongorunway/application/services/__init__.py
--rw-r--r--   0        0        0     1583 2023-06-03 08:43:33.409655 mongorunway-1.0.5a0/mongorunway/application/services/checksum_service.py
--rw-r--r--   0        0        0     6885 2023-06-10 18:23:19.406553 mongorunway-1.0.5a0/mongorunway/application/services/migration_service.py
--rw-r--r--   0        0        0     2265 2023-06-10 22:12:16.130759 mongorunway-1.0.5a0/mongorunway/application/services/status_service.py
--rw-r--r--   0        0        0     3223 2023-06-03 08:55:00.830346 mongorunway-1.0.5a0/mongorunway/application/services/validation_service.py
--rw-r--r--   0        0        0     1537 2023-05-29 15:33:37.946295 mongorunway-1.0.5a0/mongorunway/application/services/versioning_service.py
--rw-r--r--   0        0        0    17817 2023-06-12 12:12:18.392506 mongorunway-1.0.5a0/mongorunway/application/session.py
--rw-r--r--   0        0        0     2744 2023-06-10 22:12:16.025624 mongorunway-1.0.5a0/mongorunway/application/traits.py
--rw-r--r--   0        0        0     8668 2023-06-11 20:46:29.271952 mongorunway-1.0.5a0/mongorunway/application/transactions.py
--rw-r--r--   0        0        0    17308 2023-06-12 15:17:38.292466 mongorunway-1.0.5a0/mongorunway/application/use_cases.py
--rw-r--r--   0        0        0    10438 2023-06-10 21:57:50.790123 mongorunway-1.0.5a0/mongorunway/application/ux.py
--rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.667525 mongorunway-1.0.5a0/mongorunway/domain/__init__.py
--rw-r--r--   0        0        0     5087 2023-06-03 08:42:10.654208 mongorunway-1.0.5a0/mongorunway/domain/migration.py
--rw-r--r--   0        0        0     2915 2023-06-12 15:17:35.044297 mongorunway-1.0.5a0/mongorunway/domain/migration_auditlog_entry.py
--rw-r--r--   0        0        0     2739 2023-06-02 07:43:28.451121 mongorunway-1.0.5a0/mongorunway/domain/migration_business_module.py
--rw-r--r--   0        0        0     2635 2023-06-03 08:55:00.817659 mongorunway-1.0.5a0/mongorunway/domain/migration_business_rule.py
--rw-r--r--   0        0        0     1882 2023-06-03 08:41:58.635457 mongorunway-1.0.5a0/mongorunway/domain/migration_command.py
--rw-r--r--   0        0        0     1550 2023-06-10 22:12:16.038377 mongorunway-1.0.5a0/mongorunway/domain/migration_context.py
--rw-r--r--   0        0        0     2676 2023-06-12 09:02:48.786949 mongorunway-1.0.5a0/mongorunway/domain/migration_event.py
--rw-r--r--   0        0        0     3382 2023-06-12 15:17:35.081376 mongorunway-1.0.5a0/mongorunway/domain/migration_event_manager.py
--rw-r--r--   0        0        0     3596 2023-06-12 15:17:35.083879 mongorunway-1.0.5a0/mongorunway/domain/migration_exception.py
--rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.622090 mongorunway-1.0.5a0/mongorunway/infrastructure/__init__.py
--rw-r--r--   0        0        0    18145 2023-06-04 06:30:35.981777 mongorunway-1.0.5a0/mongorunway/infrastructure/commands.py
--rw-r--r--   0        0        0    13641 2023-06-12 15:17:35.213969 mongorunway-1.0.5a0/mongorunway/infrastructure/config_readers.py
--rw-r--r--   0        0        0     4114 2023-06-10 21:42:09.715186 mongorunway-1.0.5a0/mongorunway/infrastructure/event_handlers.py
--rw-r--r--   0        0        0     2806 2023-06-10 13:40:29.075274 mongorunway-1.0.5a0/mongorunway/infrastructure/filename_strategies.py
--rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.659732 mongorunway-1.0.5a0/mongorunway/infrastructure/persistence/__init__.py
--rw-r--r--   0        0        0     4546 2023-06-12 13:59:52.705479 mongorunway-1.0.5a0/mongorunway/infrastructure/persistence/auditlog_journals.py
--rw-r--r--   0        0        0     6466 2023-06-12 15:17:35.142513 mongorunway-1.0.5a0/mongorunway/infrastructure/persistence/repositories.py
--rw-r--r--   0        0        0     2874 2023-06-03 08:55:23.935731 mongorunway-1.0.5a0/mongorunway/mongo.py
--rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.640253 mongorunway-1.0.5a0/mongorunway/presentation/__init__.py
--rw-r--r--   0        0        0    18347 2023-06-12 15:17:35.257219 mongorunway-1.0.5a0/mongorunway/presentation/cli.py
--rw-r--r--   0        0        0     2324 2023-06-03 08:16:23.398941 mongorunway-1.0.5a0/mongorunway/presentation/formatters.py
--rw-r--r--   0        0        0     4028 2023-06-12 11:04:18.371307 mongorunway-1.0.5a0/mongorunway/presentation/presenters.py
--rw-r--r--   0        0        0    17162 2023-06-11 20:46:29.255224 mongorunway-1.0.5a0/mongorunway/util.py
--rw-r--r--   0        0        0     4589 2023-06-10 15:17:56.501111 mongorunway-1.0.5a0/PYPI_README.md
--rw-r--r--   0        0        0     2307 2023-06-13 16:31:19.827186 mongorunway-1.0.5a0/pyproject.toml
--rw-r--r--   0        0        0     5938 1970-01-01 00:00:00.000000 mongorunway-1.0.5a0/PKG-INFO
+-rw-r--r--   0        0        0   114798 2023-05-16 15:05:04.927930 mongorunway-1.0.6a0/assets/logo.jpg
+-rw-r--r--   0        0        0     1083 2023-04-30 10:29:59.339256 mongorunway-1.0.6a0/LICENSE
+-rw-r--r--   0        0        0     2141 2023-06-12 15:17:38.242879 mongorunway-1.0.6a0/mongorunway/__init__.py
+-rw-r--r--   0        0        0    10084 2023-06-10 15:04:53.374709 mongorunway-1.0.6a0/mongorunway/api.py
+-rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.634932 mongorunway-1.0.6a0/mongorunway/application/__init__.py
+-rw-r--r--   0        0        0    16430 2023-06-17 09:35:36.421923 mongorunway-1.0.6a0/mongorunway/application/applications.py
+-rw-r--r--   0        0        0     4711 2023-06-12 12:11:31.188916 mongorunway-1.0.6a0/mongorunway/application/config.py
+-rw-r--r--   0        0        0     6627 2023-06-12 15:17:35.125378 mongorunway-1.0.6a0/mongorunway/application/event_manager.py
+-rw-r--r--   0        0        0     1869 2023-06-10 22:12:16.143444 mongorunway-1.0.6a0/mongorunway/application/filesystem.py
+-rw-r--r--   0        0        0     3754 2023-06-10 22:12:16.090515 mongorunway-1.0.6a0/mongorunway/application/output.py
+-rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.653020 mongorunway-1.0.6a0/mongorunway/application/ports/__init__.py
+-rw-r--r--   0        0        0     2367 2023-05-29 13:10:46.336291 mongorunway-1.0.6a0/mongorunway/application/ports/auditlog_journal.py
+-rw-r--r--   0        0        0     1668 2023-06-03 08:16:22.923990 mongorunway-1.0.6a0/mongorunway/application/ports/config_reader.py
+-rw-r--r--   0        0        0     1533 2023-05-29 12:25:19.814965 mongorunway-1.0.6a0/mongorunway/application/ports/filename_strategy.py
+-rw-r--r--   0        0        0     3015 2023-06-03 06:50:09.695978 mongorunway-1.0.6a0/mongorunway/application/ports/repository.py
+-rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.628311 mongorunway-1.0.6a0/mongorunway/application/services/__init__.py
+-rw-r--r--   0        0        0     1583 2023-06-03 08:43:33.409655 mongorunway-1.0.6a0/mongorunway/application/services/checksum_service.py
+-rw-r--r--   0        0        0     6885 2023-06-10 18:23:19.406553 mongorunway-1.0.6a0/mongorunway/application/services/migration_service.py
+-rw-r--r--   0        0        0     2265 2023-06-10 22:12:16.130759 mongorunway-1.0.6a0/mongorunway/application/services/status_service.py
+-rw-r--r--   0        0        0     3223 2023-06-03 08:55:00.830346 mongorunway-1.0.6a0/mongorunway/application/services/validation_service.py
+-rw-r--r--   0        0        0     1537 2023-05-29 15:33:37.946295 mongorunway-1.0.6a0/mongorunway/application/services/versioning_service.py
+-rw-r--r--   0        0        0    17817 2023-06-12 12:12:18.392506 mongorunway-1.0.6a0/mongorunway/application/session.py
+-rw-r--r--   0        0        0     2744 2023-06-10 22:12:16.025624 mongorunway-1.0.6a0/mongorunway/application/traits.py
+-rw-r--r--   0        0        0     8668 2023-06-11 20:46:29.271952 mongorunway-1.0.6a0/mongorunway/application/transactions.py
+-rw-r--r--   0        0        0    17308 2023-06-12 15:17:38.292466 mongorunway-1.0.6a0/mongorunway/application/use_cases.py
+-rw-r--r--   0        0        0    10438 2023-06-10 21:57:50.790123 mongorunway-1.0.6a0/mongorunway/application/ux.py
+-rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.667525 mongorunway-1.0.6a0/mongorunway/domain/__init__.py
+-rw-r--r--   0        0        0     5087 2023-06-03 08:42:10.654208 mongorunway-1.0.6a0/mongorunway/domain/migration.py
+-rw-r--r--   0        0        0     2915 2023-06-12 15:17:35.044297 mongorunway-1.0.6a0/mongorunway/domain/migration_auditlog_entry.py
+-rw-r--r--   0        0        0     2739 2023-06-02 07:43:28.451121 mongorunway-1.0.6a0/mongorunway/domain/migration_business_module.py
+-rw-r--r--   0        0        0     2635 2023-06-03 08:55:00.817659 mongorunway-1.0.6a0/mongorunway/domain/migration_business_rule.py
+-rw-r--r--   0        0        0     1882 2023-06-03 08:41:58.635457 mongorunway-1.0.6a0/mongorunway/domain/migration_command.py
+-rw-r--r--   0        0        0     1550 2023-06-10 22:12:16.038377 mongorunway-1.0.6a0/mongorunway/domain/migration_context.py
+-rw-r--r--   0        0        0     2676 2023-06-12 09:02:48.786949 mongorunway-1.0.6a0/mongorunway/domain/migration_event.py
+-rw-r--r--   0        0        0     3382 2023-06-12 15:17:35.081376 mongorunway-1.0.6a0/mongorunway/domain/migration_event_manager.py
+-rw-r--r--   0        0        0     3596 2023-06-12 15:17:35.083879 mongorunway-1.0.6a0/mongorunway/domain/migration_exception.py
+-rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.622090 mongorunway-1.0.6a0/mongorunway/infrastructure/__init__.py
+-rw-r--r--   0        0        0    18145 2023-06-04 06:30:35.981777 mongorunway-1.0.6a0/mongorunway/infrastructure/commands.py
+-rw-r--r--   0        0        0    13641 2023-06-12 15:17:35.213969 mongorunway-1.0.6a0/mongorunway/infrastructure/config_readers.py
+-rw-r--r--   0        0        0     4114 2023-06-10 21:42:09.715186 mongorunway-1.0.6a0/mongorunway/infrastructure/event_handlers.py
+-rw-r--r--   0        0        0     2806 2023-06-10 13:40:29.075274 mongorunway-1.0.6a0/mongorunway/infrastructure/filename_strategies.py
+-rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.659732 mongorunway-1.0.6a0/mongorunway/infrastructure/persistence/__init__.py
+-rw-r--r--   0        0        0     4546 2023-06-12 13:59:52.705479 mongorunway-1.0.6a0/mongorunway/infrastructure/persistence/auditlog_journals.py
+-rw-r--r--   0        0        0     6466 2023-06-12 15:17:35.142513 mongorunway-1.0.6a0/mongorunway/infrastructure/persistence/repositories.py
+-rw-r--r--   0        0        0     2874 2023-06-03 08:55:23.935731 mongorunway-1.0.6a0/mongorunway/mongo.py
+-rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.640253 mongorunway-1.0.6a0/mongorunway/presentation/__init__.py
+-rw-r--r--   0        0        0    18347 2023-06-12 15:17:35.257219 mongorunway-1.0.6a0/mongorunway/presentation/cli.py
+-rw-r--r--   0        0        0     2324 2023-06-03 08:16:23.398941 mongorunway-1.0.6a0/mongorunway/presentation/formatters.py
+-rw-r--r--   0        0        0     4028 2023-06-12 11:04:18.371307 mongorunway-1.0.6a0/mongorunway/presentation/presenters.py
+-rw-r--r--   0        0        0    17162 2023-06-11 20:46:29.255224 mongorunway-1.0.6a0/mongorunway/util.py
+-rw-r--r--   0        0        0     4589 2023-06-10 15:17:56.501111 mongorunway-1.0.6a0/PYPI_README.md
+-rw-r--r--   0        0        0     2307 2023-06-17 10:00:24.426704 mongorunway-1.0.6a0/pyproject.toml
+-rw-r--r--   0        0        0     5938 1970-01-01 00:00:00.000000 mongorunway-1.0.6a0/PKG-INFO
```

### Comparing `mongorunway-1.0.5a0/assets/logo.jpg` & `mongorunway-1.0.6a0/assets/logo.jpg`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/LICENSE` & `mongorunway-1.0.6a0/LICENSE`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/__init__.py` & `mongorunway-1.0.6a0/mongorunway/__init__.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/api.py` & `mongorunway-1.0.6a0/mongorunway/api.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/application/__init__.py` & `mongorunway-1.0.6a0/mongorunway/application/__init__.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/application/applications.py` & `mongorunway-1.0.6a0/mongorunway/application/applications.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     "MigrationApp",
     "MigrationAppImpl",
 )
 
 import abc
 import functools
 import logging
+import operator
 import typing
 
 import typing_extensions
 
 from mongorunway.application import event_manager
 from mongorunway.application import session
 from mongorunway.application import traits
@@ -330,15 +331,19 @@
                 return transactions.TRANSACTION_SUCCESS
 
     @requires_migrations(is_applied=False)
     def upgrade_while(
         self, predicate: typing.Callable[[domain_migration.Migration], bool], /
     ) -> int:
         upgraded = 0
-        pending_migration_models = self._session.get_migration_models_by_flag(is_applied=False)
+        pending_migration_models = list(
+            self._session.get_migration_models_by_flag(is_applied=False)
+        )
+        pending_migration_models.sort(key=operator.attrgetter("version"))
+        print(len(pending_migration_models), pending_migration_models)
 
         with self._session.begin_mongo_session() as session_context:
             while pending_migration_models:
                 migration = self._migration_service.get_migration(
                     (model := pending_migration_models.pop(0)).name,
                     model.version,
                 )
@@ -369,15 +374,18 @@
             return upgraded
 
     @requires_migrations(is_applied=True)
     def downgrade_while(
         self, predicate: typing.Callable[[domain_migration.Migration], bool], /
     ) -> int:
         downgraded = 0
-        applied_migration_models = self._session.get_migration_models_by_flag(is_applied=True)
+        applied_migration_models = list(
+            self._session.get_migration_models_by_flag(is_applied=True)
+        )
+        applied_migration_models.sort(key=operator.attrgetter("version"), reverse=True)
 
         with self._session.begin_mongo_session() as session_context:
             while applied_migration_models:
                 migration = self._migration_service.get_migration(
                     (model := applied_migration_models.pop(0)).name,
                     model.version,
                 )
```

### Comparing `mongorunway-1.0.5a0/mongorunway/application/config.py` & `mongorunway-1.0.6a0/mongorunway/application/config.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/application/event_manager.py` & `mongorunway-1.0.6a0/mongorunway/application/event_manager.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/application/filesystem.py` & `mongorunway-1.0.6a0/mongorunway/application/filesystem.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/application/output.py` & `mongorunway-1.0.6a0/mongorunway/application/output.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/application/ports/__init__.py` & `mongorunway-1.0.6a0/mongorunway/application/ports/__init__.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/application/ports/auditlog_journal.py` & `mongorunway-1.0.6a0/mongorunway/application/ports/auditlog_journal.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/application/ports/config_reader.py` & `mongorunway-1.0.6a0/mongorunway/application/ports/config_reader.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/application/ports/filename_strategy.py` & `mongorunway-1.0.6a0/mongorunway/application/ports/filename_strategy.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/application/ports/repository.py` & `mongorunway-1.0.6a0/mongorunway/application/ports/repository.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/application/services/__init__.py` & `mongorunway-1.0.6a0/mongorunway/application/services/__init__.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/application/services/checksum_service.py` & `mongorunway-1.0.6a0/mongorunway/application/services/checksum_service.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/application/services/migration_service.py` & `mongorunway-1.0.6a0/mongorunway/application/services/migration_service.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/application/services/status_service.py` & `mongorunway-1.0.6a0/mongorunway/application/services/status_service.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/application/services/validation_service.py` & `mongorunway-1.0.6a0/mongorunway/application/services/validation_service.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/application/services/versioning_service.py` & `mongorunway-1.0.6a0/mongorunway/application/services/versioning_service.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/application/session.py` & `mongorunway-1.0.6a0/mongorunway/application/session.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/application/traits.py` & `mongorunway-1.0.6a0/mongorunway/application/traits.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/application/transactions.py` & `mongorunway-1.0.6a0/mongorunway/application/transactions.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/application/use_cases.py` & `mongorunway-1.0.6a0/mongorunway/application/use_cases.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/application/ux.py` & `mongorunway-1.0.6a0/mongorunway/application/ux.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/domain/__init__.py` & `mongorunway-1.0.6a0/mongorunway/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/domain/migration.py` & `mongorunway-1.0.6a0/mongorunway/domain/migration.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/domain/migration_auditlog_entry.py` & `mongorunway-1.0.6a0/mongorunway/domain/migration_auditlog_entry.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/domain/migration_business_module.py` & `mongorunway-1.0.6a0/mongorunway/domain/migration_business_module.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/domain/migration_business_rule.py` & `mongorunway-1.0.6a0/mongorunway/domain/migration_business_rule.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/domain/migration_command.py` & `mongorunway-1.0.6a0/mongorunway/domain/migration_command.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/domain/migration_context.py` & `mongorunway-1.0.6a0/mongorunway/domain/migration_context.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/domain/migration_event.py` & `mongorunway-1.0.6a0/mongorunway/domain/migration_event.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/domain/migration_event_manager.py` & `mongorunway-1.0.6a0/mongorunway/domain/migration_event_manager.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/domain/migration_exception.py` & `mongorunway-1.0.6a0/mongorunway/domain/migration_exception.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/infrastructure/__init__.py` & `mongorunway-1.0.6a0/mongorunway/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/infrastructure/commands.py` & `mongorunway-1.0.6a0/mongorunway/infrastructure/commands.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/infrastructure/config_readers.py` & `mongorunway-1.0.6a0/mongorunway/infrastructure/config_readers.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/infrastructure/event_handlers.py` & `mongorunway-1.0.6a0/mongorunway/infrastructure/event_handlers.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/infrastructure/filename_strategies.py` & `mongorunway-1.0.6a0/mongorunway/infrastructure/filename_strategies.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/infrastructure/persistence/__init__.py` & `mongorunway-1.0.6a0/mongorunway/infrastructure/persistence/__init__.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/infrastructure/persistence/auditlog_journals.py` & `mongorunway-1.0.6a0/mongorunway/infrastructure/persistence/auditlog_journals.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/infrastructure/persistence/repositories.py` & `mongorunway-1.0.6a0/mongorunway/infrastructure/persistence/repositories.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/mongo.py` & `mongorunway-1.0.6a0/mongorunway/mongo.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/presentation/__init__.py` & `mongorunway-1.0.6a0/mongorunway/presentation/__init__.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/presentation/cli.py` & `mongorunway-1.0.6a0/mongorunway/presentation/cli.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/presentation/formatters.py` & `mongorunway-1.0.6a0/mongorunway/presentation/formatters.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/presentation/presenters.py` & `mongorunway-1.0.6a0/mongorunway/presentation/presenters.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/mongorunway/util.py` & `mongorunway-1.0.6a0/mongorunway/util.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/PYPI_README.md` & `mongorunway-1.0.6a0/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.5a0/pyproject.toml` & `mongorunway-1.0.6a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 [tool.black]
 line-length = 99
 target-version = ["py39"]
 
 [tool.poetry]
 name = "mongorunway"
-version = "1.0.5a"
+version = "1.0.6a"
 description = "A MongoDB migration tool."
 authors = ["Animatea <animatea.programming@gmail.com>"]
 readme = "PYPI_README.md"
 license = "MIT"
 homepage = "https://github.com/Animatea/mongorunway"
 repository = "https://github.com/Animatea/mongorunway"
 documentation = "https://animatea.github.io/mongorunway/"
```

### Comparing `mongorunway-1.0.5a0/PKG-INFO` & `mongorunway-1.0.6a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongorunway
-Version: 1.0.5a0
+Version: 1.0.6a0
 Summary: A MongoDB migration tool.
 Home-page: https://github.com/Animatea/mongorunway
 License: MIT
 Keywords: migration,mongodb,mongo,mongorunway
 Author: Animatea
 Author-email: animatea.programming@gmail.com
 Requires-Python: >=3.9,<4.0
```

