# Comparing `tmp/rudderclient-1.7.0.tar.gz` & `tmp/rudderclient-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rudderclient-1.7.0.tar", last modified: Wed May 31 09:11:58 2023, max compression
+gzip compressed data, was "rudderclient-1.8.0.tar", last modified: Thu Jun  1 11:40:47 2023, max compression
```

## Comparing `rudderclient-1.7.0.tar` & `rudderclient-1.8.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-31 09:11:58.309699 rudderclient-1.7.0/
--rw-r--r--   0 runner    (1001) runner    (1001)     1069 2023-05-31 09:11:31.000000 rudderclient-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) runner    (1001)     1968 2023-05-31 09:11:58.309699 rudderclient-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)      224 2023-05-31 09:11:31.000000 rudderclient-1.7.0/README.md
--rw-r--r--   0 runner    (1001) runner    (1001)     1030 2023-05-31 09:11:49.000000 rudderclient-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) runner    (1001)       38 2023-05-31 09:11:58.309699 rudderclient-1.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-31 09:11:58.302698 rudderclient-1.7.0/src/
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-31 09:11:58.304699 rudderclient-1.7.0/src/rudderclient/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-31 09:11:31.000000 rudderclient-1.7.0/src/rudderclient/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-31 09:11:58.306699 rudderclient-1.7.0/src/rudderclient/aws/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-31 09:11:31.000000 rudderclient-1.7.0/src/rudderclient/aws/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5274 2023-05-31 09:11:31.000000 rudderclient-1.7.0/src/rudderclient/aws/requests.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-31 09:11:58.307699 rudderclient-1.7.0/src/rudderclient/gcp/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-31 09:11:31.000000 rudderclient-1.7.0/src/rudderclient/gcp/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2747 2023-05-31 09:11:31.000000 rudderclient-1.7.0/src/rudderclient/gcp/auth.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2088 2023-05-31 09:11:47.000000 rudderclient-1.7.0/src/rudderclient/gcp/http_requests.py
--rw-r--r--   0 runner    (1001) runner    (1001)      943 2023-05-31 09:11:31.000000 rudderclient-1.7.0/src/rudderclient/gcp/pubsub.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-31 09:11:58.308699 rudderclient-1.7.0/src/rudderclient/request/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-31 09:11:31.000000 rudderclient-1.7.0/src/rudderclient/request/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      528 2023-05-31 09:11:31.000000 rudderclient-1.7.0/src/rudderclient/request/exceptions.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1316 2023-05-31 09:11:31.000000 rudderclient-1.7.0/src/rudderclient/request/helpers.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-31 09:11:58.308699 rudderclient-1.7.0/src/rudderclient/tools/
--rw-r--r--   0 runner    (1001) runner    (1001)     5491 2023-05-31 09:11:31.000000 rudderclient-1.7.0/src/rudderclient/tools/send_account_email.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-31 09:11:58.305699 rudderclient-1.7.0/src/rudderclient.egg-info/
--rw-r--r--   0 runner    (1001) runner    (1001)     1968 2023-05-31 09:11:58.000000 rudderclient-1.7.0/src/rudderclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)      614 2023-05-31 09:11:58.000000 rudderclient-1.7.0/src/rudderclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        1 2023-05-31 09:11:58.000000 rudderclient-1.7.0/src/rudderclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       28 2023-05-31 09:11:58.000000 rudderclient-1.7.0/src/rudderclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       13 2023-05-31 09:11:58.000000 rudderclient-1.7.0/src/rudderclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-01 11:40:47.605796 rudderclient-1.8.0/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1069 2023-06-01 11:40:15.000000 rudderclient-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) runner    (1001)     1968 2023-06-01 11:40:47.605796 rudderclient-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)      224 2023-06-01 11:40:15.000000 rudderclient-1.8.0/README.md
+-rw-r--r--   0 runner    (1001) runner    (1001)     1030 2023-06-01 11:40:37.000000 rudderclient-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) runner    (1001)       38 2023-06-01 11:40:47.605796 rudderclient-1.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-01 11:40:47.596795 rudderclient-1.8.0/src/
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-01 11:40:47.599795 rudderclient-1.8.0/src/rudderclient/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-06-01 11:40:15.000000 rudderclient-1.8.0/src/rudderclient/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-01 11:40:47.601796 rudderclient-1.8.0/src/rudderclient/aws/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-06-01 11:40:15.000000 rudderclient-1.8.0/src/rudderclient/aws/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5006 2023-06-01 11:40:15.000000 rudderclient-1.8.0/src/rudderclient/aws/requests.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-01 11:40:47.603796 rudderclient-1.8.0/src/rudderclient/gcp/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-06-01 11:40:15.000000 rudderclient-1.8.0/src/rudderclient/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2649 2023-06-01 11:40:15.000000 rudderclient-1.8.0/src/rudderclient/gcp/auth.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1969 2023-06-01 11:40:35.000000 rudderclient-1.8.0/src/rudderclient/gcp/http_requests.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      869 2023-06-01 11:40:15.000000 rudderclient-1.8.0/src/rudderclient/gcp/pubsub.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3832 2023-06-01 11:40:35.000000 rudderclient-1.8.0/src/rudderclient/gcp/workspace.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-01 11:40:47.604796 rudderclient-1.8.0/src/rudderclient/request/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-06-01 11:40:15.000000 rudderclient-1.8.0/src/rudderclient/request/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      528 2023-06-01 11:40:15.000000 rudderclient-1.8.0/src/rudderclient/request/exceptions.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1260 2023-06-01 11:40:15.000000 rudderclient-1.8.0/src/rudderclient/request/helpers.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-01 11:40:47.604796 rudderclient-1.8.0/src/rudderclient/tools/
+-rw-r--r--   0 runner    (1001) runner    (1001)     5321 2023-06-01 11:40:15.000000 rudderclient-1.8.0/src/rudderclient/tools/send_account_email.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-01 11:40:47.600796 rudderclient-1.8.0/src/rudderclient.egg-info/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1968 2023-06-01 11:40:47.000000 rudderclient-1.8.0/src/rudderclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)      648 2023-06-01 11:40:47.000000 rudderclient-1.8.0/src/rudderclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        1 2023-06-01 11:40:47.000000 rudderclient-1.8.0/src/rudderclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       28 2023-06-01 11:40:47.000000 rudderclient-1.8.0/src/rudderclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       13 2023-06-01 11:40:47.000000 rudderclient-1.8.0/src/rudderclient.egg-info/top_level.txt
```

### Comparing `rudderclient-1.7.0/LICENSE` & `rudderclient-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rudderclient-1.7.0/PKG-INFO` & `rudderclient-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rudderclient
-Version: 1.7.0
+Version: 1.8.0
 Summary: Shared helpers for rudder application functions code
 Author-email: Rudder Team <rudder@realnaut.com>
 License: MIT License
         
         Copyright (c) 2023 RealNaut Ops
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rudderclient-1.7.0/pyproject.toml` & `rudderclient-1.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0.0", "wheel",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rudderclient"
-version = "1.7.0"
+version = "1.8.0"
 description = "Shared helpers for rudder application functions code"
 readme = "README.md"
 classifiers = [ "License :: OSI Approved :: MIT License", "Programming Language :: Python", "Programming Language :: Python :: 3.10",]
 keywords = [ "rudder", "client", "helper",]
 dependencies = [ "google-cloud-secret-manager",]
 requires-python = ">=3.10"
 [[project.authors]]
