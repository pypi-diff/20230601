# Comparing `tmp/swagger-petstore-3-sdk-1.0.4.tar.gz` & `tmp/swagger-petstore-3-sdk-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swagger-petstore-3-sdk-1.0.4.tar", last modified: Wed May 31 12:59:46 2023, max compression
+gzip compressed data, was "swagger-petstore-3-sdk-2.0.1.tar", last modified: Thu Jun  1 08:10:33 2023, max compression
```

## Comparing `swagger-petstore-3-sdk-1.0.4.tar` & `swagger-petstore-3-sdk-2.0.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:59:46.149617 swagger-petstore-3-sdk-1.0.4/
--rw-r--r--   0 root         (0) root         (0)     1213 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      462 2023-05-31 12:59:46.149617 swagger-petstore-3-sdk-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4212 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/README.md
--rw-r--r--   0 root         (0) root         (0)      799 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       77 2023-05-31 12:59:46.150617 swagger-petstore-3-sdk-1.0.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:59:46.112617 swagger-petstore-3-sdk-1.0.4/swagger_petstore_3_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      462 2023-05-31 12:59:46.000000 swagger-petstore-3-sdk-1.0.4/swagger_petstore_3_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1811 2023-05-31 12:59:46.000000 swagger-petstore-3-sdk-1.0.4/swagger_petstore_3_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 12:59:46.000000 swagger-petstore-3-sdk-1.0.4/swagger_petstore_3_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      164 2023-05-31 12:59:46.000000 swagger-petstore-3-sdk-1.0.4/swagger_petstore_3_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-05-31 12:59:46.000000 swagger-petstore-3-sdk-1.0.4/swagger_petstore_3_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:59:46.116617 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/
--rw-r--r--   0 root         (0) root         (0)      163 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/__init__.py
--rw-r--r--   0 root         (0) root         (0)      567 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/api_helper.py
--rw-r--r--   0 root         (0) root         (0)     4155 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:59:46.124617 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/controllers/
--rw-r--r--   0 root         (0) root         (0)      110 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1990 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/controllers/base_controller.py
--rw-r--r--   0 root         (0) root         (0)    15580 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/controllers/pet_controller.py
--rw-r--r--   0 root         (0) root         (0)     7469 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/controllers/store_controller.py
--rw-r--r--   0 root         (0) root         (0)    13430 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/controllers/user_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:59:46.126617 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/exceptions/
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/exceptions/api_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:59:46.130617 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/http/
--rw-r--r--   0 root         (0) root         (0)      118 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/http/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:59:46.133617 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/http/auth/
--rw-r--r--   0 root         (0) root         (0)       51 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/http/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      726 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/http/auth/custom_header_authentication.py
--rw-r--r--   0 root         (0) root         (0)      486 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/http/http_call_back.py
--rw-r--r--   0 root         (0) root         (0)      493 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/http/http_method_enum.py
--rw-r--r--   0 root         (0) root         (0)     1875 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/http/http_request.py
--rw-r--r--   0 root         (0) root         (0)     1496 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/http/http_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:59:46.145617 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/models/
--rw-r--r--   0 root         (0) root         (0)      203 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2536 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/models/address.py
--rw-r--r--   0 root         (0) root         (0)     1861 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/models/category.py
--rw-r--r--   0 root         (0) root         (0)     2452 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/models/customer.py
--rw-r--r--   0 root         (0) root         (0)     3417 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/models/order.py
--rw-r--r--   0 root         (0) root         (0)      518 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/models/order_status_enum.py
--rw-r--r--   0 root         (0) root         (0)     3397 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/models/pet.py
--rw-r--r--   0 root         (0) root         (0)     2241 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/models/pet_image.py
--rw-r--r--   0 root         (0) root         (0)      516 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/models/pet_status_enum.py
--rw-r--r--   0 root         (0) root         (0)      520 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/models/status_enum.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/models/tag.py
--rw-r--r--   0 root         (0) root         (0)     4052 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/models/user.py
--rw-r--r--   0 root         (0) root         (0)     3298 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/swaggerpetstoreopenapi_30_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:59:46.147617 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/utilities/
--rw-r--r--   0 root         (0) root         (0)       35 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      441 2023-05-31 12:59:13.000000 swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/utilities/file_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 08:10:33.489822 swagger-petstore-3-sdk-2.0.1/
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      422 2023-06-01 08:10:33.489822 swagger-petstore-3-sdk-2.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4212 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/README.md
+-rw-r--r--   0 root         (0) root         (0)     4647 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       77 2023-06-01 08:10:33.490822 swagger-petstore-3-sdk-2.0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 08:10:33.460822 swagger-petstore-3-sdk-2.0.1/swagger_petstore_3_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      422 2023-06-01 08:10:33.000000 swagger-petstore-3-sdk-2.0.1/swagger_petstore_3_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-06-01 08:10:33.000000 swagger-petstore-3-sdk-2.0.1/swagger_petstore_3_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 08:10:33.000000 swagger-petstore-3-sdk-2.0.1/swagger_petstore_3_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      164 2023-06-01 08:10:33.000000 swagger-petstore-3-sdk-2.0.1/swagger_petstore_3_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-01 08:10:33.000000 swagger-petstore-3-sdk-2.0.1/swagger_petstore_3_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 08:10:33.463822 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/
+-rw-r--r--   0 root         (0) root         (0)      163 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      567 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/api_helper.py
+-rw-r--r--   0 root         (0) root         (0)     4155 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 08:10:33.467822 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/controllers/
+-rw-r--r--   0 root         (0) root         (0)      110 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1990 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/controllers/base_controller.py
+-rw-r--r--   0 root         (0) root         (0)    15580 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/controllers/pet_controller.py
+-rw-r--r--   0 root         (0) root         (0)     7469 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/controllers/store_controller.py
+-rw-r--r--   0 root         (0) root         (0)    13430 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/controllers/user_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 08:10:33.469823 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/exceptions/
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/exceptions/api_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 08:10:33.476822 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/http/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/http/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 08:10:33.477822 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/http/auth/
+-rw-r--r--   0 root         (0) root         (0)       51 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/http/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      726 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/http/auth/custom_header_authentication.py
+-rw-r--r--   0 root         (0) root         (0)      486 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/http/http_call_back.py
+-rw-r--r--   0 root         (0) root         (0)      493 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/http/http_method_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1875 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/http/http_request.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/http/http_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 08:10:33.488823 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/
+-rw-r--r--   0 root         (0) root         (0)      203 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2536 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/address.py
+-rw-r--r--   0 root         (0) root         (0)     1861 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/category.py
+-rw-r--r--   0 root         (0) root         (0)     2452 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/customer.py
+-rw-r--r--   0 root         (0) root         (0)     3417 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/order.py
+-rw-r--r--   0 root         (0) root         (0)      518 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/order_status_enum.py
+-rw-r--r--   0 root         (0) root         (0)     3397 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/pet.py
+-rw-r--r--   0 root         (0) root         (0)     2241 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/pet_image.py
+-rw-r--r--   0 root         (0) root         (0)      516 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/pet_status_enum.py
+-rw-r--r--   0 root         (0) root         (0)      520 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/status_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/tag.py
+-rw-r--r--   0 root         (0) root         (0)     4052 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/user.py
+-rw-r--r--   0 root         (0) root         (0)     3298 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/swaggerpetstoreopenapi_30_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 08:10:33.489822 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/utilities/
+-rw-r--r--   0 root         (0) root         (0)       35 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      441 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/utilities/file_wrapper.py
```

### Comparing `swagger-petstore-3-sdk-1.0.4/LICENSE` & `swagger-petstore-3-sdk-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-1.0.4/README.md` & `swagger-petstore-3-sdk-2.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -19,34 +19,34 @@
 
 ## Install the Package
 
 The package is compatible with Python versions `3 >=3.7, <= 3.11`.
 Install the package from PyPi using the following pip command:
 
 ```python
-pip install swagger-petstore-3-sdk==1.0.4
+pip install swagger-petstore-3-sdk==2.0.1
 ```
 
 You can also view the package at:
