# Comparing `tmp/strawberry_azure_auth-1.1.0.tar.gz` & `tmp/strawberry_azure_auth-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_azure_auth-1.1.0.tar", max compression
+gzip compressed data, was "strawberry_azure_auth-1.2.0.tar", max compression
```

## Comparing `strawberry_azure_auth-1.1.0.tar` & `strawberry_azure_auth-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1065 2023-05-23 10:28:24.979394 strawberry_azure_auth-1.1.0/LICENSE
--rw-r--r--   0        0        0     3418 2023-05-23 10:28:24.979394 strawberry_azure_auth-1.1.0/README.md
--rw-r--r--   0        0        0      955 2023-05-23 10:28:24.979394 strawberry_azure_auth-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      167 2023-05-23 10:28:24.979394 strawberry_azure_auth-1.1.0/strawberry_azure_auth/__init__.py
--rw-r--r--   0        0        0      154 2023-05-23 10:28:24.979394 strawberry_azure_auth-1.1.0/strawberry_azure_auth/channels/__init__.py
--rw-r--r--   0        0        0     1318 2023-05-23 10:28:24.979394 strawberry_azure_auth-1.1.0/strawberry_azure_auth/channels/context.py
--rw-r--r--   0        0        0     1851 2023-05-23 10:28:24.979394 strawberry_azure_auth-1.1.0/strawberry_azure_auth/channels/handlers.py
--rw-r--r--   0        0        0     7097 2023-05-23 10:28:24.979394 strawberry_azure_auth-1.1.0/strawberry_azure_auth/channels/schema.py
--rw-r--r--   0        0        0        0 2023-05-23 10:28:24.979394 strawberry_azure_auth-1.1.0/strawberry_azure_auth/django/__init__.py
--rw-r--r--   0        0        0      920 2023-05-23 10:28:24.979394 strawberry_azure_auth-1.1.0/strawberry_azure_auth/django/context.py
--rw-r--r--   0        0        0    10627 2023-05-23 10:28:24.979394 strawberry_azure_auth-1.1.0/strawberry_azure_auth/extension.py
--rw-r--r--   0        0        0     5416 2023-05-23 10:28:24.979394 strawberry_azure_auth-1.1.0/strawberry_azure_auth/openid.py
--rw-r--r--   0        0        0     1164 2023-05-23 10:28:24.979394 strawberry_azure_auth-1.1.0/strawberry_azure_auth/permissions.py
--rw-r--r--   0        0        0      519 2023-05-23 10:28:24.979394 strawberry_azure_auth-1.1.0/strawberry_azure_auth/types.py
--rw-r--r--   0        0        0     1585 2023-05-23 10:28:24.979394 strawberry_azure_auth-1.1.0/strawberry_azure_auth/utils.py
--rw-r--r--   0        0        0     4174 1970-01-01 00:00:00.000000 strawberry_azure_auth-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-01 16:07:40.921981 strawberry_azure_auth-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3418 2023-06-01 16:07:40.921981 strawberry_azure_auth-1.2.0/README.md
+-rw-r--r--   0        0        0      955 2023-06-01 16:07:40.925982 strawberry_azure_auth-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      167 2023-06-01 16:07:40.925982 strawberry_azure_auth-1.2.0/strawberry_azure_auth/__init__.py
+-rw-r--r--   0        0        0      154 2023-06-01 16:07:40.925982 strawberry_azure_auth-1.2.0/strawberry_azure_auth/channels/__init__.py
+-rw-r--r--   0        0        0     1318 2023-06-01 16:07:40.925982 strawberry_azure_auth-1.2.0/strawberry_azure_auth/channels/context.py
+-rw-r--r--   0        0        0     1851 2023-06-01 16:07:40.925982 strawberry_azure_auth-1.2.0/strawberry_azure_auth/channels/handlers.py
+-rw-r--r--   0        0        0     8597 2023-06-01 16:07:40.925982 strawberry_azure_auth-1.2.0/strawberry_azure_auth/channels/schema.py
+-rw-r--r--   0        0        0        0 2023-06-01 16:07:40.925982 strawberry_azure_auth-1.2.0/strawberry_azure_auth/django/__init__.py
+-rw-r--r--   0        0        0      920 2023-06-01 16:07:40.925982 strawberry_azure_auth-1.2.0/strawberry_azure_auth/django/context.py
+-rw-r--r--   0        0        0    10706 2023-06-01 16:07:40.925982 strawberry_azure_auth-1.2.0/strawberry_azure_auth/extension.py
+-rw-r--r--   0        0        0     5569 2023-06-01 16:07:40.925982 strawberry_azure_auth-1.2.0/strawberry_azure_auth/openid.py
+-rw-r--r--   0        0        0     1164 2023-06-01 16:07:40.925982 strawberry_azure_auth-1.2.0/strawberry_azure_auth/permissions.py
+-rw-r--r--   0        0        0      519 2023-06-01 16:07:40.925982 strawberry_azure_auth-1.2.0/strawberry_azure_auth/types.py
+-rw-r--r--   0        0        0     1585 2023-06-01 16:07:40.925982 strawberry_azure_auth-1.2.0/strawberry_azure_auth/utils.py
+-rw-r--r--   0        0        0     4174 1970-01-01 00:00:00.000000 strawberry_azure_auth-1.2.0/PKG-INFO
```

### Comparing `strawberry_azure_auth-1.1.0/LICENSE` & `strawberry_azure_auth-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-1.1.0/README.md` & `strawberry_azure_auth-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-1.1.0/pyproject.toml` & `strawberry_azure_auth-1.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strawberry-azure-auth"
-version = "1.1.0"
+version = "1.2.0"
 description = "Azure AD authentication for Strawberry GraphQL"
 authors = ["skarre-r <skarre-r@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/skarre-r/strawberry-azure-auth"
 packages = [{include = "strawberry_azure_auth"}]
 
@@ -12,15 +12,15 @@
 python = "^3.11"
 httpx = "^0.24.1"
 pyjwt = { version = "^2.7.0", extras = ["crypto"] }
 strawberry-graphql = { version = "^0.177.3", extras = ["channels"] }
 strawberry-graphql-django = "^0.9.4"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.0.269"
+ruff = "^0.0.270"
 mypy = "^1.3.0"
 black = "^23.3.0"
 pre-commit = "^3.3.1"
 ipython = "^8.13.2"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `strawberry_azure_auth-1.1.0/strawberry_azure_auth/channels/context.py` & `strawberry_azure_auth-1.2.0/strawberry_azure_auth/channels/context.py`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-1.1.0/strawberry_azure_auth/channels/handlers.py` & `strawberry_azure_auth-1.2.0/strawberry_azure_auth/channels/handlers.py`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-1.1.0/strawberry_azure_auth/channels/schema.py` & `strawberry_azure_auth-1.2.0/strawberry_azure_auth/channels/schema.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 from __future__ import annotations
 
 __all__ = ["Schema"]
 
 import logging
 import strawberry
-from typing import Any, AsyncIterable, AsyncGenerator, Callable
+from typing import Any, AsyncIterable, AsyncGenerator, Callable, Iterable, TYPE_CHECKING
+
 from strawberry.types.graphql import OperationType
 from strawberry.schema.execute import _run_validation, parse_document
-from strawberry.extensions import SchemaExtension
 from strawberry.extensions.runner import SchemaExtensionsRunner
 from strawberry.exceptions import MissingQueryError
 from strawberry.schema.exceptions import InvalidOperationTypeError
 from graphql import (
     ExecutionResult,
-    GraphQLSchema,
     GraphQLError,
-    DocumentNode,
-    GraphQLFieldResolver,
     parse,
     subscribe,
 )
 
 from .context import ChannelsExecutionContext
 
+if TYPE_CHECKING:
+    from strawberry.custom_scalar import ScalarWrapper, ScalarDefinition
+    from strawberry.directive import StrawberryDirective
+    from strawberry.schema.config import StrawberryConfig
+    from strawberry.type import StrawberryType
+    from strawberry.extensions import SchemaExtension
+    from graphql import GraphQLFieldResolver, DocumentNode, GraphQLSchema, ExecutionContext
+
+
 logger: logging.Logger = logging.getLogger(name="strawberry.execution")
 
 
 async def _subscribe(
     schema: GraphQLSchema,
     document: DocumentNode,
     extensions: list[type[SchemaExtension] | SchemaExtension],  # !
@@ -129,14 +135,42 @@
     Custom :class:`strawberry.Schema<strawberry.Schema>` class
     that overrides the :method:`subscribe<strawberry.Schema.subscribe>` method
     to make schema extensions also apply to GraphQL subscriptions.
 
     Inspired by: https://github.com/strawberry-graphql/strawberry/issues/2097#issuecomment-1314812575
     """
 
+    def __init__(
+        self,
+        query: type,
+        mutation: type | None = None,
+        subscription: type | None = None,
+        directives: Iterable[StrawberryDirective] = (),
+        types: Iterable[type | StrawberryType] = (),
+        extensions: Iterable[type[SchemaExtension] | SchemaExtension] = (),
+        execution_context_class: type[ExecutionContext] | None = None,
+        config: StrawberryConfig | None = None,
+        scalar_overrides: dict[object, type | ScalarWrapper | ScalarDefinition] | None = None,
+        schema_directives: Iterable[object] = (),
+        debug: bool = False,
+    ) -> None:
+        self.debug: bool = debug
+        super().__init__(
+            query=query,
+            mutation=mutation,
+            subscription=subscription,
+            directives=directives,
+            types=types,
+            extensions=extensions,
+            execution_context_class=execution_context_class,
+            config=config,
+            scalar_overrides=scalar_overrides,
+            schema_directives=schema_directives,
+        )
+
     async def subscribe(
         self,
         query: str,
         variable_values: dict[str, Any] | None = None,
         context_value: Any | None = None,
         root_value: Any | None = None,
         operation_name: str | None = None,
@@ -163,8 +197,11 @@
 
     def process_errors(
         self,
         errors: list[GraphQLError],
         execution_context: ChannelsExecutionContext | None = None,  # type: ignore[override]
     ) -> None:
         for error in errors:
-            logger.error(error)
+            if self.debug:
+                logger.error(error, exc_info=error.original_error)
+            else:
+                logger.error(error)
```

### Comparing `strawberry_azure_auth-1.1.0/strawberry_azure_auth/django/context.py` & `strawberry_azure_auth-1.2.0/strawberry_azure_auth/django/context.py`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-1.1.0/strawberry_azure_auth/extension.py` & `strawberry_azure_auth-1.2.0/strawberry_azure_auth/extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         ...             scopes=...
         ...         )
         ...     ]
     """
 
     execution_context: ExecutionContext
 
+    # TODO: rename the 'allow_unauthenticated' and 'allow_unauthorized' params
     def __init__(
         self,
         *,
         client_id: str,
         tenant_id: str,
         scopes: str | list[str],
         roles: list[str] | None = None,
```

### Comparing `strawberry_azure_auth-1.1.0/strawberry_azure_auth/openid.py` & `strawberry_azure_auth-1.2.0/strawberry_azure_auth/openid.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 __all__ = ["OpenIDConfig"]
 
 import httpx
 import logging
-import contextlib
 from typing import Final, TypedDict
 from datetime import datetime, timedelta
 from jwt.algorithms import RSAAlgorithm
 from cryptography.hazmat.primitives.asymmetric.rsa import RSAPublicKey
 from django.core.cache import cache
 
 logger: logging.Logger = logging.getLogger(name="strawberry.auth")
@@ -97,24 +96,26 @@
         try:
             await self._load_openid_configuration()
         except Exception as exc:
             logger.error("Failed to update the OpenID configuration!", exc_info=exc)
 
     async def _load_openid_configuration(self) -> None:
         if self._use_cache:
-            with contextlib.suppress(Exception):
+            try:
                 cached_config: CacheValues
-                if cached_config := await cache.aget(KEY=CACHE_KEY):
+                if cached_config := await cache.aget(CACHE_KEY):
                     logger.debug("Using OpenID config from cache...")
                     self.issuer = cached_config["issuer"]
                     self.signing_keys = {
                         key: RSAAlgorithm.from_jwk(jwk=value) for key, value in cached_config["keys"].items()
                     }
                     self._last_update = datetime.fromisoformat(cached_config["dt"])
                     return
+            except Exception as exc:
+                logger.warning("Failed to use the cached OpenID config!", exc_info=exc)
 
         async with httpx.AsyncClient(timeout=10) as client:
             openid_url: str = (
                 f"https://login.microsoftonline.com/{self._tenant_id}/v2.0/.well-known/openid-configuration"
             )
             logger.debug("Fetching the OpenID configuration document from '%s'...", openid_url)
             openid_response: httpx.Response = await client.get(
@@ -136,19 +137,21 @@
             if jwk["use"] == "sig":  # signing key
                 public_key: RSAPublicKey = RSAAlgorithm.from_jwk(jwk=jwk)
                 self.signing_keys.update({jwk["kid"]: public_key})
 
         self._last_update = datetime.now()
 
         if self._use_cache:
-            logger.debug("Updating OpenID config in cache...")
-            with contextlib.suppress(Exception):
+            logger.debug("Updating the OpenID cache...")
+            try:
                 value: CacheValues = {
                     "issuer": self.issuer,
                     "keys": {key: RSAAlgorithm.to_jwk(key_obj=value) for key, value in self.signing_keys.items()},
                     "dt": self._last_update.isoformat(),
                 }
                 await cache.aset(key=CACHE_KEY, value=value, timeout=60 * 60 * 24)
+            except Exception as exc:
+                logger.warning("Failed to update the OpenID cache!", exc_info=exc)
 
         logger.debug("OpenID config updated:")
         logger.debug("issuer: %s", self.issuer)
         logger.debug("keys: %s", len(self.signing_keys))
```

### Comparing `strawberry_azure_auth-1.1.0/strawberry_azure_auth/permissions.py` & `strawberry_azure_auth-1.2.0/strawberry_azure_auth/permissions.py`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-1.1.0/strawberry_azure_auth/types.py` & `strawberry_azure_auth-1.2.0/strawberry_azure_auth/types.py`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-1.1.0/strawberry_azure_auth/utils.py` & `strawberry_azure_auth-1.2.0/strawberry_azure_auth/utils.py`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-1.1.0/PKG-INFO` & `strawberry_azure_auth-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-azure-auth
-Version: 1.1.0
+Version: 1.2.0
 Summary: Azure AD authentication for Strawberry GraphQL
 Home-page: https://github.com/skarre-r/strawberry-azure-auth
 License: MIT
 Author: skarre-r
 Author-email: skarre-r@protonmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