```

### Comparing `rudderclient-1.7.0/src/rudderclient/aws/requests.py` & `rudderclient-1.8.0/src/rudderclient/aws/requests.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,118 +1,86 @@
-"""
-This library provides an easy way to interact with boto3, the official Python library of AWS.
+"""This library provides an easy way to interact with boto3, the official Python library of AWS."""
 
-Functions:
----------
-get_boto3_client(resource, region, acces_key_id, secret_access_key):
-    Returns a low-level service client.
-
-    Parameters:
-    ----------
-    resource: The name of a service, e.g 'identitystore'. You can get a list of available
-              services via get_available_services().
-    region: The name of the region associated with the client. A client is associated with a single region.
-    access_key_id: The access key to use when creating the client.
-    secret_access_key: The secret key to use when creating the client.
 
-
-delete_user(operation_parameters, region, acces_key_id, secret_access_key):
-    Deletes a user of a unique identityStore.
-
-    Parameters:
-    ----------
-    operation_parameters: A dict with the IdentityStoreId and the UserId you want to delete.
-                          Example: {'IdentityStoreId': identityStoreId, 'UserId': user_id}
-    region: The name of the region associated with the identityStore.
-    access_key_id: The access key to use when creating the client.
-    secret_access_key: The secret key to use when creating the client.
-
-
-get_identitystore_id(region, acces_key_id, secret_access_key):
-    Returns the ID of your organization Identity Store in a unique region.
-
-    Parameters:
-    ----------
-    region: The name of the region associated with the identityStore.
-    access_key_id: The access key to use when creating the client.
-    secret_access_key: The secret key to use when creating the client.
-
-
-describe_user(userId, region, acces_key_id, secret_access_key):
-    Returns information of a user.
-
-    Parameters:
-    ----------
-    userId: The ID of the user.
-    region: The name of the region associated with the identityStore.
-    access_key_id: The access key to use when creating the client.
-    secret_access_key: The secret key to use when creating the client.
-
-
-create_user(userEmail, firstName, surnames, region, acces_key_id, secret_access_key):
-    Creates a user in an identity Store.
-
-    Parameters:
-    ----------
-    userEmail: the work email of the user.
-    firstName: Name of the user.
-    surnames: One or two surnames of the user.
-    region: The name of the region associated with the identityStore.
-    access_key_id: The access key to use when creating the client.
-    secret_access_key: The secret key to use when creating the client.
+import boto3
 
 
-pagination(action, operation_parameters, region, acces_key_id, secret_access_key):
-    Paginates a list result.
+def get_boto3_client(resource, region, acces_key_id, secret_access_key):
+    """
+    Returns a low-level service client.
 
     Parameters:
     ----------