-https://pypi.python.org/pypi/swagger-petstore-3-sdk/1.0.4
+https://pypi.python.org/pypi/swagger-petstore-3-sdk/2.0.1
 
 ## Test the SDK
 
 You can test the generated SDK and the server with test cases. `unittest` is used as the testing framework and `pytest` is used as the test runner. You can run the tests as follows:
 
 Navigate to the root directory of the SDK and run the following commands
 
 ```
 pip install -r test-requirements.txt
 pytest
 ```
 
 ## Initialize the API Client
 
-**_Note:_** Documentation for the client can be found [here.](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/1.0.4/doc/client.md)
+**_Note:_** Documentation for the client can be found [here.](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/2.0.1/doc/client.md)
 
 The following parameters are configurable for the API Client:
 
 | Parameter | Type | Description |
 |  --- | --- | --- |
 | `http_client_instance` | `HttpClient` | The Http Client passed from the sdk user for making requests |
 | `override_http_client_configuration` | `bool` | The value which determines to override properties of the passed Http Client from the sdk user |
@@ -72,17 +72,17 @@
 
 ## Authorization
 
 This API uses `Custom Header Signature`.
 
 ## List of APIs
 
-* [Pet](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/1.0.4/doc/controllers/pet.md)
-* [Store](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/1.0.4/doc/controllers/store.md)
-* [User](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/1.0.4/doc/controllers/user.md)
+* [Pet](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/2.0.1/doc/controllers/pet.md)
+* [Store](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/2.0.1/doc/controllers/store.md)
+* [User](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/2.0.1/doc/controllers/user.md)
 
 ## Classes Documentation
 
