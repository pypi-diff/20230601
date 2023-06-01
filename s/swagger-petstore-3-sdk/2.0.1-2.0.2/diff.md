# Comparing `tmp/swagger-petstore-3-sdk-2.0.1.tar.gz` & `tmp/swagger-petstore-3-sdk-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swagger-petstore-3-sdk-2.0.1.tar", last modified: Thu Jun  1 08:10:33 2023, max compression
+gzip compressed data, was "swagger-petstore-3-sdk-2.0.2.tar", last modified: Thu Jun  1 08:57:18 2023, max compression
```

## Comparing `swagger-petstore-3-sdk-2.0.1.tar` & `swagger-petstore-3-sdk-2.0.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 08:10:33.489822 swagger-petstore-3-sdk-2.0.1/
--rw-r--r--   0 root         (0) root         (0)     1213 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      422 2023-06-01 08:10:33.489822 swagger-petstore-3-sdk-2.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4212 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)     4647 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       77 2023-06-01 08:10:33.490822 swagger-petstore-3-sdk-2.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 08:10:33.460822 swagger-petstore-3-sdk-2.0.1/swagger_petstore_3_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      422 2023-06-01 08:10:33.000000 swagger-petstore-3-sdk-2.0.1/swagger_petstore_3_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1811 2023-06-01 08:10:33.000000 swagger-petstore-3-sdk-2.0.1/swagger_petstore_3_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 08:10:33.000000 swagger-petstore-3-sdk-2.0.1/swagger_petstore_3_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      164 2023-06-01 08:10:33.000000 swagger-petstore-3-sdk-2.0.1/swagger_petstore_3_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-06-01 08:10:33.000000 swagger-petstore-3-sdk-2.0.1/swagger_petstore_3_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 08:10:33.463822 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/
--rw-r--r--   0 root         (0) root         (0)      163 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/__init__.py
--rw-r--r--   0 root         (0) root         (0)      567 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/api_helper.py
--rw-r--r--   0 root         (0) root         (0)     4155 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 08:10:33.467822 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/controllers/
--rw-r--r--   0 root         (0) root         (0)      110 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1990 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/controllers/base_controller.py
--rw-r--r--   0 root         (0) root         (0)    15580 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/controllers/pet_controller.py
--rw-r--r--   0 root         (0) root         (0)     7469 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/controllers/store_controller.py
--rw-r--r--   0 root         (0) root         (0)    13430 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/controllers/user_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 08:10:33.469823 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/exceptions/
--rw-r--r--   0 root         (0) root         (0)       36 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/exceptions/api_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 08:10:33.476822 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/http/
--rw-r--r--   0 root         (0) root         (0)      118 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/http/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 08:10:33.477822 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/http/auth/
--rw-r--r--   0 root         (0) root         (0)       51 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/http/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      726 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/http/auth/custom_header_authentication.py
--rw-r--r--   0 root         (0) root         (0)      486 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/http/http_call_back.py
--rw-r--r--   0 root         (0) root         (0)      493 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/http/http_method_enum.py
--rw-r--r--   0 root         (0) root         (0)     1875 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/http/http_request.py
--rw-r--r--   0 root         (0) root         (0)     1496 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/http/http_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 08:10:33.488823 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/
--rw-r--r--   0 root         (0) root         (0)      203 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2536 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/address.py
--rw-r--r--   0 root         (0) root         (0)     1861 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/category.py
--rw-r--r--   0 root         (0) root         (0)     2452 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/customer.py
--rw-r--r--   0 root         (0) root         (0)     3417 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/order.py
--rw-r--r--   0 root         (0) root         (0)      518 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/order_status_enum.py
--rw-r--r--   0 root         (0) root         (0)     3397 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/pet.py
--rw-r--r--   0 root         (0) root         (0)     2241 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/pet_image.py
--rw-r--r--   0 root         (0) root         (0)      516 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/pet_status_enum.py
--rw-r--r--   0 root         (0) root         (0)      520 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/status_enum.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/tag.py
--rw-r--r--   0 root         (0) root         (0)     4052 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/user.py
--rw-r--r--   0 root         (0) root         (0)     3298 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/swaggerpetstoreopenapi_30_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 08:10:33.489822 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/utilities/
--rw-r--r--   0 root         (0) root         (0)       35 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      441 2023-06-01 08:10:08.000000 swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/utilities/file_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 08:57:18.945323 swagger-petstore-3-sdk-2.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4603 2023-06-01 08:57:18.945323 swagger-petstore-3-sdk-2.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4212 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      778 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       77 2023-06-01 08:57:18.947323 swagger-petstore-3-sdk-2.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 08:57:18.924323 swagger-petstore-3-sdk-2.0.2/swagger_petstore_3_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4603 2023-06-01 08:57:18.000000 swagger-petstore-3-sdk-2.0.2/swagger_petstore_3_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-06-01 08:57:18.000000 swagger-petstore-3-sdk-2.0.2/swagger_petstore_3_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 08:57:18.000000 swagger-petstore-3-sdk-2.0.2/swagger_petstore_3_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      164 2023-06-01 08:57:18.000000 swagger-petstore-3-sdk-2.0.2/swagger_petstore_3_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-01 08:57:18.000000 swagger-petstore-3-sdk-2.0.2/swagger_petstore_3_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 08:57:18.928323 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/
+-rw-r--r--   0 root         (0) root         (0)      163 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      567 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/api_helper.py
+-rw-r--r--   0 root         (0) root         (0)     4155 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 08:57:18.931323 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/controllers/
+-rw-r--r--   0 root         (0) root         (0)      110 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1990 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/controllers/base_controller.py
+-rw-r--r--   0 root         (0) root         (0)    15580 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/controllers/pet_controller.py
+-rw-r--r--   0 root         (0) root         (0)     7469 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/controllers/store_controller.py
+-rw-r--r--   0 root         (0) root         (0)    13430 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/controllers/user_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 08:57:18.932323 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/exceptions/
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/exceptions/api_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 08:57:18.935323 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/http/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/http/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 08:57:18.936323 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/http/auth/
+-rw-r--r--   0 root         (0) root         (0)       51 2023-06-01 08:56:48.000000 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/http/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      726 2023-06-01 08:56:48.000000 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/http/auth/custom_header_authentication.py
+-rw-r--r--   0 root         (0) root         (0)      486 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/http/http_call_back.py
+-rw-r--r--   0 root         (0) root         (0)      493 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/http/http_method_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1875 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/http/http_request.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/http/http_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 08:57:18.943323 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/models/
+-rw-r--r--   0 root         (0) root         (0)      203 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2536 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/models/address.py
+-rw-r--r--   0 root         (0) root         (0)     1861 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/models/category.py
+-rw-r--r--   0 root         (0) root         (0)     2452 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/models/customer.py
+-rw-r--r--   0 root         (0) root         (0)     3417 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/models/order.py
+-rw-r--r--   0 root         (0) root         (0)      518 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/models/order_status_enum.py
+-rw-r--r--   0 root         (0) root         (0)     3397 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/models/pet.py
+-rw-r--r--   0 root         (0) root         (0)     2241 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/models/pet_image.py
+-rw-r--r--   0 root         (0) root         (0)      516 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/models/pet_status_enum.py
+-rw-r--r--   0 root         (0) root         (0)      520 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/models/status_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/models/tag.py
+-rw-r--r--   0 root         (0) root         (0)     4052 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/models/user.py
+-rw-r--r--   0 root         (0) root         (0)     3298 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/swaggerpetstoreopenapi_30_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 08:57:18.944323 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/utilities/
+-rw-r--r--   0 root         (0) root         (0)       35 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      441 2023-06-01 08:56:47.000000 swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/utilities/file_wrapper.py
```

### Comparing `swagger-petstore-3-sdk-2.0.1/LICENSE` & `swagger-petstore-3-sdk-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-2.0.1/README.md` & `swagger-petstore-3-sdk-2.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -19,34 +19,34 @@
 
 ## Install the Package
 
 The package is compatible with Python versions `3 >=3.7, <= 3.11`.
 Install the package from PyPi using the following pip command:
 
 ```python
-pip install swagger-petstore-3-sdk==2.0.1
+pip install swagger-petstore-3-sdk==2.0.2
 ```
 
 You can also view the package at:
-https://pypi.python.org/pypi/swagger-petstore-3-sdk/2.0.1
+https://pypi.python.org/pypi/swagger-petstore-3-sdk/2.0.2
 
 ## Test the SDK
 
 You can test the generated SDK and the server with test cases. `unittest` is used as the testing framework and `pytest` is used as the test runner. You can run the tests as follows:
 
 Navigate to the root directory of the SDK and run the following commands
 
 ```
 pip install -r test-requirements.txt
 pytest
 ```
 
 ## Initialize the API Client
 
-**_Note:_** Documentation for the client can be found [here.](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/2.0.1/doc/client.md)
+**_Note:_** Documentation for the client can be found [here.](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/2.0.2/doc/client.md)
 
 The following parameters are configurable for the API Client:
 
 | Parameter | Type | Description |
 |  --- | --- | --- |
 | `http_client_instance` | `HttpClient` | The Http Client passed from the sdk user for making requests |
 | `override_http_client_configuration` | `bool` | The value which determines to override properties of the passed Http Client from the sdk user |
@@ -72,17 +72,17 @@
 
 ## Authorization
 
 This API uses `Custom Header Signature`.
 
 ## List of APIs
 
-* [Pet](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/2.0.1/doc/controllers/pet.md)
-* [Store](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/2.0.1/doc/controllers/store.md)
-* [User](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/2.0.1/doc/controllers/user.md)
+* [Pet](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/2.0.2/doc/controllers/pet.md)
+* [Store](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/2.0.2/doc/controllers/store.md)
+* [User](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/2.0.2/doc/controllers/user.md)
 
 ## Classes Documentation
 