-    action: The action you want to paginate. For example, 'list_users'.
-    operation_parameters: Necessary parameters for doing the action.
-                          For example {'IdentityStoreId': identityStoreId, 'UserId': user_id}
-    region: The name of the region associated with the identityStore.
-    access_key_id: The access key to use when creating the client.
-    secret_access_key: The secret key to use when creating the client.
-"""
-
-
-import boto3
-
-
-def get_boto3_client(resource, region, acces_key_id, secret_access_key):
+        resource: The name of a service, e.g 'identitystore'. You can get a list of available
+                services via get_available_services().
+        region: The name of the region associated with the client. A client is associated with a single region.
+        access_key_id: The access key to use when creating the client.
+        secret_access_key: The secret key to use when creating the client.
+    """
     client = boto3.client(
         resource,
         region_name=region,
         aws_access_key_id=acces_key_id,
         aws_secret_access_key=secret_access_key,
     )
     return client
 
 
 def delete_user(operation_parameters, region, acces_key_id, secret_access_key):
+    """
+    Deletes a user of a unique identityStore.
+
+    Parameters:
+    ----------
+        operation_parameters: A dict with the IdentityStoreId and the UserId you want to delete.
+                            Example: {'IdentityStoreId': identityStoreId, 'UserId': user_id}
+        region: The name of the region associated with the identityStore.
+        access_key_id: The access key to use when creating the client.
+        secret_access_key: The secret key to use when creating the client.
+    """
     # Create IAM client
     client = get_boto3_client(
         "identitystore", region, acces_key_id, secret_access_key
     )
 
     deleteResponse = client.delete_user(**operation_parameters)
 
     return deleteResponse
 
 
 def get_identitystore_id(region, acces_key_id, secret_access_key):
