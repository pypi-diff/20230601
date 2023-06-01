# Comparing `tmp/mypy-boto3-alexaforbusiness-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-alexaforbusiness-1.26.145.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-alexaforbusiness-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:01 2022, max compression
+gzip compressed data, was "mypy-boto3-alexaforbusiness-1.26.145.tar", last modified: Thu Jun  1 19:32:38 2023, max compression
```

## Comparing `mypy-boto3-alexaforbusiness-1.26.0.post1.tar` & `mypy-boto3-alexaforbusiness-1.26.145.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:01.392824 mypy-boto3-alexaforbusiness-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:30:05.000000 mypy-boto3-alexaforbusiness-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    24128 2022-11-01 21:43:01.388824 mypy-boto3-alexaforbusiness-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    22651 2022-11-01 21:30:05.000000 mypy-boto3-alexaforbusiness-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:01.384824 mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness/
--rw-r--r--   0 runner    (1001) docker     (121)     3262 2022-11-01 21:30:05.000000 mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3261 2022-11-01 21:30:05.000000 mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      953 2022-11-01 21:30:05.000000 mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    67440 2022-11-01 21:30:05.000000 mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    67327 2022-11-01 21:30:05.000000 mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    11895 2022-11-01 21:30:05.000000 mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    11893 2022-11-01 21:30:05.000000 mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    16333 2022-11-01 21:30:05.000000 mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)    16318 2022-11-01 21:30:05.000000 mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:30:05.000000 mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    70780 2022-11-01 21:30:07.000000 mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    70705 2022-11-01 21:30:06.000000 mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:30:05.000000 mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:01.388824 mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    24128 2022-11-01 21:43:01.000000 mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-11-01 21:43:01.000000 mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:01.000000 mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:01.000000 mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:01.000000 mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-11-01 21:43:01.000000 mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:01.392824 mypy-boto3-alexaforbusiness-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2031 2022-11-01 21:30:04.000000 mypy-boto3-alexaforbusiness-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:32:38.630084 mypy-boto3-alexaforbusiness-1.26.145/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-01 19:31:50.000000 mypy-boto3-alexaforbusiness-1.26.145/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24255 2023-06-01 19:32:38.630084 mypy-boto3-alexaforbusiness-1.26.145/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22730 2023-06-01 19:31:50.000000 mypy-boto3-alexaforbusiness-1.26.145/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:32:38.626083 mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness/
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-06-01 19:31:50.000000 mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-01 19:31:50.000000 mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-01 19:31:50.000000 mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67440 2023-06-01 19:31:50.000000 mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67327 2023-06-01 19:31:50.000000 mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-06-01 19:31:51.000000 mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-06-01 19:31:50.000000 mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16333 2023-06-01 19:31:50.000000 mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16318 2023-06-01 19:31:50.000000 mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:31:50.000000 mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    71403 2023-06-01 19:31:52.000000 mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71328 2023-06-01 19:31:52.000000 mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-01 19:31:50.000000 mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:32:38.630084 mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24255 2023-06-01 19:32:38.000000 mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-01 19:32:38.000000 mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 19:32:38.000000 mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 19:32:38.000000 mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-01 19:32:38.000000 mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-01 19:32:38.000000 mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 19:32:38.630084 mypy-boto3-alexaforbusiness-1.26.145/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-01 19:31:50.000000 mypy-boto3-alexaforbusiness-1.26.145/setup.py
```

### Comparing `mypy-boto3-alexaforbusiness-1.26.0.post1/LICENSE` & `mypy-boto3-alexaforbusiness-1.26.145/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Vlad Emelianov
+Copyright (c) 2023 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-alexaforbusiness-1.26.0.post1/PKG-INFO` & `mypy-boto3-alexaforbusiness-1.26.145/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-alexaforbusiness
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.AlexaForBusiness 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.145
+Summary: Type annotations for boto3.AlexaForBusiness 1.26.145 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_alexaforbusiness/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,43 +18,44 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-alexaforbusiness"></a>
 
 # mypy-boto3-alexaforbusiness
 
 [![PyPI - mypy-boto3-alexaforbusiness](https://img.shields.io/pypi/v/mypy-boto3-alexaforbusiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-alexaforbusiness)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-alexaforbusiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-alexaforbusiness)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_alexaforbusiness/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-alexaforbusiness?color=blue)](https://pypistats.org/packages/mypy-boto3-alexaforbusiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AlexaForBusiness 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
+[boto3.AlexaForBusiness 1.26.145](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-alexaforbusiness docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_alexaforbusiness/).
 
 See how it helps to find and fix potential bugs:
 
@@ -423,14 +424,15 @@
     SipAddressTypeDef,
     SsmlTypeDef,
     TextTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     CreateEndOfMeetingReminderTypeDef,
     CreateInstantBookingTypeDef,
+    CreateProactiveJoinTypeDef,
     CreateRequireCheckInTypeDef,
     DeleteAddressBookRequestRequestTypeDef,
     DeleteBusinessReportScheduleRequestRequestTypeDef,
     DeleteConferenceProviderRequestRequestTypeDef,
     DeleteContactRequestRequestTypeDef,
     DeleteDeviceRequestRequestTypeDef,
     DeleteDeviceUsageDataRequestRequestTypeDef,
@@ -483,14 +485,15 @@
     ListSkillsRequestRequestTypeDef,
     SkillSummaryTypeDef,
     ListSkillsStoreCategoriesRequestRequestTypeDef,
     ListSkillsStoreSkillsByCategoryRequestRequestTypeDef,
     ListSmartHomeAppliancesRequestRequestTypeDef,
     SmartHomeApplianceTypeDef,
     ListTagsRequestRequestTypeDef,
+    ProactiveJoinTypeDef,
     RequireCheckInTypeDef,
     NetworkProfileDataTypeDef,
     ProfileDataTypeDef,
     PutInvitationConfigurationRequestRequestTypeDef,
     PutSkillAuthorizationRequestRequestTypeDef,
     RejectSkillRequestRequestTypeDef,
     ResolveRoomRequestRequestTypeDef,
@@ -505,14 +508,15 @@
     UntagResourceRequestRequestTypeDef,
     UpdateAddressBookRequestRequestTypeDef,
     UpdateDeviceRequestRequestTypeDef,
     UpdateEndOfMeetingReminderTypeDef,
     UpdateGatewayGroupRequestRequestTypeDef,
     UpdateGatewayRequestRequestTypeDef,
     UpdateInstantBookingTypeDef,
+    UpdateProactiveJoinTypeDef,
     UpdateRequireCheckInTypeDef,
     UpdateNetworkProfileRequestRequestTypeDef,
     UpdateRoomRequestRequestTypeDef,
     UpdateSkillGroupRequestRequestTypeDef,
     UpdateBusinessReportScheduleRequestRequestTypeDef,
     BusinessReportTypeDef,
     PutConferencePreferenceRequestRequestTypeDef,
@@ -622,42 +626,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-alexaforbusiness-1.26.0.post1/README.md` & `mypy-boto3-alexaforbusiness-1.26.145/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-alexaforbusiness"></a>
 
 # mypy-boto3-alexaforbusiness
 
 [![PyPI - mypy-boto3-alexaforbusiness](https://img.shields.io/pypi/v/mypy-boto3-alexaforbusiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-alexaforbusiness)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-alexaforbusiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-alexaforbusiness)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_alexaforbusiness/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-alexaforbusiness?color=blue)](https://pypistats.org/packages/mypy-boto3-alexaforbusiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AlexaForBusiness 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
+[boto3.AlexaForBusiness 1.26.145](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-alexaforbusiness docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_alexaforbusiness/).
 
 See how it helps to find and fix potential bugs:
 
@@ -392,14 +392,15 @@
     SipAddressTypeDef,
     SsmlTypeDef,
     TextTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     CreateEndOfMeetingReminderTypeDef,
     CreateInstantBookingTypeDef,
+    CreateProactiveJoinTypeDef,
     CreateRequireCheckInTypeDef,
     DeleteAddressBookRequestRequestTypeDef,
     DeleteBusinessReportScheduleRequestRequestTypeDef,
     DeleteConferenceProviderRequestRequestTypeDef,
     DeleteContactRequestRequestTypeDef,
     DeleteDeviceRequestRequestTypeDef,
     DeleteDeviceUsageDataRequestRequestTypeDef,
@@ -452,14 +453,15 @@
     ListSkillsRequestRequestTypeDef,
     SkillSummaryTypeDef,
     ListSkillsStoreCategoriesRequestRequestTypeDef,
     ListSkillsStoreSkillsByCategoryRequestRequestTypeDef,
     ListSmartHomeAppliancesRequestRequestTypeDef,
     SmartHomeApplianceTypeDef,
     ListTagsRequestRequestTypeDef,
+    ProactiveJoinTypeDef,
     RequireCheckInTypeDef,
     NetworkProfileDataTypeDef,
     ProfileDataTypeDef,
     PutInvitationConfigurationRequestRequestTypeDef,
     PutSkillAuthorizationRequestRequestTypeDef,
     RejectSkillRequestRequestTypeDef,
     ResolveRoomRequestRequestTypeDef,
@@ -474,14 +476,15 @@
     UntagResourceRequestRequestTypeDef,
     UpdateAddressBookRequestRequestTypeDef,
     UpdateDeviceRequestRequestTypeDef,
     UpdateEndOfMeetingReminderTypeDef,
     UpdateGatewayGroupRequestRequestTypeDef,
     UpdateGatewayRequestRequestTypeDef,
     UpdateInstantBookingTypeDef,
+    UpdateProactiveJoinTypeDef,
     UpdateRequireCheckInTypeDef,
     UpdateNetworkProfileRequestRequestTypeDef,
     UpdateRoomRequestRequestTypeDef,
     UpdateSkillGroupRequestRequestTypeDef,
     UpdateBusinessReportScheduleRequestRequestTypeDef,
     BusinessReportTypeDef,
     PutConferencePreferenceRequestRequestTypeDef,
@@ -591,42 +594,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness/__init__.py` & `mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness/__init__.pyi` & `mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness/__main__.py` & `mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AlexaForBusiness 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.AlexaForBusiness 1.26.145\nVersion:         1.26.145\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_alexaforbusiness//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.0.post1")
+    print("1.26.145")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness/client.py` & `mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness/client.pyi` & `mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness/literals.py` & `mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,14 +166,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -183,27 +184,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -232,14 +237,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -284,51 +290,57 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -341,14 +353,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -360,28 +373,33 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -390,14 +408,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -408,55 +427,63 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness/literals.pyi` & `mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -164,14 +164,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -181,27 +182,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -230,14 +235,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -282,51 +288,57 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -339,14 +351,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -358,28 +371,33 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -388,14 +406,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -406,55 +425,63 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness/paginator.py` & `mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness/paginator.pyi` & `mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness/type_defs.py` & `mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,14 +75,15 @@
     "SipAddressTypeDef",
     "SsmlTypeDef",
     "TextTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "CreateEndOfMeetingReminderTypeDef",
     "CreateInstantBookingTypeDef",
+    "CreateProactiveJoinTypeDef",
     "CreateRequireCheckInTypeDef",
     "DeleteAddressBookRequestRequestTypeDef",
     "DeleteBusinessReportScheduleRequestRequestTypeDef",
     "DeleteConferenceProviderRequestRequestTypeDef",
     "DeleteContactRequestRequestTypeDef",
     "DeleteDeviceRequestRequestTypeDef",
     "DeleteDeviceUsageDataRequestRequestTypeDef",
@@ -135,14 +136,15 @@
     "ListSkillsRequestRequestTypeDef",
     "SkillSummaryTypeDef",
     "ListSkillsStoreCategoriesRequestRequestTypeDef",
     "ListSkillsStoreSkillsByCategoryRequestRequestTypeDef",
     "ListSmartHomeAppliancesRequestRequestTypeDef",
     "SmartHomeApplianceTypeDef",
     "ListTagsRequestRequestTypeDef",
+    "ProactiveJoinTypeDef",
     "RequireCheckInTypeDef",
     "NetworkProfileDataTypeDef",
     "ProfileDataTypeDef",
     "PutInvitationConfigurationRequestRequestTypeDef",
     "PutSkillAuthorizationRequestRequestTypeDef",
     "RejectSkillRequestRequestTypeDef",
     "ResolveRoomRequestRequestTypeDef",
@@ -157,14 +159,15 @@
     "UntagResourceRequestRequestTypeDef",
     "UpdateAddressBookRequestRequestTypeDef",
     "UpdateDeviceRequestRequestTypeDef",
     "UpdateEndOfMeetingReminderTypeDef",
     "UpdateGatewayGroupRequestRequestTypeDef",
     "UpdateGatewayRequestRequestTypeDef",
     "UpdateInstantBookingTypeDef",
+    "UpdateProactiveJoinTypeDef",
     "UpdateRequireCheckInTypeDef",
     "UpdateNetworkProfileRequestRequestTypeDef",
     "UpdateRoomRequestRequestTypeDef",
     "UpdateSkillGroupRequestRequestTypeDef",
     "UpdateBusinessReportScheduleRequestRequestTypeDef",
     "BusinessReportTypeDef",
     "PutConferencePreferenceRequestRequestTypeDef",
@@ -494,14 +497,21 @@
     "CreateInstantBookingTypeDef",
     {
         "DurationInMinutes": int,
         "Enabled": bool,
     },
 )
 
+CreateProactiveJoinTypeDef = TypedDict(
+    "CreateProactiveJoinTypeDef",
+    {
+        "EnabledByMotion": bool,
+    },
+)
+
 CreateRequireCheckInTypeDef = TypedDict(
     "CreateRequireCheckInTypeDef",
     {
         "ReleaseAfterMinutes": int,
         "Enabled": bool,
     },
 )
@@ -1146,14 +1156,22 @@
 
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
 ):
     pass
 
 
+ProactiveJoinTypeDef = TypedDict(
+    "ProactiveJoinTypeDef",
+    {
+        "EnabledByMotion": bool,
+    },
+    total=False,
+)
+
 RequireCheckInTypeDef = TypedDict(
     "RequireCheckInTypeDef",
     {
         "ReleaseAfterMinutes": int,
         "Enabled": bool,
     },
     total=False,
@@ -1440,14 +1458,21 @@
     {
         "DurationInMinutes": int,
         "Enabled": bool,
     },
     total=False,
 )
 
+UpdateProactiveJoinTypeDef = TypedDict(
+    "UpdateProactiveJoinTypeDef",
+    {
+        "EnabledByMotion": bool,
+    },
+)
+
 UpdateRequireCheckInTypeDef = TypedDict(
     "UpdateRequireCheckInTypeDef",
     {
         "ReleaseAfterMinutes": int,
         "Enabled": bool,
     },
     total=False,
@@ -2069,14 +2094,15 @@
 CreateMeetingRoomConfigurationTypeDef = TypedDict(
     "CreateMeetingRoomConfigurationTypeDef",
     {
         "RoomUtilizationMetricsEnabled": bool,
         "EndOfMeetingReminder": CreateEndOfMeetingReminderTypeDef,
         "InstantBooking": CreateInstantBookingTypeDef,
         "RequireCheckIn": CreateRequireCheckInTypeDef,
+        "ProactiveJoin": CreateProactiveJoinTypeDef,
     },
     total=False,
 )
 
 SkillDetailsTypeDef = TypedDict(
     "SkillDetailsTypeDef",
     {
@@ -2356,14 +2382,15 @@
 MeetingRoomConfigurationTypeDef = TypedDict(
     "MeetingRoomConfigurationTypeDef",
     {
         "RoomUtilizationMetricsEnabled": bool,
         "EndOfMeetingReminder": EndOfMeetingReminderTypeDef,
         "InstantBooking": InstantBookingTypeDef,
         "RequireCheckIn": RequireCheckInTypeDef,
+        "ProactiveJoin": ProactiveJoinTypeDef,
     },
     total=False,
 )
 
 SearchNetworkProfilesResponseTypeDef = TypedDict(
     "SearchNetworkProfilesResponseTypeDef",
     {
@@ -2555,14 +2582,15 @@
 UpdateMeetingRoomConfigurationTypeDef = TypedDict(
     "UpdateMeetingRoomConfigurationTypeDef",
     {
         "RoomUtilizationMetricsEnabled": bool,
         "EndOfMeetingReminder": UpdateEndOfMeetingReminderTypeDef,
         "InstantBooking": UpdateInstantBookingTypeDef,
         "RequireCheckIn": UpdateRequireCheckInTypeDef,
+        "ProactiveJoin": UpdateProactiveJoinTypeDef,
     },
     total=False,
 )
 
 BusinessReportScheduleTypeDef = TypedDict(
     "BusinessReportScheduleTypeDef",
     {
```

### Comparing `mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness/type_defs.pyi` & `mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
     "SipAddressTypeDef",
     "SsmlTypeDef",
     "TextTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "CreateEndOfMeetingReminderTypeDef",
     "CreateInstantBookingTypeDef",
+    "CreateProactiveJoinTypeDef",
     "CreateRequireCheckInTypeDef",
     "DeleteAddressBookRequestRequestTypeDef",
     "DeleteBusinessReportScheduleRequestRequestTypeDef",
     "DeleteConferenceProviderRequestRequestTypeDef",
     "DeleteContactRequestRequestTypeDef",
     "DeleteDeviceRequestRequestTypeDef",
     "DeleteDeviceUsageDataRequestRequestTypeDef",
@@ -134,14 +135,15 @@
     "ListSkillsRequestRequestTypeDef",
     "SkillSummaryTypeDef",
     "ListSkillsStoreCategoriesRequestRequestTypeDef",
     "ListSkillsStoreSkillsByCategoryRequestRequestTypeDef",
     "ListSmartHomeAppliancesRequestRequestTypeDef",
     "SmartHomeApplianceTypeDef",
     "ListTagsRequestRequestTypeDef",
+    "ProactiveJoinTypeDef",
     "RequireCheckInTypeDef",
     "NetworkProfileDataTypeDef",
     "ProfileDataTypeDef",
     "PutInvitationConfigurationRequestRequestTypeDef",
     "PutSkillAuthorizationRequestRequestTypeDef",
     "RejectSkillRequestRequestTypeDef",
     "ResolveRoomRequestRequestTypeDef",
@@ -156,14 +158,15 @@
     "UntagResourceRequestRequestTypeDef",
     "UpdateAddressBookRequestRequestTypeDef",
     "UpdateDeviceRequestRequestTypeDef",
     "UpdateEndOfMeetingReminderTypeDef",
     "UpdateGatewayGroupRequestRequestTypeDef",
     "UpdateGatewayRequestRequestTypeDef",
     "UpdateInstantBookingTypeDef",
+    "UpdateProactiveJoinTypeDef",
     "UpdateRequireCheckInTypeDef",
     "UpdateNetworkProfileRequestRequestTypeDef",
     "UpdateRoomRequestRequestTypeDef",
     "UpdateSkillGroupRequestRequestTypeDef",
     "UpdateBusinessReportScheduleRequestRequestTypeDef",
     "BusinessReportTypeDef",
     "PutConferencePreferenceRequestRequestTypeDef",
@@ -491,14 +494,21 @@
     "CreateInstantBookingTypeDef",
     {
         "DurationInMinutes": int,
         "Enabled": bool,
     },
 )
 
+CreateProactiveJoinTypeDef = TypedDict(
+    "CreateProactiveJoinTypeDef",
+    {
+        "EnabledByMotion": bool,
+    },
+)
+
 CreateRequireCheckInTypeDef = TypedDict(
     "CreateRequireCheckInTypeDef",
     {
         "ReleaseAfterMinutes": int,
         "Enabled": bool,
     },
 )
@@ -1125,14 +1135,22 @@
 )
 
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
 ):
     pass
 
+ProactiveJoinTypeDef = TypedDict(
+    "ProactiveJoinTypeDef",
+    {
+        "EnabledByMotion": bool,
+    },
+    total=False,
+)
+
 RequireCheckInTypeDef = TypedDict(
     "RequireCheckInTypeDef",
     {
         "ReleaseAfterMinutes": int,
         "Enabled": bool,
     },
     total=False,
@@ -1407,14 +1425,21 @@
     {
         "DurationInMinutes": int,
         "Enabled": bool,
     },
     total=False,
 )
 
+UpdateProactiveJoinTypeDef = TypedDict(
+    "UpdateProactiveJoinTypeDef",
+    {
+        "EnabledByMotion": bool,
+    },
+)
+
 UpdateRequireCheckInTypeDef = TypedDict(
     "UpdateRequireCheckInTypeDef",
     {
         "ReleaseAfterMinutes": int,
         "Enabled": bool,
     },
     total=False,
@@ -2008,14 +2033,15 @@
 CreateMeetingRoomConfigurationTypeDef = TypedDict(
     "CreateMeetingRoomConfigurationTypeDef",
     {
         "RoomUtilizationMetricsEnabled": bool,
         "EndOfMeetingReminder": CreateEndOfMeetingReminderTypeDef,
         "InstantBooking": CreateInstantBookingTypeDef,
         "RequireCheckIn": CreateRequireCheckInTypeDef,
+        "ProactiveJoin": CreateProactiveJoinTypeDef,
     },
     total=False,
 )
 
 SkillDetailsTypeDef = TypedDict(
     "SkillDetailsTypeDef",
     {
@@ -2285,14 +2311,15 @@
 MeetingRoomConfigurationTypeDef = TypedDict(
     "MeetingRoomConfigurationTypeDef",
     {
         "RoomUtilizationMetricsEnabled": bool,
         "EndOfMeetingReminder": EndOfMeetingReminderTypeDef,
         "InstantBooking": InstantBookingTypeDef,
         "RequireCheckIn": RequireCheckInTypeDef,
+        "ProactiveJoin": ProactiveJoinTypeDef,
     },
     total=False,
 )
 
 SearchNetworkProfilesResponseTypeDef = TypedDict(
     "SearchNetworkProfilesResponseTypeDef",
     {
@@ -2484,14 +2511,15 @@
 UpdateMeetingRoomConfigurationTypeDef = TypedDict(
     "UpdateMeetingRoomConfigurationTypeDef",
     {
         "RoomUtilizationMetricsEnabled": bool,
         "EndOfMeetingReminder": UpdateEndOfMeetingReminderTypeDef,
         "InstantBooking": UpdateInstantBookingTypeDef,
         "RequireCheckIn": UpdateRequireCheckInTypeDef,
+        "ProactiveJoin": UpdateProactiveJoinTypeDef,
     },
     total=False,
 )
 
 BusinessReportScheduleTypeDef = TypedDict(
     "BusinessReportScheduleTypeDef",
     {
```

### Comparing `mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness.egg-info/PKG-INFO` & `mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-alexaforbusiness
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.AlexaForBusiness 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.145
+Summary: Type annotations for boto3.AlexaForBusiness 1.26.145 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_alexaforbusiness/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,43 +18,44 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-alexaforbusiness"></a>
 
 # mypy-boto3-alexaforbusiness
 
 [![PyPI - mypy-boto3-alexaforbusiness](https://img.shields.io/pypi/v/mypy-boto3-alexaforbusiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-alexaforbusiness)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-alexaforbusiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-alexaforbusiness)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_alexaforbusiness/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-alexaforbusiness?color=blue)](https://pypistats.org/packages/mypy-boto3-alexaforbusiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AlexaForBusiness 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
+[boto3.AlexaForBusiness 1.26.145](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-alexaforbusiness docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_alexaforbusiness/).
 
 See how it helps to find and fix potential bugs:
 
@@ -423,14 +424,15 @@
     SipAddressTypeDef,
     SsmlTypeDef,
     TextTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     CreateEndOfMeetingReminderTypeDef,
     CreateInstantBookingTypeDef,
+    CreateProactiveJoinTypeDef,
     CreateRequireCheckInTypeDef,
     DeleteAddressBookRequestRequestTypeDef,
     DeleteBusinessReportScheduleRequestRequestTypeDef,
     DeleteConferenceProviderRequestRequestTypeDef,
     DeleteContactRequestRequestTypeDef,
     DeleteDeviceRequestRequestTypeDef,
     DeleteDeviceUsageDataRequestRequestTypeDef,
@@ -483,14 +485,15 @@
     ListSkillsRequestRequestTypeDef,
     SkillSummaryTypeDef,
     ListSkillsStoreCategoriesRequestRequestTypeDef,
     ListSkillsStoreSkillsByCategoryRequestRequestTypeDef,
     ListSmartHomeAppliancesRequestRequestTypeDef,
     SmartHomeApplianceTypeDef,
     ListTagsRequestRequestTypeDef,
+    ProactiveJoinTypeDef,
     RequireCheckInTypeDef,
     NetworkProfileDataTypeDef,
     ProfileDataTypeDef,
     PutInvitationConfigurationRequestRequestTypeDef,
     PutSkillAuthorizationRequestRequestTypeDef,
     RejectSkillRequestRequestTypeDef,
     ResolveRoomRequestRequestTypeDef,
@@ -505,14 +508,15 @@
     UntagResourceRequestRequestTypeDef,
     UpdateAddressBookRequestRequestTypeDef,
     UpdateDeviceRequestRequestTypeDef,
     UpdateEndOfMeetingReminderTypeDef,
     UpdateGatewayGroupRequestRequestTypeDef,
     UpdateGatewayRequestRequestTypeDef,
     UpdateInstantBookingTypeDef,
+    UpdateProactiveJoinTypeDef,
     UpdateRequireCheckInTypeDef,
     UpdateNetworkProfileRequestRequestTypeDef,
     UpdateRoomRequestRequestTypeDef,
     UpdateSkillGroupRequestRequestTypeDef,
     UpdateBusinessReportScheduleRequestRequestTypeDef,
     BusinessReportTypeDef,
     PutConferencePreferenceRequestRequestTypeDef,
@@ -622,42 +626,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-alexaforbusiness-1.26.0.post1/mypy_boto3_alexaforbusiness.egg-info/SOURCES.txt` & `mypy-boto3-alexaforbusiness-1.26.145/mypy_boto3_alexaforbusiness.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-alexaforbusiness-1.26.0.post1/setup.py` & `mypy-boto3-alexaforbusiness-1.26.145/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-alexaforbusiness.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-alexaforbusiness",
-    version="1.26.0.post1",
+    version="1.26.145",
     packages=["mypy_boto3_alexaforbusiness"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AlexaForBusiness 1.26.0 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.AlexaForBusiness 1.26.145 service generated with"
+        " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 alexaforbusiness type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_alexaforbusiness": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_alexaforbusiness": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_alexaforbusiness/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        "typing-extensions>=4.1.0",
+        'typing-extensions>=4.1.0; python_version<"3.9"',
     ],
     zip_safe=False,
 )
```