-* [Utility Classes](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/2.0.1/doc/utility-classes.md)
-* [HttpResponse](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/2.0.1/doc/http-response.md)
-* [HttpRequest](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/2.0.1/doc/http-request.md)
+* [Utility Classes](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/2.0.2/doc/utility-classes.md)
+* [HttpResponse](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/2.0.2/doc/http-response.md)
+* [HttpRequest](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/2.0.2/doc/http-request.md)
```

### Comparing `swagger-petstore-3-sdk-2.0.1/pyproject.toml` & `swagger-petstore-3-sdk-2.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,100 @@
-[build-system]
-build-backend = "setuptools.build_meta"
-requires = ["setuptools>=61.0"]
-[project]
-name = "swagger-petstore-3-sdk"
-description = "## Swagger Petstore - OpenAPI 3.0\n\nSwagger Petstore OpenAPI 3.0 package for PyPI is a powerful and user-friendly Python library that simplifies the integration and interaction with the Swagger Petstore API. It provides client functions, data models, error handling capabilities, authentication support, comprehensive documentation, and PyPI compatibility. By utilizing this package, developers can seamlessly consume and manage pet resources from the Swagger Petstore API in their Python applications.\n\n## Install the Package\n\nThe package is compatible with Python versions `3 >=3.7, <= 3.11`.\nInstall the package from PyPi using the following pip command:\n\n```python\npip install swagger-petstore-3-sdk==1.0.4\n```\n\nYou can also view the package at:\nhttps://pypi.python.org/pypi/swagger-petstore-3-sdk/1.0.4\n\n## Test the SDK\n\nYou can test the generated SDK and the server with test cases. `unittest` is used as the testing framework and `pytest` is used as the test runner. You can run the tests as follows:\n\nNavigate to the root directory of the SDK and run the following commands\n\n```\npip install -r test-requirements.txt\npytest\n```\n\n## Initialize the API Client\n\n**_Note:_** Documentation for the client can be found [here.](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/1.0.4/doc/client.md)\n\nThe following parameters are configurable for the API Client:\n\n| Parameter | Type | Description |\n|  --- | --- | --- |\n| `http_client_instance` | `HttpClient` | The Http Client passed from the sdk user for making requests |\n| `override_http_client_configuration` | `bool` | The value which determines to override properties of the passed Http Client from the sdk user |\n| `http_call_back` | `HttpCallBack` | The callback value that is invoked before and after an HTTP call is made to an endpoint |\n| `timeout` | `float` | The value to use for connection timeout. <br> **Default: 60** |\n| `max_retries` | `int` | The number of times to retry an endpoint call if it fails. <br> **Default: 0** |\n| `backoff_factor` | `float` | A backoff factor to apply between attempts after the second try. <br> **Default: 2** |\n| `retry_statuses` | `Array of int` | The http statuses on which retry is to be done. <br> **Default: [408, 413, 429, 500, 502, 503, 504, 521, 522, 524]** |\n| `retry_methods` | `Array of string` | The http methods on which retry is to be done. <br> **Default: ['GET', 'PUT']** |\n| `api_key` | `string` |  |\n\nThe API client can be initialized as follows:\n\n```python\nfrom swaggerpetstoreopenapi30.swaggerpetstoreopenapi_30_client import Swaggerpetstoreopenapi30Client\nfrom swaggerpetstoreopenapi30.configuration import Environment\n\nclient = Swaggerpetstoreopenapi30Client(\n    api_key='api_key',\n    environment=Environment.PRODUCTION\n)\n```\n\n## Authorization\n\nThis API uses `Custom Header Signature`.\n\n## List of APIs\n\n* [Pet](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/1.0.4/doc/controllers/pet.md)\n* [Store](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/1.0.4/doc/controllers/store.md)\n* [User](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/1.0.4/doc/controllers/user.md)\n\n## Classes Documentation\n\n* [Utility Classes](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/1.0.4/doc/utility-classes.md)\n* [HttpResponse](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/1.0.4/doc/http-response.md)\n* [HttpRequest](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/1.0.4/doc/http-request.md)\n\n\n## Cloning the repository\nYou can clone the `swagger-petstore-3-0-python-sdk` by doing:\n\n```\ngit clone https://github.com/moizgillani/swagger-petstore-3-0-python-sdk.git\n```\n\nYou can also view the package at:\nhttps://github.com/moizgillani/swagger-petstore-3-0-python-sdk"
-version = "2.0.1"
-requires-python = ">=3.7"
-keywords = ["OpenAPI", "swagger", "apimatic", "petstore"]
-authors = [{name = "Apimatic Developer", email = "developer@apimatic.io"}]
-urls = {Documentation = "https://dev.apimatic.io/api-docs-preview/dashboard/647726e85a75e59f9aa0ed19/v/1_0_11#/http/step-by-step-tutorial"}
-dependencies = ["apimatic-core~=0.2.0", "apimatic-core-interfaces~=0.1.0", "apimatic-requests-client-adapter~=0.1.0", "python-dateutil~=2.8.1", "enum34~=1.1, >=1.1.10"]
-classifiers = []
-[project.optional-dependencies]
-testutils = ["pytest>=7.2.2"]
+Metadata-Version: 2.1
+Name: swagger-petstore-3-sdk
+Version: 2.0.2
+Summary: Swagger Petstore - OpenAPI 3.0
+Author-email: Apimatic Developer <developer@apimatic.io>
+Project-URL: Documentation, https://dev.apimatic.io/api-docs-preview/dashboard/647726e85a75e59f9aa0ed19/v/1_0_11#/http/step-by-step-tutorial
+Keywords: OpenAPI,swagger,apimatic,petstore
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: testutils
+License-File: LICENSE
+
+
+# Getting Started with Swagger Petstore - OpenAPI 3.0
+
+## Introduction
+
+This is a sample Pet Store Server based on the OpenAPI 3.0 specification.  You can find out more about
+Swagger at [https://swagger.io](https://swagger.io). In the third iteration of the pet store, we've switched to the design first approach!
+You can now help us improve the API whether it's by making changes to the definition itself or to the code.
+That way, with time, we can improve the API in general, and expose some of the new features in OAS3.
+
+_If you're looking for the Swagger 2.0/OAS 2.0 version of Petstore, then click [here](https://editor.swagger.io/?url=https://petstore.swagger.io/v2/swagger.yaml). Alternatively, you can load via the `Edit > Load Petstore OAS 2.0` menu option!_
+
+Some useful links:
+
+- [The Pet Store repository](https://github.com/swagger-api/swagger-petstore)
+- [The source API definition for the Pet Store](https://github.com/swagger-api/swagger-petstore/blob/master/src/main/resources/openapi.yaml)
+
+Find out more about Swagger: [http://swagger.io](http://swagger.io)
+
+## Install the Package
+
+The package is compatible with Python versions `3 >=3.7, <= 3.11`.
+Install the package from PyPi using the following pip command:
+
+```python
+pip install swagger-petstore-3-sdk==2.0.2
+```
+
+You can also view the package at:
+https://pypi.python.org/pypi/swagger-petstore-3-sdk/2.0.2
+
+## Test the SDK
+
+You can test the generated SDK and the server with test cases. `unittest` is used as the testing framework and `pytest` is used as the test runner. You can run the tests as follows:
+
+Navigate to the root directory of the SDK and run the following commands
+
+```
+pip install -r test-requirements.txt
+pytest
+```
+
+## Initialize the API Client
+
+**_Note:_** Documentation for the client can be found [here.](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/2.0.2/doc/client.md)
+
+The following parameters are configurable for the API Client:
+
+| Parameter | Type | Description |
+|  --- | --- | --- |
+| `http_client_instance` | `HttpClient` | The Http Client passed from the sdk user for making requests |
+| `override_http_client_configuration` | `bool` | The value which determines to override properties of the passed Http Client from the sdk user |
+| `http_call_back` | `HttpCallBack` | The callback value that is invoked before and after an HTTP call is made to an endpoint |
+| `timeout` | `float` | The value to use for connection timeout. <br> **Default: 60** |
+| `max_retries` | `int` | The number of times to retry an endpoint call if it fails. <br> **Default: 0** |
+| `backoff_factor` | `float` | A backoff factor to apply between attempts after the second try. <br> **Default: 2** |
+| `retry_statuses` | `Array of int` | The http statuses on which retry is to be done. <br> **Default: [408, 413, 429, 500, 502, 503, 504, 521, 522, 524]** |
+| `retry_methods` | `Array of string` | The http methods on which retry is to be done. <br> **Default: ['GET', 'PUT']** |
+| `api_key` | `string` |  |
+
+The API client can be initialized as follows:
+
+```python
+from swaggerpetstoreopenapi30.swaggerpetstoreopenapi_30_client import Swaggerpetstoreopenapi30Client
+from swaggerpetstoreopenapi30.configuration import Environment
+
+client = Swaggerpetstoreopenapi30Client(
+    api_key='api_key',
+    environment=Environment.PRODUCTION
+)
+```
+
+## Authorization
+
+This API uses `Custom Header Signature`.
+
+## List of APIs
+
+* [Pet](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/2.0.2/doc/controllers/pet.md)
+* [Store](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/2.0.2/doc/controllers/store.md)
+* [User](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/2.0.2/doc/controllers/user.md)
+
+## Classes Documentation
+
+* [Utility Classes](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/2.0.2/doc/utility-classes.md)
+* [HttpResponse](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/2.0.2/doc/http-response.md)
+* [HttpRequest](https://www.github.com/moizgillani/swagger-petstore-3-0-python-sdk/tree/2.0.2/doc/http-request.md)
+
```

### Comparing `swagger-petstore-3-sdk-2.0.1/swagger_petstore_3_sdk.egg-info/SOURCES.txt` & `swagger-petstore-3-sdk-2.0.2/swagger_petstore_3_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/api_helper.py` & `swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/api_helper.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/configuration.py` & `swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/configuration.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/controllers/base_controller.py` & `swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/controllers/pet_controller.py` & `swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/controllers/pet_controller.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/controllers/store_controller.py` & `swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/controllers/store_controller.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/controllers/user_controller.py` & `swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/controllers/user_controller.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/exceptions/api_exception.py` & `swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/http/auth/custom_header_authentication.py` & `swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/http/auth/custom_header_authentication.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/http/http_request.py` & `swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/http/http_request.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/http/http_response.py` & `swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/http/http_response.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/address.py` & `swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/models/address.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/category.py` & `swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/models/category.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/customer.py` & `swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/models/customer.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/order.py` & `swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/models/order.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/order_status_enum.py` & `swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/models/order_status_enum.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/pet.py` & `swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/models/pet.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/pet_image.py` & `swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/models/pet_image.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/pet_status_enum.py` & `swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/models/pet_status_enum.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/status_enum.py` & `swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/models/status_enum.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/tag.py` & `swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/models/tag.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/models/user.py` & `swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/models/user.py`

 * *Files identical despite different names*

### Comparing `swagger-petstore-3-sdk-2.0.1/swaggerpetstoreopenapi30/swaggerpetstoreopenapi_30_client.py` & `swagger-petstore-3-sdk-2.0.2/swaggerpetstoreopenapi30/swaggerpetstoreopenapi_30_client.py`

 * *Files identical despite different names*