+    """
+    Returns the ID of your organization Identity Store in a unique region.
+
+    Parameters:
+    ----------
+        region: The name of the region associated with the identityStore.
+        access_key_id: The access key to use when creating the client.
+        secret_access_key: The secret key to use when creating the client.
+    """
     client = get_boto3_client(
         "sso-admin", region, acces_key_id, secret_access_key
     )
     identitystore = client.list_instances()
     id = identitystore["Instances"][0]["IdentityStoreId"]
     return id
 
 
 def describe_user(userId, region, acces_key_id, secret_access_key):
+    """
+    Returns information of a user.
+
+    Parameters:
+    ----------
+        userId: The ID of the user.
+        region: The name of the region associated with the identityStore.
+        access_key_id: The access key to use when creating the client.
+        secret_access_key: The secret key to use when creating the client.
+
+    """
     client = get_boto3_client(
         "identitystore", region, acces_key_id, secret_access_key
     )
     identitystore = get_identitystore_id(
         region, acces_key_id, secret_access_key
     )
     response = client.describe_user(
@@ -120,14 +88,26 @@
     )
     return response
 
 
 def create_user(
     userEmail, firstName, surnames, region, acces_key_id, secret_access_key
 ):
+    """
+    Creates a user in an identity Store.
+
+    Parameters:
+    ----------
+        userEmail: the work email of the user.
+        firstName: Name of the user.
+        surnames: One or two surnames of the user.
+        region: The name of the region associated with the identityStore.
+        access_key_id: The access key to use when creating the client.
+        secret_access_key: The secret key to use when creating the client.
+    """
     client = get_boto3_client(
         "identitystore", region, acces_key_id, secret_access_key
     )
     identitystore = get_identitystore_id(
         region, acces_key_id, secret_access_key
     )
     display_name = f"{firstName} {surnames}"
@@ -141,14 +121,26 @@
     )
     return response
 
 
 def pagination(
     action, operation_parameters, region, acces_key_id, secret_access_key
 ):
+    """
+    Paginates a list result.
+
+    Parameters:
+    ----------
+        action: The action you want to paginate. For example, 'list_users'.
+        operation_parameters: Necessary parameters for doing the action.
+                            For example {'IdentityStoreId': identityStoreId, 'UserId': user_id}
+        region: The name of the region associated with the identityStore.
+        access_key_id: The access key to use when creating the client.
+        secret_access_key: The secret key to use when creating the client.
+    """
     # Create IAM client
     client = get_boto3_client(
         "identitystore", region, acces_key_id, secret_access_key
     )
 
     paginator = client.get_paginator(action)
     page_iterator = paginator.paginate(**operation_parameters)
```

### Comparing `rudderclient-1.7.0/src/rudderclient/gcp/auth.py` & `rudderclient-1.8.0/src/rudderclient/gcp/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,85 +1,84 @@
 """
 GCP Authentication library.
 
 This library provides an easy way for authenticating to GCP services. Also offers a simple method
 to read a value secret interacting with secretmanager API.
 
-Functions:
-----------
-get_secret(secret_id):
-    Returns a secret value from secret manager service.
-
-    Parameters:
-    ----------
-    secret_id: str
-        Secret resource name like projects/xxxxxx/secrets/xxxxxxxx/versions/latest
-
-    Returns:
-    -------
-    The value of the secret.
-
-get_OIDC_token_iap_request(client_id, **kwargs):
-    Returns a token for doing an HTTP request to an application protected by Identity-Aware Proxy.
-
-    Parameters:
-    ----------
-    client_id: The client ID used by Identity-Aware Proxy
-    **kwargs: Any of the parameters defined for the request function:
-              https://github.com/requests/requests/blob/master/requests/api.py
-              If no timeout is provided, it is set to 90 by default.
-
-    Returns:
-    -------
-    An OpenID Connect (OIDC) token from metadata server.
-
-get_workspace_impersonate_credentials_sa(credentials_info, scopes, impersonate_mail):
-    Obtain the credentials with the permissions of the service account, in an impersonal way.
-
-    Parameters:
-    ----------
-    credentials_info: json access key of the service account.
-    scopes: Array of the granular permissions that determine what specific resources and operations the service
-            account can access.
-    impersonate_mail: Email to impersonate the service account.
-
-    Returns:
-    -------
-    The impersonate credentials with the service account and scope permissions.
 """
 
 
 from google.cloud import secretmanager
 from google.oauth2 import id_token
 from google.auth.transport.requests import Request
 from google.oauth2 import service_account
 
 
 def get_secret(secret_id):
