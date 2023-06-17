# Comparing `tmp/strawberry_django_plus-3.0.0.tar.gz` & `tmp/strawberry_django_plus-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_django_plus-3.0.0.tar", max compression
+gzip compressed data, was "strawberry_django_plus-3.0.1.tar", max compression
```

## Comparing `strawberry_django_plus-3.0.0.tar` & `strawberry_django_plus-3.0.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1094 2023-06-15 22:48:01.093610 strawberry_django_plus-3.0.0/LICENSE
--rw-r--r--   0        0        0     3354 2023-06-15 22:48:01.093610 strawberry_django_plus-3.0.0/README.md
--rw-r--r--   0        0        0     4208 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     3001 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/__init__.py
--rw-r--r--   0        0        0     5649 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/descriptors.py
--rw-r--r--   0        0        0     5752 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/directives.py
--rw-r--r--   0        0        0    28702 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/field.py
--rw-r--r--   0        0        0     3033 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/filters.py
--rw-r--r--   0        0        0     1556 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/gql/__init__.py
--rw-r--r--   0        0        0     1515 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/gql/django.py
--rw-r--r--   0        0        0        0 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/integrations/__init__.py
--rw-r--r--   0        0        0     1939 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/integrations/guardian.py
--rw-r--r--   0        0        0        0 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/management/commands/__init__.py
--rw-r--r--   0        0        0     1168 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/management/commands/export_schema.py
--rw-r--r--   0        0        0        0 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/middlewares/__init__.py
--rw-r--r--   0        0        0      896 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/middlewares/user_warmup.py
--rw-r--r--   0        0        0        0 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/mutations/__init__.py
--rw-r--r--   0        0        0    23947 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/mutations/fields.py
--rw-r--r--   0        0        0    14791 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/mutations/resolvers.py
--rw-r--r--   0        0        0    26439 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/optimizer.py
--rw-r--r--   0        0        0     1340 2023-06-15 22:48:01.101610 strawberry_django_plus-3.0.0/strawberry_django_plus/ordering.py
--rw-r--r--   0        0        0    28085 2023-06-15 22:48:01.101610 strawberry_django_plus-3.0.0/strawberry_django_plus/permissions.py
--rw-r--r--   0        0        0        0 2023-06-15 22:48:01.101610 strawberry_django_plus-3.0.0/strawberry_django_plus/py.typed
--rw-r--r--   0        0        0     2532 2023-06-15 22:48:01.101610 strawberry_django_plus-3.0.0/strawberry_django_plus/relay.py
--rw-r--r--   0        0        0     1027 2023-06-15 22:48:01.101610 strawberry_django_plus-3.0.0/strawberry_django_plus/settings.py
--rw-r--r--   0        0        0        0 2023-06-15 22:48:01.101610 strawberry_django_plus-3.0.0/strawberry_django_plus/test/__init__.py
--rw-r--r--   0        0        0     2408 2023-06-15 22:48:01.101610 strawberry_django_plus-3.0.0/strawberry_django_plus/test/client.py
--rw-r--r--   0        0        0    16382 2023-06-15 22:48:01.101610 strawberry_django_plus-3.0.0/strawberry_django_plus/type.py
--rw-r--r--   0        0        0     9889 2023-06-15 22:48:01.101610 strawberry_django_plus-3.0.0/strawberry_django_plus/types.py
--rw-r--r--   0        0        0        0 2023-06-15 22:48:01.101610 strawberry_django_plus-3.0.0/strawberry_django_plus/utils/__init__.py
--rw-r--r--   0        0        0     6916 2023-06-15 22:48:01.101610 strawberry_django_plus-3.0.0/strawberry_django_plus/utils/aio.py
--rw-r--r--   0        0        0    13223 2023-06-15 22:48:01.101610 strawberry_django_plus-3.0.0/strawberry_django_plus/utils/inspect.py
--rw-r--r--   0        0        0     1077 2023-06-15 22:48:01.101610 strawberry_django_plus-3.0.0/strawberry_django_plus/utils/pyutils.py
--rw-r--r--   0        0        0     5865 2023-06-15 22:48:01.101610 strawberry_django_plus-3.0.0/strawberry_django_plus/utils/query.py
--rw-r--r--   0        0        0    16244 2023-06-15 22:48:01.101610 strawberry_django_plus-3.0.0/strawberry_django_plus/utils/resolvers.py
--rw-r--r--   0        0        0      938 2023-06-15 22:48:01.101610 strawberry_django_plus-3.0.0/strawberry_django_plus/utils/typing.py
--rw-r--r--   0        0        0     4875 1970-01-01 00:00:00.000000 strawberry_django_plus-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-06-17 17:55:21.212398 strawberry_django_plus-3.0.1/LICENSE
+-rw-r--r--   0        0        0     3354 2023-06-17 17:55:21.212398 strawberry_django_plus-3.0.1/README.md
+-rw-r--r--   0        0        0     4208 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3001 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/strawberry_django_plus/__init__.py
+-rw-r--r--   0        0        0     5649 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/strawberry_django_plus/descriptors.py
+-rw-r--r--   0        0        0     5752 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/strawberry_django_plus/directives.py
+-rw-r--r--   0        0        0    29442 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/strawberry_django_plus/field.py
+-rw-r--r--   0        0        0     3033 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/strawberry_django_plus/filters.py
+-rw-r--r--   0        0        0     1556 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/strawberry_django_plus/gql/__init__.py
+-rw-r--r--   0        0        0     1515 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/strawberry_django_plus/gql/django.py
+-rw-r--r--   0        0        0        0 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/strawberry_django_plus/integrations/__init__.py
+-rw-r--r--   0        0        0     1939 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/strawberry_django_plus/integrations/guardian.py
+-rw-r--r--   0        0        0        0 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/strawberry_django_plus/management/commands/__init__.py
+-rw-r--r--   0        0        0     1168 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/strawberry_django_plus/management/commands/export_schema.py
+-rw-r--r--   0        0        0        0 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/strawberry_django_plus/middlewares/__init__.py
+-rw-r--r--   0        0        0      896 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/strawberry_django_plus/middlewares/user_warmup.py
+-rw-r--r--   0        0        0        0 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/strawberry_django_plus/mutations/__init__.py
+-rw-r--r--   0        0        0    24104 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/strawberry_django_plus/mutations/fields.py
+-rw-r--r--   0        0        0    14791 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/strawberry_django_plus/mutations/resolvers.py
+-rw-r--r--   0        0        0    26439 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/optimizer.py
+-rw-r--r--   0        0        0     1340 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/ordering.py
+-rw-r--r--   0        0        0    28085 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/permissions.py
+-rw-r--r--   0        0        0        0 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/py.typed
+-rw-r--r--   0        0        0     2532 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/relay.py
+-rw-r--r--   0        0        0     1027 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/settings.py
+-rw-r--r--   0        0        0        0 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/test/__init__.py
+-rw-r--r--   0        0        0     2408 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/test/client.py
+-rw-r--r--   0        0        0    16382 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/type.py
+-rw-r--r--   0        0        0     9889 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/types.py
+-rw-r--r--   0        0        0        0 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/utils/__init__.py
+-rw-r--r--   0        0        0     6916 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/utils/aio.py
+-rw-r--r--   0        0        0    13223 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/utils/inspect.py
+-rw-r--r--   0        0        0     1077 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/utils/pyutils.py
+-rw-r--r--   0        0        0     5865 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/utils/query.py
+-rw-r--r--   0        0        0    16244 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/utils/resolvers.py
+-rw-r--r--   0        0        0      938 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/utils/typing.py
+-rw-r--r--   0        0        0     4875 1970-01-01 00:00:00.000000 strawberry_django_plus-3.0.1/PKG-INFO
```

### Comparing `strawberry_django_plus-3.0.0/LICENSE` & `strawberry_django_plus-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.0/README.md` & `strawberry_django_plus-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.0/pyproject.toml` & `strawberry_django_plus-3.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strawberry-django-plus"
-version = "3.0.0"
+version = "3.0.1"
 description = "Enhanced Strawberry GraphQL integration with Django"
 authors = ["Thiago Bellini Ribeiro <thiago@bellini.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/blb-ventures/strawberry-django-plus"
 repository = "https://github.com/blb-ventures/strawberry-django-plus"
 documentation = "https://strawberry-django-plus.readthedocs.io"
```

### Comparing `strawberry_django_plus-3.0.0/strawberry_django_plus/__init__.py` & `strawberry_django_plus-3.0.1/strawberry_django_plus/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 _original_process_type = object_type._process_type
 _original_wrap_dataclass = object_type._wrap_dataclass
 _original_field_init = StrawberryField.__init__
 _original_field_call = StrawberryField.__call__
 _original_enum_init = EnumDefinition.__init__
 _original_from_generic = NameConverter.from_generic
 
-__version__ = "3.0.0"  # x-release-please-version
+__version__ = "3.0.1"  # x-release-please-version
 
 
 def _get_doc(obj):
     if not obj.__doc__:
         return None
     return inspect.cleandoc(obj.__doc__)
```

### Comparing `strawberry_django_plus-3.0.0/strawberry_django_plus/descriptors.py` & `strawberry_django_plus-3.0.1/strawberry_django_plus/descriptors.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.0/strawberry_django_plus/directives.py` & `strawberry_django_plus-3.0.1/strawberry_django_plus/directives.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.0/strawberry_django_plus/field.py` & `strawberry_django_plus-3.0.1/strawberry_django_plus/field.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     TypeVar,
     Union,
     cast,
     overload,
 )
 
 import strawberry
