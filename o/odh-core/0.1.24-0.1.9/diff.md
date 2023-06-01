# Comparing `tmp/odh_core-0.1.24.tar.gz` & `tmp/odh_core-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odh_core-0.1.24.tar", last modified: Thu Jun  1 12:13:46 2023, max compression
+gzip compressed data, was "odh_core-0.1.9.tar", last modified: Wed May  3 15:19:24 2023, max compression
```

## Comparing `odh_core-0.1.24.tar` & `odh_core-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0      171 2023-05-11 11:57:09.306140 odh_core-0.1.24/README.md
--rw-r--r--   0        0        0      483 2023-06-01 12:13:12.610104 odh_core-0.1.24/odh_core/__init__.py
--rw-r--r--   0        0        0     5482 2023-06-01 12:12:32.578009 odh_core-0.1.24/odh_core/graphql_client.py
--rw-r--r--   0        0        0     2056 2023-05-05 13:51:59.703502 odh_core-0.1.24/odh_core/logger.py
--rw-r--r--   0        0        0     4786 2023-05-31 12:40:53.590891 odh_core-0.1.24/odh_core/logging_settings.py
--rw-r--r--   0        0        0    15013 2023-05-31 12:40:53.590891 odh_core-0.1.24/odh_core/ms_odata.py
--rw-r--r--   0        0        0     2101 2023-05-05 13:52:03.193525 odh_core-0.1.24/odh_core/phonenumber.py
--rw-r--r--   0        0        0     1174 2023-06-01 10:40:44.450636 odh_core-0.1.24/odh_core/ssn.py
--rw-r--r--   0        0        0     1161 2023-06-01 12:13:46.711267 odh_core-0.1.24/pyproject.toml
--rw-r--r--   0        0        0     1286 1970-01-01 00:00:00.000000 odh_core-0.1.24/PKG-INFO
+-rw-r--r--   0        0        0      171 2023-05-03 14:19:54.886571 odh_core-0.1.9/README.md
+-rw-r--r--   0        0        0      440 2023-05-03 14:46:18.755967 odh_core-0.1.9/odh_core/__init__.py
+-rw-r--r--   0        0        0     2523 2023-05-03 08:43:09.611592 odh_core-0.1.9/odh_core/graphql_client.py
+-rw-r--r--   0        0        0     2056 2023-04-26 08:25:44.881301 odh_core-0.1.9/odh_core/logger.py
+-rw-r--r--   0        0        0     4784 2023-04-26 15:14:15.298371 odh_core-0.1.9/odh_core/logging_settings.py
+-rw-r--r--   0        0        0    12313 2023-04-28 12:42:22.472776 odh_core-0.1.9/odh_core/ms_odata.py
+-rw-r--r--   0        0        0     2101 2023-05-03 13:57:06.837560 odh_core-0.1.9/odh_core/phonenumber.py
+-rw-r--r--   0        0        0     1067 2023-05-03 15:19:24.212108 odh_core-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1128 1970-01-01 00:00:00.000000 odh_core-0.1.9/PKG-INFO
```

### Comparing `odh_core-0.1.24/odh_core/logger.py` & `odh_core-0.1.9/odh_core/logger.py`

 * *Files identical despite different names*

### Comparing `odh_core-0.1.24/odh_core/logging_settings.py` & `odh_core-0.1.9/odh_core/logging_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         },
     },
     # root sets default values and subsequent loggers can override the values
     # "root": {"handlers": ["console"], "level": "DEBUG"},
     "root": {"handlers": ["console"], "level": "INFO"},
     "loggers": {
         "gql.transport.aiohttp": {
-            "level": "WARNING",
+            "level": "DEBUG",
             "filters": ["hide_gql_schema", "hide_gql_IntrospectionQuery"],
             # "handlers": ["file"],
         },
         "odh": {
             "level": "INFO",
             # "handlers": ["console"],
         },
```

### Comparing `odh_core-0.1.24/odh_core/ms_odata.py` & `odh_core-0.1.9/odh_core/ms_odata.py`

 * *Files 17% similar despite different names*

```diff
@@ -286,94 +286,30 @@
         request_retry = 0
         while request_retry < 5:
             # make the request
             url = f"/{endpoint}/{resource}"
             async with self.session.post(url=url, data=data) as resp:
                 if resp.status == 204:
                     resp_json = {}
-                    return resp_json
-                # if we get 200, return the data
-                if resp.status >= 200 and resp.status < 300:
-                    resp_json = await resp.json()
-                    if not resp.ok:
-                        log.error(f'graph error: {resp_json["error"]["message"]}')
-                        log.debug(resp_json)
-                    return resp_json
-                # if we get 401, refresh the token and retry
-                elif resp.status == 401:
-                    # refresh the token
-                    await self.update_token_header()
-                    request_retry += 1
-
-                # if we get 400, raise an error, something is wrong get user code to handle it
-                elif resp.status == 400:
-                    resp_json = await resp.json()
-                    raise GraphError(resp_json["error"]["message"])
-
-                # if we get 429, wait and retry
-                elif resp.status == 429:
-                    delay = float(resp.headers["retry-after"])
-                    log.info(
-                        f"Request to {url} failed with 429, retrying in {delay} seconds"
-                    )
-                    await asyncio.sleep(delay)
-                    request_retry += 1
-                # if we get 503, wait and retry
-                elif resp.status == 503:
-                    delay = float(resp.headers["retry-after"])
-                    log.info(
-                        f"Request to {url} failed with 503, retrying in {delay} seconds"
-                    )
-                    await asyncio.sleep(delay)
-                    request_retry += 1
-                # if we get anything else, log it and return empty
                 else:
                     resp_json = await resp.json()
+                if not resp.ok:
+                    log.error(f'graph error: {resp_json["error"]["message"]}')
                     log.debug(resp_json)
-                    log.error(
-                        f"Request to {url} failed with {resp.status} {resp.reason}"
-                    )
-                    return {}
-
-    async def delete(
-        self,
-        resource: str,
-        endpoint: str = "v1.0",
-    ):
-        """Handles retry logic and token refresh for microsoft graph post request
-
-        Delete data from the graph using the odata protocol
-
-        https://learn.microsoft.com/en-us/graph/errors
-
-        """
-        request_retry = 0
-        while request_retry < 5:
-            # make the request
-            url = f"/{endpoint}/{resource}"
-            async with self.session.delete(url=url) as resp:
-                if resp.status == 204:
-                    resp_json = {}
-                    return resp_json
                 # if we get 200, return the data
                 if resp.status >= 200 and resp.status < 300:
-                    resp_json = await resp.json()
-                    if not resp.ok:
-                        log.error(f'graph error: {resp_json["error"]["message"]}')
-                        log.debug(resp_json)
                     return resp_json
                 # if we get 401, refresh the token and retry
                 elif resp.status == 401:
                     # refresh the token
                     await self.update_token_header()
                     request_retry += 1
 
                 # if we get 400, raise an error, something is wrong get user code to handle it
                 elif resp.status == 400:
-                    resp_json = await resp.json()
                     raise GraphError(resp_json["error"]["message"])
 
                 # if we get 429, wait and retry
                 elif resp.status == 429:
                     delay = float(resp.headers["retry-after"])
                     log.info(
                         f"Request to {url} failed with 429, retrying in {delay} seconds"
@@ -386,13 +322,12 @@
                     log.info(
                         f"Request to {url} failed with 503, retrying in {delay} seconds"
                     )
                     await asyncio.sleep(delay)
                     request_retry += 1
                 # if we get anything else, log it and return empty
                 else:
-                    resp_json = await resp.json()
                     log.debug(resp_json)
                     log.error(
                         f"Request to {url} failed with {resp.status} {resp.reason}"
                     )
                     return {}
```

### Comparing `odh_core-0.1.24/odh_core/phonenumber.py` & `odh_core-0.1.9/odh_core/phonenumber.py`

 * *Files identical despite different names*

### Comparing `odh_core-0.1.24/pyproject.toml` & `odh_core-0.1.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -17,25 +17,23 @@
 [project]
 authors = [
     { name = "Jimmy Spets", email = "jimmy.spets@waochurch.com" },
     { name = "Viktor Freiman", email = "viktor.freiman@waochurch.com" },
 ]
 dependencies = [
     "gql[aiohttp]",
-    "personnummer",
     "phonenumbers",
-    "python-dotenv",
     "python-jose[cryptography]",
 ]
 description = "ODH Core, helper functions and classes"
 dynamic = []
 name = "odh-core"
 readme = "README.md"
 requires-python = ">=3.10"
-version = "0.1.24"
+version = "0.1.9"
 
 [project.optional-dependencies]
 dev = [
     "Sphinx",
     "black",
     "flake8",
     "flake8-bugbear",
@@ -44,16 +42,14 @@
     "sphinx-autobuild",
     "sphinx-rtd-theme",
     "toml",
     "sphinxcontrib-autoprogram",
     "docs-helper",
     "pytest",
     "pytest-asyncio",
-    "azure-identity",
-    "azure-keyvault-secrets",
 ]
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
```

### Comparing `odh_core-0.1.24/PKG-INFO` & `odh_core-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 Metadata-Version: 2.1
 Name: odh-core
-Version: 0.1.24
+Version: 0.1.9
 Summary: ODH Core, helper functions and classes
 Author-Email: Jimmy Spets <jimmy.spets@waochurch.com>, Viktor Freiman <viktor.freiman@waochurch.com>
 License: MIT
 Requires-Python: >=3.10
 Requires-Dist: gql[aiohttp]
-Requires-Dist: personnummer
 Requires-Dist: phonenumbers
-Requires-Dist: python-dotenv
 Requires-Dist: python-jose[cryptography]
 Requires-Dist: Sphinx; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: flake8-bugbear; extra == "dev"
 Requires-Dist: flake8-quotes; extra == "dev"
 Requires-Dist: rinohtype; extra == "dev"
 Requires-Dist: sphinx-autobuild; extra == "dev"
 Requires-Dist: sphinx-rtd-theme; extra == "dev"
 Requires-Dist: toml; extra == "dev"
 Requires-Dist: sphinxcontrib-autoprogram; extra == "dev"
 Requires-Dist: docs-helper; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
-Requires-Dist: azure-identity; extra == "dev"
-Requires-Dist: azure-keyvault-secrets; extra == "dev"
 Provides-Extra: dev
 Description-Content-Type: text/markdown
 
 # ODH CORE
 
 Core helper py lib for working with ODH
```