+    """
+    Returns a secret value from secret manager service.
+
+    Parameters:
+    ----------
+        secret_id: str
+            Secret resource name like projects/xxxxxx/secrets/xxxxxxxx/versions/latest
+
+    Returns:
+    -------
+    The value of the secret.
+    """
     client = secretmanager.SecretManagerServiceClient()
     secret = client.access_secret_version(request={"name": secret_id})
     value = secret.payload.data.decode("UTF-8")
     return value
 
 
 def get_OIDC_token_iap_request(client_id, **kwargs):
+    """
+    Returns a token for doing an HTTP request to an application protected by Identity-Aware Proxy.
+
+    Parameters:
+    ----------
+        client_id: The client ID used by Identity-Aware Proxy
+        **kwargs: Any of the parameters defined for the request function:
+                https://github.com/requests/requests/blob/master/requests/api.py
+                If no timeout is provided, it is set to 90 by default.
+
+    Returns:
+    -------
+    An OpenID Connect (OIDC) token from metadata server.
+    """
     # Set the default timeout, if missing
     if "timeout" not in kwargs:
         kwargs["timeout"] = 90
 
     # Obtain an OpenID Connect (OIDC) token from metadata server or using service
     # account.
     open_id_connect_token = id_token.fetch_id_token(Request(), client_id)
 
     return open_id_connect_token
 
 
 def get_workspace_impersonate_credentials_sa(
     credentials_info, scopes, impersonate_mail
 ):
+    """
+    Obtain the credentials with the permissions of the service account, in an impersonal way.
+
+    Parameters:
+    ----------
+        credentials_info: json access key of the service account.
+        scopes: Array of the granular permissions that determine what specific resources and operations the service
+                account can access.
+        impersonate_mail: Email to impersonate the service account.
+
+    Returns:
+    -------
+    The impersonate credentials with the service account and scope permissions.
+    """
     credentials = service_account.Credentials.from_service_account_info(
         credentials_info
     )
 
     scoped_credentials = credentials.with_scopes(scopes)
 
     impersonate_credentials = scoped_credentials.with_subject(impersonate_mail)
```

### Comparing `rudderclient-1.7.0/src/rudderclient/gcp/http_requests.py` & `rudderclient-1.8.0/src/rudderclient/gcp/http_requests.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,12 @@
 """
 HTTP requests library.
 
 This library provides an easy way to do HTTP request.
 
-Functions:
----------
-def iap_http_request(method: str, api_url: str, request_url: str, body: str, headers: dict[str, str]):
-    Makes an http request to an API protected by Identity-Aware Proxy.
-
-    Parameters:
-    ----------
-    method: Method of the request. "POST", "PATCH", "DELETE", "GET", "PUT".
-    api_url: The DNS of the API. For example "api-dev.api.test.cloud"
-    request_url: The request url. For example "/api/v1/users"
-    body: Body of the requests.
-    headers: Necessary headers for the requests. The "Authentication: Bearer {token}" token
-    is mandatory. The token value is an OIDC token.
-
-def make_authorized_post_request(endpoint, audience, body):
-    Makes a POST request to another HTTP Cloud Run 
-    by authenticating with the ID token obtained from the google-auth client library
-    using the specified audience value.
-
-    Parameters:
-    ----------
-    endpoint: The URL (hostname + path) receiving the request. For example: 'https://my-cloud-run-service.run.app/my/awesome/url'
-    audience: Your service's hostname. For example: 'https://my-cloud-run-service.run.app/'
-    body: The body of the request. 
-
 """
 
 
 import http.client
 import requests
 
 import google.auth.transport.requests