+from django.core.exceptions import ObjectDoesNotExist
 from django.db import models
 from django.db.models import QuerySet
 from django.db.models.fields.related_descriptors import (
     ForwardManyToOneDescriptor,
     ReverseManyToOneDescriptor,
     ReverseOneToOneDescriptor,
 )
@@ -148,31 +149,31 @@
         super(StrawberryDjangoField, self.__class__).type.fset(self, type_)  # type: ignore
 
     def get_order(self) -> Optional[Type]:
         # FIXME: This should be done on strawberry-graphql-django
         order = super().get_order()
         if order in (None, UNSET):
             t_origin = self.type_origin
-            if (f_origin := getattr(t_origin, "_django_type", None)) is not None:
+            if t_origin and (f_origin := getattr(t_origin, "_django_type", None)) is not None:
                 order = f_origin.order
 
-        return order
+        return order if order is not UNSET else None
 
     def get_filters(self) -> Optional[Type]:
         # FIXME: This should be done on strawberry-graphql-django
         filters = super().get_filters()
         if filters in (None, UNSET):
             t_origin = self.type_origin
-            if (f_origin := getattr(t_origin, "_django_type", None)) is not None:
+            if t_origin and (f_origin := getattr(t_origin, "_django_type", None)) is not None:
                 filters = f_origin.filters
 