-* [Utility Classes](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/1.0.4/doc/utility-classes.md)
-* [HttpResponse](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/1.0.4/doc/http-response.md)
-* [HttpRequest](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/1.0.4/doc/http-request.md)
+* [Utility Classes](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/2.0.1/doc/utility-classes.md)
+* [HttpResponse](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/2.0.1/doc/http-response.md)
+* [HttpRequest](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/2.0.1/doc/http-request.md)
```

### Comparing `swagger-petstore-3-sdk-1.0.4/swagger_petstore_3_sdk.egg-info/SOURCES.txt` & `swagger-petstore-3-sdk-2.0.1/swagger_petstore_3_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/api_helper.py` & `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/api_helper.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/configuration.py` & `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/configuration.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/controllers/base_controller.py` & `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/controllers/pet_controller.py` & `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/controllers/pet_controller.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/controllers/store_controller.py` & `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/controllers/store_controller.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/controllers/user_controller.py` & `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/controllers/user_controller.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/exceptions/api_exception.py` & `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/http/auth/custom_header_authentication.py` & `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/http/auth/custom_header_authentication.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/http/http_request.py` & `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/http/http_request.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/http/http_response.py` & `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/http/http_response.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/models/address.py` & `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/address.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/models/category.py` & `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/category.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/models/customer.py` & `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/customer.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/models/order.py` & `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/order.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/models/order_status_enum.py` & `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/order_status_enum.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/models/pet.py` & `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/pet.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/models/pet_image.py` & `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/pet_image.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/models/pet_status_enum.py` & `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/pet_status_enum.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/models/status_enum.py` & `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/status_enum.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/models/tag.py` & `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/tag.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/models/user.py` & `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/user.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-1.0.4/swaggerpetstoreopenapi30/swaggerpetstoreopenapi_30_client.py` & `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/swaggerpetstoreopenapi_30_client.py`

 * *Files identical despite different names*