@@ -41,23 +16,47 @@
 def iap_http_request(
     method: str,
     api_url: str,
     request_url: str,
     body: str,
     headers: dict[str, str],
 ):
+    """
+    Makes an http request to an API protected by Identity-Aware Proxy.
+
+    Parameters:
+    ----------
+        method: Method of the request. "POST", "PATCH", "DELETE", "GET", "PUT".
+        api_url: The DNS of the API. For example "api-dev.api.test.cloud"
+        request_url: The request url. For example "/api/v1/users"
+        body: Body of the requests.
+        headers: Necessary headers for the requests. The "Authentication: Bearer {token}" token
+        is mandatory. The token value is an OIDC token.
+    """
     conn = http.client.HTTPSConnection(api_url)
     conn.request(method=method, url=request_url, body=body, headers=headers)
     res = conn.getresponse()
     data = res.read()
     print(data.decode("utf-8"))
     return data.decode("utf-8")
 
 
 def make_authorized_post_request(endpoint, audience, body):
+    """
+    Makes a POST request to another HTTP Cloud Run
+    by authenticating with the ID token obtained from the google-auth client library
+    using the specified audience value.
+
+    Parameters:
+    ----------
+        endpoint: The URL (hostname + path) receiving the request. For example: 'https://my-cloud-run-service.run.app/my/awesome/url'
+        audience: Your service's hostname. For example: 'https://my-cloud-run-service.run.app/'
+        body: The body of the request.
+    """
+
     auth_req = google.auth.transport.requests.Request()
     id_token = google.oauth2.id_token.fetch_id_token(auth_req, audience)
 
     headers = {"Authorization": f"Bearer {id_token}"}
 
     response = requests.request("POST", endpoint, headers=headers, json=body)
```

### Comparing `rudderclient-1.7.0/src/rudderclient/gcp/pubsub.py` & `rudderclient-1.8.0/src/rudderclient/gcp/pubsub.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 """
 This library provides an easy way to interact with Pub/Sub API.
 
-Functions:
----------
-write_message(project_id, topic_id, message_str, status, joinerId):
+"""
+
+
+from google.cloud import pubsub_v1
+
+
+def write_message(project_id, topic_id, message_str, status, joinerId):
+    """
     Publish a message in Pub Sub.
 
     Parameters:
     ----------
         project_id: The ID of the gcp project where you want to publish a message.
         topic_id: The topic name where you want to publish the message.
         message_str: The message string to publish.
         status and joinerId: Attributes for the message.
-
-"""
-
-
-from google.cloud import pubsub_v1
-
-
-def write_message(project_id, topic_id, message_str, status, joinerId):
+    """
     publisher = pubsub_v1.PublisherClient()
     topic_path = publisher.topic_path(project_id, topic_id)
 
     # Data must be a bytestring
     message = message_str.encode("utf-8")
 
     future = publisher.publish(
```

### Comparing `rudderclient-1.7.0/src/rudderclient/request/exceptions.py` & `rudderclient-1.8.0/src/rudderclient/request/exceptions.py`

 * *Files identical despite different names*

### Comparing `rudderclient-1.7.0/src/rudderclient/request/helpers.py` & `rudderclient-1.8.0/src/rudderclient/request/helpers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,50 @@
 """
 This library contains methods to check and help with http requests.
 
-Functions:
----------
-check_content_type(request, available_content_type):
+"""
+
+import json
+from rudderclient.request.exceptions import (
+    ContentTypeNotSupported,
+    MandatoryArgsNotFilled,
+)
+
+
+def check_content_type(request, available_content_type):
+    """
     Check if the content_type of the request is the content_type available in the request.
 
     Parameters:
     ----------