-        return filters
+        return filters if filters is not UNSET else None
 
     @cached_property
-    def type_origin(self) -> Type:
+    def type_origin(self) -> Optional[Type]:
         origin = self.type
 
         tdef = cast(Optional[TypeDefinition], getattr(origin, "_type_definition", None))
         if tdef and tdef.concrete_of and issubclass(tdef.concrete_of.origin, relay.Connection):
             origin = tdef.type_var_map[relay.NodeType]  # type: ignore
             if isinstance(origin, LazyType):
                 origin = origin.resolve_type()
@@ -185,22 +186,21 @@
             for t in origin.types:
                 while isinstance(t, StrawberryContainer):
                     t = t.of_type  # noqa: PLW2901
 
                 if hasattr(t, "_django_type"):
                     olist.append(t)
 
-            assert len(olist) == 1
-            origin = olist[0]
+            origin = olist[0] if len(olist) == 1 else None
 
         return origin
 
     @cached_property
-    def model(self) -> Type[models.Model]:
-        return self.type_origin._django_type.model
+    def model(self) -> Optional[Type[models.Model]]:
+        return (type_origin := self.type_origin) and type_origin._django_type.model
 
     @cached_property
     def safe_resolver(self):
         resolver = self.base_resolver
         assert resolver
         if not resolver.is_async:
             return resolvers.async_safe(resolver)
@@ -215,15 +215,17 @@
         kwargs: Dict[str, Any],
         *,
         skip_base_resolver: bool = False,
     ) -> Union[Awaitable[Any], Any]:
         if not skip_base_resolver and self.base_resolver is not None:
             result = self.resolver(source, info, args, kwargs)
         elif source is None:
-            result = self.model._default_manager.all()
+            model = self.model
+            assert model is not None
+            result = model._default_manager.all()
         else:
             # Small optimization to async resolvers avoid having to call it in an sync_to_async
             # context if the value is already cached, since it will not hit the db anymore
             attname = self.django_name or self.python_name
             attr = getattr(source.__class__, attname, None)
             try:
                 if isinstance(attr, ModelProperty):
@@ -323,50 +325,61 @@
         try:
             qs = self.get_queryset(qs, info, **kwargs)
             if not self.base_resolver:
                 node = kwargs.get("id")
                 if isinstance(node, relay.GlobalID):
                     assert node.resolve_type(info) == unwrap_type(self.type)
                     qs = qs.filter(pk=node.node_id)
-        except self.model.DoesNotExist:
+        except ObjectDoesNotExist:
             if not self.is_optional:
                 raise
         else:
             return qs.get()
 
         return None
 
 
 class StrawberryDjangoConnectionExtension(relay.ConnectionExtension):
     def apply(self, field: StrawberryDjangoField) -> None:
         # NOTE: Because we have a base_resolver defined, our parents will not add
         # order/filters resolvers in here, so we need to add them by hand (unless they
         # are somewhat in there). We are not adding pagination because it doesn't make
         # sense together with a Connection
-        args_names = {a.python_name for a in field.arguments}
+        args: Dict[str, StrawberryArgument] = {a.python_name: a for a in field.arguments}
 
-        if "filters" not in args_names and (filters := field.get_filters()) not in (None, UNSET):
-            field.arguments = [*field.arguments, argument("filters", filters)]
-        if "order" not in args_names and (order := field.get_order()) not in (None, UNSET):
-            field.arguments = [*field.arguments, argument("order", order)]
+        if "filters" not in args and (filters := field.get_filters()) not in (None, UNSET):
+            args["filters"] = argument("filters", filters)
+        if "order" not in args and (order := field.get_order()) not in (None, UNSET):
+            args["order"] = argument("order", order)
+
+        field.arguments = list(args.values())
 
         if field.base_resolver is None:
 
             def default_resolver(
                 root: Optional[models.Model],
                 info: Info,
                 **kwargs: Any,
             ) -> Iterable[Any]:
                 if root is not None:
                     # If this is a nested field, call get_result instead because we want
                     # to retrieve the queryset from its RelatedManager
                     retval = field.get_result(root, info, [], kwargs, skip_base_resolver=True)
                 else:
+                    if (type_origin := field.type_origin) is None:
+                        raise TypeError(
+                            (
+                                "Django connection without a resolver needs to define a connection "
+                                "for one and only one django type. To use it in a union, define "
+                                "your own resolver that handles each of those"
+                            ),
+                        )
+
                     retval = resolvers.resolve_model_nodes(
-                        field.type_origin,
+                        type_origin,
                         info=info,
                         required=True,
                         filter_perms=True,
                     )
 
                 # If the type defines a custom get_queryset, use it on top of the returned queryset
                 if (get_queryset := getattr(field.type_origin, "get_queryset", None)) is not None:
```

### Comparing `strawberry_django_plus-3.0.0/strawberry_django_plus/filters.py` & `strawberry_django_plus-3.0.1/strawberry_django_plus/filters.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.0/strawberry_django_plus/gql/__init__.py` & `strawberry_django_plus-3.0.1/strawberry_django_plus/gql/__init__.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.0/strawberry_django_plus/gql/django.py` & `strawberry_django_plus-3.0.1/strawberry_django_plus/gql/django.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.0/strawberry_django_plus/integrations/guardian.py` & `strawberry_django_plus-3.0.1/strawberry_django_plus/integrations/guardian.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.0/strawberry_django_plus/management/commands/export_schema.py` & `strawberry_django_plus-3.0.1/strawberry_django_plus/management/commands/export_schema.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.0/strawberry_django_plus/middlewares/user_warmup.py` & `strawberry_django_plus-3.0.1/strawberry_django_plus/middlewares/user_warmup.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.0/strawberry_django_plus/mutations/fields.py` & `strawberry_django_plus-3.0.1/strawberry_django_plus/mutations/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,20 +227,24 @@
         source: Any,
         info: Info,
         data: object,
         args: List[Any],
         kwargs: Dict[str, Any],
     ) -> Any:
         assert data is not None
