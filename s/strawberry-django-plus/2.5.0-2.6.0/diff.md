# Comparing `tmp/strawberry_django_plus-2.5.0.tar.gz` & `tmp/strawberry_django_plus-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_django_plus-2.5.0.tar", max compression
+gzip compressed data, was "strawberry_django_plus-2.6.0.tar", max compression
```

## Comparing `strawberry_django_plus-2.5.0.tar` & `strawberry_django_plus-2.6.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0     1094 2023-05-29 19:12:42.096095 strawberry_django_plus-2.5.0/LICENSE
--rw-r--r--   0        0        0     3299 2023-05-29 19:12:42.096095 strawberry_django_plus-2.5.0/README.md
--rw-r--r--   0        0        0     4290 2023-05-29 19:12:42.096095 strawberry_django_plus-2.5.0/pyproject.toml
--rw-r--r--   0        0        0     3001 2023-05-29 19:12:42.096095 strawberry_django_plus-2.5.0/strawberry_django_plus/__init__.py
--rw-r--r--   0        0        0     5562 2023-05-29 19:12:42.096095 strawberry_django_plus-2.5.0/strawberry_django_plus/descriptors.py
--rw-r--r--   0        0        0     5751 2023-05-29 19:12:42.096095 strawberry_django_plus-2.5.0/strawberry_django_plus/directives.py
--rw-r--r--   0        0        0    26052 2023-05-29 19:12:42.096095 strawberry_django_plus-2.5.0/strawberry_django_plus/field.py
--rw-r--r--   0        0        0     3069 2023-05-29 19:12:42.096095 strawberry_django_plus-2.5.0/strawberry_django_plus/filters.py
--rw-r--r--   0        0        0     1657 2023-05-29 19:12:42.096095 strawberry_django_plus-2.5.0/strawberry_django_plus/gql/__init__.py
--rw-r--r--   0        0        0     1389 2023-05-29 19:12:42.096095 strawberry_django_plus-2.5.0/strawberry_django_plus/gql/django.py
--rw-r--r--   0        0        0        0 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/integrations/__init__.py
--rw-r--r--   0        0        0     1939 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/integrations/guardian.py
--rw-r--r--   0        0        0        0 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/management/commands/__init__.py
--rw-r--r--   0        0        0     1168 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/management/commands/export_schema.py
--rw-r--r--   0        0        0        0 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/middlewares/__init__.py
--rw-r--r--   0        0        0     6304 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/middlewares/debug_toolbar.py
--rw-r--r--   0        0        0        0 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/mutations/__init__.py
--rw-r--r--   0        0        0    25062 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/mutations/fields.py
--rw-r--r--   0        0        0    14825 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/mutations/resolvers.py
--rw-r--r--   0        0        0    26108 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/optimizer.py
--rw-r--r--   0        0        0     1372 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/ordering.py
--rw-r--r--   0        0        0    27526 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/permissions.py
--rw-r--r--   0        0        0        0 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/py.typed
--rw-r--r--   0        0        0    47560 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/relay.py
--rw-r--r--   0        0        0     1107 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/settings.py
--rw-r--r--   0        0        0     1445 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html
--rw-r--r--   0        0        0        0 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/test/__init__.py
--rw-r--r--   0        0        0     2337 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/test/client.py
--rw-r--r--   0        0        0    18301 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/type.py
--rw-r--r--   0        0        0    10174 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/types.py
--rw-r--r--   0        0        0        0 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/utils/__init__.py
--rw-r--r--   0        0        0     6916 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/utils/aio.py
--rw-r--r--   0        0        0    13069 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/utils/inspect.py
--rw-r--r--   0        0        0     1077 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/utils/pyutils.py
--rw-r--r--   0        0        0     5865 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/utils/query.py
--rw-r--r--   0        0        0    13142 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/utils/resolvers.py
--rw-r--r--   0        0        0      938 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/utils/typing.py
--rw-r--r--   0        0        0     4919 1970-01-01 00:00:00.000000 strawberry_django_plus-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-06-01 15:39:56.763017 strawberry_django_plus-2.6.0/LICENSE
+-rw-r--r--   0        0        0     3299 2023-06-01 15:39:56.763017 strawberry_django_plus-2.6.0/README.md
+-rw-r--r--   0        0        0     4309 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3001 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/__init__.py
+-rw-r--r--   0        0        0     5562 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/descriptors.py
+-rw-r--r--   0        0        0     5751 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/directives.py
+-rw-r--r--   0        0        0    26052 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/field.py
+-rw-r--r--   0        0        0     3069 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/filters.py
+-rw-r--r--   0        0        0     1657 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/gql/__init__.py
+-rw-r--r--   0        0        0     1389 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/gql/django.py
+-rw-r--r--   0        0        0        0 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/integrations/__init__.py
+-rw-r--r--   0        0        0     1939 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/integrations/guardian.py
+-rw-r--r--   0        0        0        0 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/management/commands/__init__.py
+-rw-r--r--   0        0        0     1168 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/management/commands/export_schema.py
+-rw-r--r--   0        0        0        0 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/middlewares/__init__.py
+-rw-r--r--   0        0        0     6304 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/middlewares/debug_toolbar.py
+-rw-r--r--   0        0        0      896 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/middlewares/user_warmup.py
+-rw-r--r--   0        0        0        0 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/mutations/__init__.py
+-rw-r--r--   0        0        0    25062 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/mutations/fields.py
+-rw-r--r--   0        0        0    14825 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/mutations/resolvers.py
+-rw-r--r--   0        0        0    26108 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/optimizer.py
+-rw-r--r--   0        0        0     1372 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/ordering.py
+-rw-r--r--   0        0        0    27526 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/permissions.py
+-rw-r--r--   0        0        0        0 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/py.typed
+-rw-r--r--   0        0        0    47560 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/relay.py
+-rw-r--r--   0        0        0     1107 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/settings.py
+-rw-r--r--   0        0        0     1445 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html
+-rw-r--r--   0        0        0        0 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/test/__init__.py
+-rw-r--r--   0        0        0     2337 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/test/client.py
+-rw-r--r--   0        0        0    18702 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/type.py
+-rw-r--r--   0        0        0    10297 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/types.py
+-rw-r--r--   0        0        0        0 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/utils/__init__.py
+-rw-r--r--   0        0        0     6916 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/utils/aio.py
+-rw-r--r--   0        0        0    13069 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/utils/inspect.py
+-rw-r--r--   0        0        0     1077 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/utils/pyutils.py
+-rw-r--r--   0        0        0     5865 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/utils/query.py
+-rw-r--r--   0        0        0    13142 2023-06-01 15:39:56.771016 strawberry_django_plus-2.6.0/strawberry_django_plus/utils/resolvers.py
+-rw-r--r--   0        0        0      938 2023-06-01 15:39:56.771016 strawberry_django_plus-2.6.0/strawberry_django_plus/utils/typing.py
+-rw-r--r--   0        0        0     4919 1970-01-01 00:00:00.000000 strawberry_django_plus-2.6.0/PKG-INFO
```

### Comparing `strawberry_django_plus-2.5.0/LICENSE` & `strawberry_django_plus-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.5.0/README.md` & `strawberry_django_plus-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.5.0/pyproject.toml` & `strawberry_django_plus-2.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strawberry-django-plus"
-version = "2.5.0"
+version = "2.6.0"
 description = "Enhanced Strawberry GraphQL integration with Django"
 authors = ["Thiago Bellini Ribeiro <thiago@bellini.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/blb-ventures/strawberry-django-plus"
 repository = "https://github.com/blb-ventures/strawberry-django-plus"
 documentation = "https://strawberry-django-plus.readthedocs.io"
@@ -56,14 +56,15 @@
 mkdocs = "^1.4.2"
 mkdocs-markdownextradata-plugin = "^0.2.5"
 mkdocs-material = "^9.0.9"
 mkdocs-minify-plugin = "^0.6.2"
 pymdown-extensions = ">=9.5,<11.0"
 Markdown = "^3.3.7"
 ruff = "^0.0.270"
+debugpy = "^1.6.7"
 
 
 [tool.poetry.extras]
 enum = ["django-choices-field"]
 debug-toolbar = ["django-debug-toolbar"]
 
 [tool.ruff]
```

### Comparing `strawberry_django_plus-2.5.0/strawberry_django_plus/__init__.py` & `strawberry_django_plus-2.6.0/strawberry_django_plus/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 _original_process_type = object_type._process_type
 _original_wrap_dataclass = object_type._wrap_dataclass
 _original_field_init = StrawberryField.__init__
 _original_field_call = StrawberryField.__call__
 _original_enum_init = EnumDefinition.__init__
 _original_from_generic = NameConverter.from_generic
 
-__version__ = "2.5.0"  # x-release-please-version
+__version__ = "2.6.0"  # x-release-please-version
 
 
 def _get_doc(obj):
     if not obj.__doc__:
         return None
     return inspect.cleandoc(obj.__doc__)
```

### Comparing `strawberry_django_plus-2.5.0/strawberry_django_plus/descriptors.py` & `strawberry_django_plus-2.6.0/strawberry_django_plus/descriptors.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.5.0/strawberry_django_plus/directives.py` & `strawberry_django_plus-2.6.0/strawberry_django_plus/directives.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.5.0/strawberry_django_plus/field.py` & `strawberry_django_plus-2.6.0/strawberry_django_plus/field.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.5.0/strawberry_django_plus/filters.py` & `strawberry_django_plus-2.6.0/strawberry_django_plus/filters.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.5.0/strawberry_django_plus/gql/__init__.py` & `strawberry_django_plus-2.6.0/strawberry_django_plus/gql/__init__.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.5.0/strawberry_django_plus/gql/django.py` & `strawberry_django_plus-2.6.0/strawberry_django_plus/gql/django.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.5.0/strawberry_django_plus/integrations/guardian.py` & `strawberry_django_plus-2.6.0/strawberry_django_plus/integrations/guardian.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.5.0/strawberry_django_plus/management/commands/export_schema.py` & `strawberry_django_plus-2.6.0/strawberry_django_plus/management/commands/export_schema.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.5.0/strawberry_django_plus/middlewares/debug_toolbar.py` & `strawberry_django_plus-2.6.0/strawberry_django_plus/middlewares/debug_toolbar.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.5.0/strawberry_django_plus/mutations/fields.py` & `strawberry_django_plus-2.6.0/strawberry_django_plus/mutations/fields.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.5.0/strawberry_django_plus/mutations/resolvers.py` & `strawberry_django_plus-2.6.0/strawberry_django_plus/mutations/resolvers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.5.0/strawberry_django_plus/optimizer.py` & `strawberry_django_plus-2.6.0/strawberry_django_plus/optimizer.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.5.0/strawberry_django_plus/ordering.py` & `strawberry_django_plus-2.6.0/strawberry_django_plus/ordering.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.5.0/strawberry_django_plus/permissions.py` & `strawberry_django_plus-2.6.0/strawberry_django_plus/permissions.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.5.0/strawberry_django_plus/relay.py` & `strawberry_django_plus-2.6.0/strawberry_django_plus/relay.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.5.0/strawberry_django_plus/settings.py` & `strawberry_django_plus-2.6.0/strawberry_django_plus/settings.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.5.0/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html` & `strawberry_django_plus-2.6.0/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.5.0/strawberry_django_plus/test/client.py` & `strawberry_django_plus-2.6.0/strawberry_django_plus/test/client.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.5.0/strawberry_django_plus/type.py` & `strawberry_django_plus-2.6.0/strawberry_django_plus/type.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,17 +23,18 @@
 from django.db.models.base import Model
 from django.db.models.fields.reverse_related import ManyToManyRel, ManyToOneRel
 from strawberry import UNSET
 from strawberry.annotation import StrawberryAnnotation
 from strawberry.exceptions import MissingFieldAnnotationError, PrivateStrawberryFieldError
 from strawberry.field import UNRESOLVED, StrawberryField
 from strawberry.private import is_private
+from strawberry.types import Info
 from strawberry.types.fields.resolver import StrawberryResolver
 from strawberry.unset import UnsetType
-from strawberry.utils.typing import __dataclass_transform__
+from strawberry.utils.typing import __dataclass_transform__, eval_type
 from strawberry_django.fields.field import field as _field
 from strawberry_django.fields.types import get_model_field, resolve_model_field_name
 from strawberry_django.type import StrawberryDjangoType as _StraberryDjangoType
 from strawberry_django.utils import get_annotations, is_similar_django_type
 from typing_extensions import Annotated
 
 from strawberry_django_plus.optimizer import OptimizerStore, PrefetchType
@@ -85,19 +86,25 @@
     if is_connection or isinstance(attr, ConnectionField):
         field = attr
         if not isinstance(field, ConnectionField):
             field = connection()
 
         field = cast(StrawberryDjangoField, field)
 
-        # FIXME: Improve this...
         if not field.base_resolver:
 
-            def conn_resolver(root):
-                return getattr(root, name).all()
+            def conn_resolver(root, info: Info):
+                qs = getattr(root, name).all()
+                if not type_annotation:
+                    return qs
+                remote_type_defs = get_args(type_annotation.annotation)
+                remote_type = eval_type(remote_type_defs[0], type_annotation.namespace, None)
+                if hasattr(remote_type, "get_queryset"):
+                    qs = remote_type.get_queryset(qs, info)
+                return qs
 
             field.base_resolver = StrawberryResolver(conn_resolver)
             if type_annotation is not None:
                 field.type_annotation = type_annotation
     elif isinstance(attr, StrawberryDjangoField) and not attr.origin_django_type:
         field = attr
     elif isinstance(attr, dataclasses.Field):
```

### Comparing `strawberry_django_plus-2.5.0/strawberry_django_plus/types.py` & `strawberry_django_plus-2.6.0/strawberry_django_plus/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import strawberry
 from django.db import models
 from django.db.models.fields import NOT_PROVIDED
 from django.db.models.fields.related import ManyToManyField
 from django.db.models.fields.reverse_related import ForeignObjectRel
 from strawberry import UNSET
 from strawberry.custom_scalar import ScalarWrapper
+from strawberry.enum import EnumValueDefinition
 from strawberry.file_uploads import Upload
 from strawberry.type import StrawberryType
 from strawberry.utils.str_converters import capitalize_first, to_camel_case
 from strawberry_django.fields.types import (
     DjangoModelType,
     ManyToManyInput,
     ManyToOneInput,
@@ -265,15 +266,17 @@
         and isinstance(field, models.Field)
         and (choices := getattr(field, "choices", None)) is not None
     ):
         strawberry_enum = getattr(field, "_strawberry_enum", None)
         if strawberry_enum is None:
             # Generate automatic Enum class for standard django's "choices" fields
             meta = field.model._meta
-            auto_enum_class_fields = {c[0]: c[0] for c in choices}
+            auto_enum_class_fields = {
+                c[0]: EnumValueDefinition(value=c[0], description=c[1]) for c in choices
+            }
             auto_enum_class_name = "".join(
                 (
                     capitalize_first(to_camel_case(meta.app_label)),
                     str(meta.object_name),
                     capitalize_first(to_camel_case(field.name)),
                     "Enum",
                 ),
```

### Comparing `strawberry_django_plus-2.5.0/strawberry_django_plus/utils/aio.py` & `strawberry_django_plus-2.6.0/strawberry_django_plus/utils/aio.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.5.0/strawberry_django_plus/utils/inspect.py` & `strawberry_django_plus-2.6.0/strawberry_django_plus/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.5.0/strawberry_django_plus/utils/pyutils.py` & `strawberry_django_plus-2.6.0/strawberry_django_plus/utils/pyutils.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.5.0/strawberry_django_plus/utils/query.py` & `strawberry_django_plus-2.6.0/strawberry_django_plus/utils/query.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.5.0/strawberry_django_plus/utils/resolvers.py` & `strawberry_django_plus-2.6.0/strawberry_django_plus/utils/resolvers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.5.0/strawberry_django_plus/utils/typing.py` & `strawberry_django_plus-2.6.0/strawberry_django_plus/utils/typing.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.5.0/PKG-INFO` & `strawberry_django_plus-2.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-django-plus
-Version: 2.5.0
+Version: 2.6.0
 Summary: Enhanced Strawberry GraphQL integration with Django
 Home-page: https://github.com/blb-ventures/strawberry-django-plus
 License: MIT
 Keywords: strawberry,django,graphql,relay,optimizer
 Author: Thiago Bellini Ribeiro
 Author-email: thiago@bellini.dev
 Requires-Python: >=3.8,<4.0
```