-    request: The request.
-    available_content_type: The available content type for the request.
+        request: The request.
+        available_content_type: The available content type for the request.
 
     Raise:
     -----
     An exception of type `ContentTypeNotSupported`
+    """
+    if request.headers.get("Content-Type") != available_content_type:
+        raise ContentTypeNotSupported(
+            "The request's body should be formatted as a JSON."
+        )
 
 
-get_params(request, param):
+def get_params(request, param):
+    """
     Returns the value of a specific param in the request.
 
     Parameters:
     ----------
-    reques: The request.
-    param: The name of the param in the request.
+        request: The request.
+        param: The name of the param in the request.
 
     Raise:
     -----
     An exception of type `MandatoryArgsNotFilled` if the param asked is not in the request.
-
-"""
-
-import json
-from rudderclient.request.exceptions import (
-    ContentTypeNotSupported,
-    MandatoryArgsNotFilled,
-)
-
-
-def check_content_type(request, available_content_type):
-    if request.headers.get("Content-Type") != available_content_type:
-        raise ContentTypeNotSupported(
-            "The request's body should be formatted as a JSON."
-        )
-
-
-def get_params(request, param):
+    """
     data = json.loads(request.data)
 
     if param in data:
         return data.get(param)
     else:
         raise MandatoryArgsNotFilled("Unexpected body parameters.")
```

### Comparing `rudderclient-1.7.0/src/rudderclient/tools/send_account_email.py` & `rudderclient-1.8.0/src/rudderclient/tools/send_account_email.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,13 @@
 """
 Email sending library.
 
 This library provides an easy way to send customizable emails with Python.
 It supports various kinds of attachments like images and PDF files.
 
-Functions:
-----------
-get_image(file_path):
-    Returns a MIMEImage object from a file path.
-
-get_html(file_path, replacements):
-    Returns a string from a file, replacing placeholders with actual values.
-
-get_attachment(file_path, filename, _subtype):
-    Returns a MIMEApplication object from a file path, filename, and MIME subtype.
-
-send_email(SMTP_USERNAME, SMTP_PASSWORD, FROM, TO, SUBJECT, NAME, EMAIL,
-           PLATFORM='', ACCESS_URL='', PASSWORD='', FIRST_STEPS_FILE=None,
-           ERROR=False, ATTACHMENTS_PATH='', HTML_TEMPLATE_PATH=''):
-    Sends an email using SMTP with the provided parameters.
-
-    Parameters:
-    ----------
-    SMTP_USERNAME: str
-        Username for the SMTP server.
-    SMTP_PASSWORD: str
-        Password for the SMTP server.
-    FROM: str
-        The email address that will appear as the sender of the email.
-    TO: str
-        The email address of the recipient.
-    SUBJECT: str
-        The subject of the email.
-    NAME: str
-        The name of the recipient.
-    EMAIL: str
-        The recipient's email, used in the email body.
-    PLATFORM: str, optional
-        The platform name, used in the email body.
-    ACCESS_URL: str, optional
-        The access URL, used in the email body.
-    PASSWORD: str, optional
-        The recipient's password, used in the email body.
-    FIRST_STEPS_FILE: str, optional
-        The file path of a PDF file to be attached to the email.
-    ERROR: bool, optional
-        Indicates if the email is an error email. If true, it changes the email template.
-    ATTACHMENTS_PATH: str
-        Path to the email attachments.
-    HTML_TEMPLATE_PATH: str
-        Path to the HTML template file.
-
-    Raises:
-    -------
-    Exception:
-        If there is an error reading the images, processing the email template, or sending the email.
 """
 
 
 import logging
 from email.mime.image import MIMEImage
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
@@ -73,37 +22,46 @@
 
 # AWS Config
 EMAIL_HOST = "email-smtp.us-east-1.amazonaws.com"
 EMAIL_PORT = 587
 
 
 def get_image(file_path):