+
+        model = self.model
+        assert model is not None
+
         # Do not optimize anything while retrieving the object to update
         token = DjangoOptimizerExtension.enabled.set(False)
         try:
             retval = resolvers.create(
                 info,
-                self.model,
+                model,
                 resolvers.parse_input(info, vars(data)),
                 full_clean=self.full_clean,
             )
         finally:
             DjangoOptimizerExtension.enabled.reset(token)
 
         return retval
@@ -266,18 +270,21 @@
         assert data is not None
 
         vdata = vars(data)
         pk = vdata.pop("id", UNSET)
         if pk is UNSET:
             pk = vdata.pop("pk")
 
+        model = self.model
+        assert model
+
         # Do not optimize anything while retrieving the object to update
         token = DjangoOptimizerExtension.enabled.set(False)
         try:
-            instance = get_with_perms(pk, info, required=True, model=self.model)
+            instance = get_with_perms(pk, info, required=True, model=model)
             retval = resolvers.update(
                 info,
                 instance,
                 resolvers.parse_input(info, vdata),
                 full_clean=self.full_clean,
             )
         finally:
@@ -306,18 +313,21 @@
         assert data is not None
 
         vdata = vars(data)
         pk = vdata.pop("id", UNSET)
         if pk is UNSET:
             pk = vdata.pop("pk")
 
+        model = self.model
+        assert model is not None
+
         # Do not optimize anything while retrieving the object to delete
         token = DjangoOptimizerExtension.enabled.set(False)
         try:
-            instance = get_with_perms(pk, info, required=True, model=self.model)
+            instance = get_with_perms(pk, info, required=True, model=model)
             retval = resolvers.delete(info, instance, data=resolvers.parse_input(info, vdata))
         finally:
             DjangoOptimizerExtension.enabled.reset(token)
 
         return retval
```

### Comparing `strawberry_django_plus-3.0.0/strawberry_django_plus/mutations/resolvers.py` & `strawberry_django_plus-3.0.1/strawberry_django_plus/mutations/resolvers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.0/strawberry_django_plus/optimizer.py` & `strawberry_django_plus-3.0.1/strawberry_django_plus/optimizer.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.0/strawberry_django_plus/ordering.py` & `strawberry_django_plus-3.0.1/strawberry_django_plus/ordering.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.0/strawberry_django_plus/permissions.py` & `strawberry_django_plus-3.0.1/strawberry_django_plus/permissions.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.0/strawberry_django_plus/relay.py` & `strawberry_django_plus-3.0.1/strawberry_django_plus/relay.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.0/strawberry_django_plus/settings.py` & `strawberry_django_plus-3.0.1/strawberry_django_plus/settings.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.0/strawberry_django_plus/test/client.py` & `strawberry_django_plus-3.0.1/strawberry_django_plus/test/client.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.0/strawberry_django_plus/type.py` & `strawberry_django_plus-3.0.1/strawberry_django_plus/type.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.0/strawberry_django_plus/types.py` & `strawberry_django_plus-3.0.1/strawberry_django_plus/types.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.0/strawberry_django_plus/utils/aio.py` & `strawberry_django_plus-3.0.1/strawberry_django_plus/utils/aio.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.0/strawberry_django_plus/utils/inspect.py` & `strawberry_django_plus-3.0.1/strawberry_django_plus/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.0/strawberry_django_plus/utils/pyutils.py` & `strawberry_django_plus-3.0.1/strawberry_django_plus/utils/pyutils.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.0/strawberry_django_plus/utils/query.py` & `strawberry_django_plus-3.0.1/strawberry_django_plus/utils/query.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.0/strawberry_django_plus/utils/resolvers.py` & `strawberry_django_plus-3.0.1/strawberry_django_plus/utils/resolvers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.0/strawberry_django_plus/utils/typing.py` & `strawberry_django_plus-3.0.1/strawberry_django_plus/utils/typing.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.0/PKG-INFO` & `strawberry_django_plus-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-django-plus
-Version: 3.0.0
+Version: 3.0.1
 Summary: Enhanced Strawberry GraphQL integration with Django
 Home-page: https://github.com/blb-ventures/strawberry-django-plus
 License: MIT
 Keywords: strawberry,django,graphql,relay,optimizer
 Author: Thiago Bellini Ribeiro
 Author-email: thiago@bellini.dev
 Requires-Python: >=3.8,<4.0
```