+    """
+    Returns a MIMEImage object from a file path.
+    """
     try:
         with open(file_path, "rb") as f:
             return MIMEImage(f.read())
     except FileNotFoundError:
         logging.info(f"Image file not found: {file_path}")
         return None
 
 
 def get_html(file_path, replacements):
+    """
+    Returns a string from a file, replacing placeholders with actual values.
+    """
     try:
         with open(file_path, "r") as file:
             filedata = file.read()
 
         for key, val in replacements.items():
             filedata = filedata.replace(key, val)
 
         return filedata
     except Exception as e:
         logging.error(f"Error processing the email template: {e}")
         raise
 
 
 def get_attachment(file_path, filename):
+    """
+    Returns a MIMEApplication object from a file path, filename, and MIME subtype.
+    """
     with open(file_path, "rb") as f:
         ext = filename.split(".")[-1]
         attach = MIMEApplication(f.read(), _subtype=ext)
         attach.add_header(
             "Content-Disposition", "attachment", filename=str(filename)
         )
         return attach
@@ -119,14 +77,53 @@
     EMAIL,
     PLATFORM="",
     ACCESS_URL="",
     PASSWORD="",
     ATTACHMENTS_PATH="",
     HTML_TEMPLATE_PATH="",
 ):
+    """
+    Sends an email using SMTP with the provided parameters.
+
+    Parameters:
+    ----------
+        SMTP_USERNAME: str
+            Username for the SMTP server.
+        SMTP_PASSWORD: str
+            Password for the SMTP server.
+        FROM: str
+            The email address that will appear as the sender of the email.
+        TO: str
+            The email address of the recipient.
+        SUBJECT: str
+            The subject of the email.
+        NAME: str
+            The name of the recipient.
+        EMAIL: str
+            The recipient's email, used in the email body.
+        PLATFORM: str, optional
+            The platform name, used in the email body.
+        ACCESS_URL: str, optional
+            The access URL, used in the email body.
+        PASSWORD: str, optional
+            The recipient's password, used in the email body.
+        FIRST_STEPS_FILE: str, optional
+            The file path of a PDF file to be attached to the email.
+        ERROR: bool, optional
+            Indicates if the email is an error email. If true, it changes the email template.
+        ATTACHMENTS_PATH: str
+            Path to the email attachments.
+        HTML_TEMPLATE_PATH: str
+            Path to the HTML template file.
+
+    Raises:
+    -------
+    Exception:
+        If there is an error reading the images, processing the email template, or sending the email.
+    """
     # AWS Config
     EMAIL_HOST_USER = SMTP_USERNAME
     EMAIL_HOST_PASSWORD = SMTP_PASSWORD
 
     msg = MIMEMultipart("alternative")
     msg["Subject"] = SUBJECT
     msg["From"] = FROM
```

### Comparing `rudderclient-1.7.0/src/rudderclient.egg-info/PKG-INFO` & `rudderclient-1.8.0/src/rudderclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rudderclient
-Version: 1.7.0
+Version: 1.8.0
 Summary: Shared helpers for rudder application functions code
 Author-email: Rudder Team <rudder@realnaut.com>
 License: MIT License
         
         Copyright (c) 2023 RealNaut Ops
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rudderclient-1.7.0/src/rudderclient.egg-info/SOURCES.txt` & `rudderclient-1.8.0/src/rudderclient.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -9,11 +9,12 @@
 src/rudderclient.egg-info/top_level.txt
 src/rudderclient/aws/__init__.py
 src/rudderclient/aws/requests.py
 src/rudderclient/gcp/__init__.py
 src/rudderclient/gcp/auth.py
 src/rudderclient/gcp/http_requests.py
 src/rudderclient/gcp/pubsub.py
+src/rudderclient/gcp/workspace.py
 src/rudderclient/request/__init__.py
 src/rudderclient/request/exceptions.py
 src/rudderclient/request/helpers.py
 src/rudderclient/tools/send_account_email.py
```

