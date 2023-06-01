# Comparing `tmp/iam_actions-1.2.20230531.tar.gz` & `tmp/iam_actions-1.2.20230601.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230531.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230601.tar", max compression
```

## Comparing `iam_actions-1.2.20230531.tar` & `iam_actions-1.2.20230601.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-05-31 02:48:07.461038 iam_actions-1.2.20230531/LICENSE
--rw-r--r--   0        0        0     2302 2023-05-31 02:48:07.461038 iam_actions-1.2.20230531/README.md
--rw-r--r--   0        0        0      228 2023-05-31 02:48:07.461038 iam_actions-1.2.20230531/iam_actions/__init__.py
--rw-r--r--   0        0        0  4280299 2023-05-31 02:49:49.509393 iam_actions-1.2.20230531/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-05-31 02:48:07.461038 iam_actions-1.2.20230531/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-05-31 02:48:07.461038 iam_actions-1.2.20230531/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-05-31 02:48:07.461038 iam_actions-1.2.20230531/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-05-31 02:48:07.461038 iam_actions-1.2.20230531/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-05-31 02:48:07.461038 iam_actions-1.2.20230531/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-05-31 02:48:07.461038 iam_actions-1.2.20230531/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-05-31 02:48:07.461038 iam_actions-1.2.20230531/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-05-31 02:48:07.461038 iam_actions-1.2.20230531/iam_actions/generate/services.py
--rw-r--r--   0        0        0   549782 2023-05-31 02:49:49.513393 iam_actions-1.2.20230531/iam_actions/policies.json
--rw-r--r--   0        0        0   195033 2023-05-31 02:49:49.509393 iam_actions-1.2.20230531/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   533302 2023-05-31 02:49:49.509393 iam_actions-1.2.20230531/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-05-31 02:49:50.577393 iam_actions-1.2.20230531/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230531/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230531/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-01 03:05:45.952042 iam_actions-1.2.20230601/LICENSE
+-rw-r--r--   0        0        0     2302 2023-06-01 03:05:45.952042 iam_actions-1.2.20230601/README.md
+-rw-r--r--   0        0        0      228 2023-06-01 03:05:45.952042 iam_actions-1.2.20230601/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4277029 2023-06-01 03:07:23.245078 iam_actions-1.2.20230601/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-06-01 03:05:45.952042 iam_actions-1.2.20230601/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-06-01 03:05:45.952042 iam_actions-1.2.20230601/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-06-01 03:05:45.952042 iam_actions-1.2.20230601/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-06-01 03:05:45.952042 iam_actions-1.2.20230601/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-06-01 03:05:45.952042 iam_actions-1.2.20230601/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-06-01 03:05:45.952042 iam_actions-1.2.20230601/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-06-01 03:05:45.952042 iam_actions-1.2.20230601/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-06-01 03:05:45.952042 iam_actions-1.2.20230601/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   550024 2023-06-01 03:07:23.245078 iam_actions-1.2.20230601/iam_actions/policies.json
+-rw-r--r--   0        0        0   195249 2023-06-01 03:07:23.245078 iam_actions-1.2.20230601/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   533536 2023-06-01 03:07:23.245078 iam_actions-1.2.20230601/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-06-01 03:07:24.029086 iam_actions-1.2.20230601/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230601/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230601/PKG-INFO
```

### Comparing `iam_actions-1.2.20230531/LICENSE` & `iam_actions-1.2.20230601/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230531/README.md` & `iam_actions-1.2.20230601/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230531/iam_actions/actions.json` & `iam_actions-1.2.20230601/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991141837368779%*

 * *Differences: {"'appflow'": "{'CancelFlowExecutions': OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *              "'CancelFlowExecutions'), ('condition_keys', []), ('description', 'Not Documented by "*

 * *              "AWS'), ('orphan', False), ('resources', [])])}",*

 * * "'iotfleetwise'": "{'CreateCampaign': {'condition_keys': {insert: [(2, "*

 * *                   "'iotfleetwise:DestinationArn')]}}}",*

 * * "'schemas'": "{'CreateDiscoverer': {'resources': []}}",*

 * * "'securitylake'": "{'CreateAwsLogSource': {'description':  […]*

```diff
@@ -4133,14 +4133,22 @@
             "resources": [
                 "application",
                 "configurationprofile"
             ]
         }
     },
     "appflow": {
+        "CancelFlowExecutions": {
+            "access_level": "Undocumented",
+            "action": "CancelFlowExecutions",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateConnectorProfile": {
             "access_level": "Write",
             "action": "CreateConnectorProfile",
             "condition_keys": [],
             "description": "Grants permission to create a login profile to be used with Amazon AppFlow flows",
             "orphan": false,
             "resources": []
@@ -78125,15 +78133,16 @@
             ]
         },
         "CreateCampaign": {
             "access_level": "Write",
             "action": "CreateCampaign",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
+                "aws:TagKeys",
+                "iotfleetwise:DestinationArn"
             ],
             "description": "Grants permission to create a campaign",
             "orphan": false,
             "resources": [
                 "fleet",
                 "signalcatalog",
                 "vehicle"
@@ -128314,17 +128323,15 @@
             "action": "CreateDiscoverer",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to create an event schema discoverer. Once created, your events will be automatically map into corresponding schema documents",
             "orphan": false,
-            "resources": [
-                "discoverer"
-            ]
+            "resources": []
         },
         "CreateRegistry": {
             "access_level": "Write",
             "action": "CreateRegistry",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
@@ -129919,401 +129926,267 @@
         }
     },
     "securitylake": {
         "CreateAwsLogSource": {
             "access_level": "Write",
             "action": "CreateAwsLogSource",
             "condition_keys": [],
-            "description": "Grants permission to enable any source type in any region for accounts that are either part of a trusted organization or standalone accounts",
+            "description": "Grants permission to enable any source type in any region for accounts that are either part of a trusted organization or standalone account",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "data-lake"
+            ]
         },
         "CreateCustomLogSource": {
             "access_level": "Write",
             "action": "CreateCustomLogSource",
             "condition_keys": [],
-            "description": "Grants permission to add a custom source name",
+            "description": "Grants permission to add a custom source",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "data-lake"
+            ]
         },
         "CreateDataLake": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateDataLake",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to create a new security data lake",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "data-lake"
+            ]
         },
         "CreateDataLakeExceptionSubscription": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateDataLakeExceptionSubscription",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to get instant notifications about exceptions. Subscribes to the SNS topics for exception notifications",
             "orphan": false,
             "resources": []
         },
         "CreateDataLakeOrganizationConfiguration": {
-            "access_level": "Undocumented",
-            "action": "CreateDataLakeOrganizationConfiguration",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
-        },
-        "CreateDatalake": {
             "access_level": "Write",
-            "action": "CreateDatalake",
-            "condition_keys": [],
-            "description": "Grants permission to create a new Security Data Lake",
-            "orphan": false,
-            "resources": []
-        },
-        "CreateDatalakeAutoEnable": {
-            "access_level": "Write",
-            "action": "CreateDatalakeAutoEnable",
-            "condition_keys": [],
-            "description": "Grants permission to add to the configuration for automatically enabling Amazon Security Lake access for new organization accounts",
-            "orphan": false,
-            "resources": []
-        },
-        "CreateDatalakeDelegatedAdmin": {
-            "access_level": "Write",
-            "action": "CreateDatalakeDelegatedAdmin",
-            "condition_keys": [],
-            "description": "Grants permission to designate the Amazon Security Lake administrator account for the organization",
-            "orphan": false,
-            "resources": []
-        },
-        "CreateDatalakeExceptionsSubscription": {
-            "access_level": "Write",
-            "action": "CreateDatalakeExceptionsSubscription",
+            "action": "CreateDataLakeOrganizationConfiguration",
             "condition_keys": [],
-            "description": "Grants permission to get instant notifications about exceptions by subscribing to the SNS topics for exception notifications",
+            "description": "Grants permission to automatically enable Amazon Security Lake for new member accounts in your organization",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "data-lake"
+            ]
         },
         "CreateSubscriber": {
             "access_level": "Write",
             "action": "CreateSubscriber",
             "condition_keys": [],
-            "description": "Grants permission to create a subscription permission for accounts that are already enabled",
+            "description": "Grants permission to create a subscriber",
             "orphan": false,
             "resources": []
         },
         "CreateSubscriberNotification": {
-            "access_level": "Undocumented",
-            "action": "CreateSubscriberNotification",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
-        },
-        "CreateSubscriptionNotificationConfiguration": {
             "access_level": "Write",
-            "action": "CreateSubscriptionNotificationConfiguration",
+            "action": "CreateSubscriberNotification",
             "condition_keys": [],
-            "description": "Grants permission to create a webhook invocation to notify a client when there is new data in the Data Lake",
+            "description": "Grants permission to create a webhook invocation to notify a client when there is new data in the data lake",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "subscriber"
+            ]
         },
         "DeleteAwsLogSource": {
             "access_level": "Write",
             "action": "DeleteAwsLogSource",
             "condition_keys": [],
-            "description": "Grants permission to disable any source type in any region for accounts that are either part of a trusted organization or standalone accounts",
+            "description": "Grants permission to disable any source type in any region for accounts that are part of a trusted organization or standalone accounts",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "data-lake"
+            ]
         },
         "DeleteCustomLogSource": {
             "access_level": "Write",
             "action": "DeleteCustomLogSource",
             "condition_keys": [],
-            "description": "Grants permission to remove a custom source name",
+            "description": "Grants permission to remove a custom source",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "data-lake"
+            ]
         },
         "DeleteDataLake": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteDataLake",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete security data lake",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "data-lake"
+            ]
         },
         "DeleteDataLakeExceptionSubscription": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteDataLakeExceptionSubscription",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to unsubscribe from SNS topics for exception notifications. Removes exception notifications for the SNS topic",
             "orphan": false,
             "resources": []
         },
         "DeleteDataLakeOrganizationConfiguration": {
-            "access_level": "Undocumented",
-            "action": "DeleteDataLakeOrganizationConfiguration",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
-        },
-        "DeleteDatalake": {
-            "access_level": "Write",
-            "action": "DeleteDatalake",
-            "condition_keys": [],
-            "description": "Grants permission to delete all Security Data Lakes",
-            "orphan": false,
-            "resources": []
-        },
-        "DeleteDatalakeAutoEnable": {
-            "access_level": "Write",
-            "action": "DeleteDatalakeAutoEnable",
-            "condition_keys": [],
-            "description": "Grants permission to remove from the existing configuration the automatic enabling of Amazon Security Lake access for new organization accounts",
-            "orphan": false,
-            "resources": []
-        },
-        "DeleteDatalakeDelegatedAdmin": {
-            "access_level": "Write",
-            "action": "DeleteDatalakeDelegatedAdmin",
-            "condition_keys": [],
-            "description": "Grants permission to remove the Delegated Administrator account and disable Amazon Security Lake as a service for this organization",
-            "orphan": false,
-            "resources": []
-        },
-        "DeleteDatalakeExceptionsSubscription": {
             "access_level": "Write",
-            "action": "DeleteDatalakeExceptionsSubscription",
+            "action": "DeleteDataLakeOrganizationConfiguration",
             "condition_keys": [],
-            "description": "Grants permission to unsubscribe from SNS topics for exception notifications. Also, removes the SNS exception notifications topic",
+            "description": "Grants permission to remove the automatic enablement of Amazon Security Lake access for new organization accounts",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "data-lake"
+            ]
         },
         "DeleteSubscriber": {
             "access_level": "Write",
             "action": "DeleteSubscriber",
             "condition_keys": [],
-            "description": "Grants permission to delete the specified subscription permissions for accounts that are already enabled",
+            "description": "Grants permission to delete the specified subscriber",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "subscriber"
+            ]
         },
         "DeleteSubscriberNotification": {
-            "access_level": "Undocumented",
-            "action": "DeleteSubscriberNotification",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
-        },
-        "DeleteSubscriptionNotificationConfiguration": {
             "access_level": "Write",
-            "action": "DeleteSubscriptionNotificationConfiguration",
+            "action": "DeleteSubscriberNotification",
             "condition_keys": [],
-            "description": "Grants permission to remove a webhook invocation to notify a client when there is new data in the Data Lake",
+            "description": "Grants permission to remove a webhook invocation to notify a client when there is new data in the data lake",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "subscriber"
+            ]
         },
         "DeregisterDataLakeDelegatedAdministrator": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeregisterDataLakeDelegatedAdministrator",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to remove the Delegated Administrator account and disable Amazon Security Lake as a service for this organization",
             "orphan": false,
             "resources": []
         },
         "GetDataLakeExceptionSubscription": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetDataLakeExceptionSubscription",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to query the protocol and endpoint that were provided when subscribing to SNS topics for exception notifications",
             "orphan": false,
             "resources": []
         },
         "GetDataLakeOrganizationConfiguration": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetDataLakeOrganizationConfiguration",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to get an organization\u2019s configuration setting for automatically enabling Amazon Security Lake access for new organization accounts",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "data-lake"
+            ]
         },
         "GetDataLakeSources": {
-            "access_level": "Undocumented",
-            "action": "GetDataLakeSources",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
-        },
-        "GetDatalake": {
-            "access_level": "Read",
-            "action": "GetDatalake",
-            "condition_keys": [],
-            "description": "Grants permission to get information on the Security Data Lake",
-            "orphan": false,
-            "resources": []
-        },
-        "GetDatalakeAutoEnable": {
-            "access_level": "Read",
-            "action": "GetDatalakeAutoEnable",
-            "condition_keys": [],
-            "description": "Grants permission to get an organization\u2019s configuration setting for the automatic enabling of Amazon Security Lake access for new organization accounts",
-            "orphan": false,
-            "resources": []
-        },
-        "GetDatalakeExceptionsExpiry": {
             "access_level": "Read",
-            "action": "GetDatalakeExceptionsExpiry",
-            "condition_keys": [],
-            "description": "Grants permission to allow user to query what was set as the expiration period for the exception message",
-            "orphan": false,
-            "resources": []
-        },
-        "GetDatalakeExceptionsSubscription": {
-            "access_level": "Read",
-            "action": "GetDatalakeExceptionsSubscription",
-            "condition_keys": [],
-            "description": "Grants permission to query the protocol and endpoint that were supplied when subscribing to the SNS topics for exception notifications",
-            "orphan": false,
-            "resources": []
-        },
-        "GetDatalakeStatus": {
-            "access_level": "Read",
-            "action": "GetDatalakeStatus",
+            "action": "GetDataLakeSources",
             "condition_keys": [],
-            "description": "Grants permission to get a static snapshot of the Security Data Lake in the current region, including enabled accounts and log sources",
+            "description": "Grants permission to get a static snapshot of the security data lake in the current region. The snapshot includes enabled accounts and log sources",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "data-lake"
+            ]
         },
         "GetSubscriber": {
             "access_level": "Read",
             "action": "GetSubscriber",
             "condition_keys": [],
-            "description": "Grants permission to get subscription information for a subscription permission for accounts that are already enabled",
+            "description": "Grants permission to get information about subscriber that is already created",
             "orphan": false,
-            "resources": []
-        },
-        "GetSubscriptionNotificationConfiguration": {
-            "access_level": "Read",
-            "action": "GetSubscriptionNotificationConfiguration",
-            "condition_keys": [],
-            "description": "Grants permission to get information for a webhook invocation to notify a client when there is new data in the Data Lake",
-            "orphan": false,
-            "resources": []
+            "resources": [
+                "subscriber"
+            ]
         },
         "ListDataLakeExceptions": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListDataLakeExceptions",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to get the list of all non-retryable failures",
             "orphan": false,
             "resources": []
         },
         "ListDataLakes": {
-            "access_level": "Undocumented",
-            "action": "ListDataLakes",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
-        },
-        "ListDatalakeExceptions": {
             "access_level": "List",
-            "action": "ListDatalakeExceptions",
+            "action": "ListDataLakes",
             "condition_keys": [],
-            "description": "Grants permission to get the list of all non-retry-able failures",
+            "description": "Grants permission to list information about the security data lakes",
             "orphan": false,
             "resources": []
         },
         "ListLogSources": {
             "access_level": "List",
             "action": "ListLogSources",
             "condition_keys": [],
-            "description": "Grants permission to show the estate view of enabled accounts with the enabled sources in the enabled regions",
+            "description": "Grants permission to view the enabled accounts. You can view the enabled sources in the enabled regions",
             "orphan": false,
             "resources": []
         },
         "ListSubscribers": {
             "access_level": "List",
             "action": "ListSubscribers",
             "condition_keys": [],
-            "description": "Grants permission to list all subscription permissions for accounts that are already enabled",
+            "description": "Grants permission to list all subscribers",
             "orphan": false,
             "resources": []
         },
         "RegisterDataLakeDelegatedAdministrator": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "RegisterDataLakeDelegatedAdministrator",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to designate an account as the Amazon Security Lake administrator account for the organization",
             "orphan": false,
             "resources": []
         },
         "UpdateDataLake": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateDataLake",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update a security data lake",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "data-lake"
+            ]
         },
         "UpdateDataLakeExceptionSubscription": {
-            "access_level": "Undocumented",
-            "action": "UpdateDataLakeExceptionSubscription",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
-        },
-        "UpdateDatalake": {
             "access_level": "Write",
-            "action": "UpdateDatalake",
-            "condition_keys": [],
-            "description": "Grants permission to update a Security Data Lake",
-            "orphan": false,
-            "resources": []
-        },
-        "UpdateDatalakeExceptionsExpiry": {
-            "access_level": "Write",
-            "action": "UpdateDatalakeExceptionsExpiry",
-            "condition_keys": [],
-            "description": "Grants permission to control the time-to-live (TTL) for the exception message to remain in service cache",
-            "orphan": false,
-            "resources": []
-        },
-        "UpdateDatalakeExceptionsSubscription": {
-            "access_level": "Write",
-            "action": "UpdateDatalakeExceptionsSubscription",
+            "action": "UpdateDataLakeExceptionSubscription",
             "condition_keys": [],
             "description": "Grants permission to update subscriptions to the SNS topics for exception notifications",
             "orphan": false,
             "resources": []
         },
         "UpdateSubscriber": {
             "access_level": "Write",
             "action": "UpdateSubscriber",
             "condition_keys": [],
-            "description": "Grants permission to update subscription information for a subscription permission for accounts that are already enabled",
+            "description": "Grants permission to update subscriber",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "subscriber"
+            ]
         },
         "UpdateSubscriberNotification": {
-            "access_level": "Undocumented",
-            "action": "UpdateSubscriberNotification",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
-        },
-        "UpdateSubscriptionNotificationConfiguration": {
             "access_level": "Write",
-            "action": "UpdateSubscriptionNotificationConfiguration",
+            "action": "UpdateSubscriberNotification",
             "condition_keys": [],
-            "description": "Grants permission to update a webhook invocation to notify a client when there is new data in the Data Lake",
+            "description": "Grants permission to update a webhook invocation to notify a client when there is new data in the data lake",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "subscriber"
+            ]
         }
     },
     "serverlessrepo": {
         "CreateApplication": {
             "access_level": "Write",
             "action": "CreateApplication",
             "condition_keys": [],
@@ -152549,14 +152422,22 @@
             "description": "Grants permission to associate browser settings to web portals",
             "orphan": false,
             "resources": [
                 "browserSettings",
                 "portal"
             ]
         },
+        "AssociateIpAccessSettings": {
+            "access_level": "Undocumented",
+            "action": "AssociateIpAccessSettings",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "AssociateNetworkSettings": {
             "access_level": "Write",
             "action": "AssociateNetworkSettings",
             "condition_keys": [],
             "description": "Grants permission to associate network settings to web portals",
             "orphan": false,
             "resources": [
@@ -152614,14 +152495,22 @@
             "condition_keys": [],
             "description": "Grants permission to create identity providers",
             "orphan": false,
             "resources": [
                 "portal"
             ]
         },
+        "CreateIpAccessSettings": {
+            "access_level": "Undocumented",
+            "action": "CreateIpAccessSettings",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateNetworkSettings": {
             "access_level": "Write",
             "action": "CreateNetworkSettings",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
@@ -152687,14 +152576,22 @@
             "access_level": "Write",
             "action": "DeleteIdentityProvider",
             "condition_keys": [],
             "description": "Grants permission to delete identity providers",
             "orphan": false,
             "resources": []
         },
+        "DeleteIpAccessSettings": {
+            "access_level": "Undocumented",
+            "action": "DeleteIpAccessSettings",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteNetworkSettings": {
             "access_level": "Write",
             "action": "DeleteNetworkSettings",
             "condition_keys": [],
             "description": "Grants permission to delete network settings",
             "orphan": false,
             "resources": [
@@ -152747,14 +152644,22 @@
             "condition_keys": [],
             "description": "Grants permission to disassociate browser settings from web portals",
             "orphan": false,
             "resources": [
                 "portal"
             ]
         },
+        "DisassociateIpAccessSettings": {
+            "access_level": "Undocumented",
+            "action": "DisassociateIpAccessSettings",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DisassociateNetworkSettings": {
             "access_level": "Write",
             "action": "DisassociateNetworkSettings",
             "condition_keys": [],
             "description": "Grants permission to disassociate network settings from web portals",
             "orphan": false,
             "resources": [
@@ -152805,14 +152710,22 @@
             "access_level": "Read",
             "action": "GetIdentityProvider",
             "condition_keys": [],
             "description": "Grants permission to get details on identity providers",
             "orphan": false,
             "resources": []
         },
+        "GetIpAccessSettings": {
+            "access_level": "Undocumented",
+            "action": "GetIpAccessSettings",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetNetworkSettings": {
             "access_level": "Read",
             "action": "GetNetworkSettings",
             "condition_keys": [],
             "description": "Grants permission to get details on network settings",
             "orphan": false,
             "resources": [
@@ -152891,14 +152804,22 @@
             "access_level": "Read",
             "action": "ListIdentityProviders",
             "condition_keys": [],
             "description": "Grants permission to list identity providers",
             "orphan": false,
             "resources": []
         },
+        "ListIpAccessSettings": {
+            "access_level": "Undocumented",
+            "action": "ListIpAccessSettings",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListNetworkSettings": {
             "access_level": "Read",
             "action": "ListNetworkSettings",
             "condition_keys": [],
             "description": "Grants permission to list network settings",
             "orphan": false,
             "resources": []
@@ -153001,14 +152922,22 @@
             "access_level": "Write",
             "action": "UpdateIdentityProvider",
             "condition_keys": [],
             "description": "Grants permission to update identity provider",
             "orphan": false,
             "resources": []
         },
+        "UpdateIpAccessSettings": {
+            "access_level": "Undocumented",
+            "action": "UpdateIpAccessSettings",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateNetworkSettings": {
             "access_level": "Write",
             "action": "UpdateNetworkSettings",
             "condition_keys": [],
             "description": "Grants permission to update network settings",
             "orphan": false,
             "resources": [
```

### Comparing `iam_actions-1.2.20230531/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230601/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230531/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230601/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230531/iam_actions/generate/generate.py` & `iam_actions-1.2.20230601/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230531/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230601/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230531/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230601/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230531/iam_actions/generate/services.py` & `iam_actions-1.2.20230601/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230531/iam_actions/policies.json` & `iam_actions-1.2.20230601/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999982977123286%*

 * *Differences: {"'serviceMap'": "{'Amazon AppFlow': {'Actions': {insert: [(0, 'CancelFlowExecutions')]}}, 'Amazon "*

 * *                 "WorkSpaces Web': {'Actions': {insert: [(1, 'AssociateIpAccessSettings'), (8, "*

 * *                 "'CreateIpAccessSettings'), (16, 'DeleteIpAccessSettings'), (23, "*

 * *                 "'DisassociateIpAccessSettings'), (30, 'GetIpAccessSettings'), (40, "*

 * *                 "'ListIpAccessSettings'), (52, 'UpdateIpAccessSettings')]}}}"}*

```diff
@@ -9725,14 +9725,15 @@
                 "aws:TagKeys"
             ]
         },
         "Amazon AppFlow": {
             "ARNFormat": "arn:aws:appflow:${Region}:${Account}:${ResourceType}/${ResourceName}",
             "ARNRegex": "^arn:aws:appflow:.+:.+:.+",
             "Actions": [
+                "CancelFlowExecutions",
                 "CreateConnectorProfile",
                 "CreateFlow",
                 "DeleteConnectorProfile",
                 "DeleteFlow",
                 "DescribeConnector",
                 "DescribeConnectorEntity",
                 "DescribeConnectorFields",
@@ -19540,59 +19541,66 @@
             "StringPrefix": "wam"
         },
         "Amazon WorkSpaces Web": {
             "ARNFormat": "arn:aws:workspaces-web:${Region}:${Account}:${ResourceType}/${ResourceIdentifier}",
             "ARNRegex": "^arn:aws:workspaces-web:.+",
             "Actions": [
                 "AssociateBrowserSettings",
+                "AssociateIpAccessSettings",
                 "AssociateNetworkSettings",
                 "AssociateTrustStore",
                 "AssociateUserAccessLoggingSettings",
                 "AssociateUserSettings",
                 "CreateBrowserSettings",
                 "CreateIdentityProvider",
+                "CreateIpAccessSettings",
                 "CreateNetworkSettings",
                 "CreatePortal",
                 "CreateTrustStore",
                 "CreateUserAccessLoggingSettings",
                 "CreateUserSettings",
                 "DeleteBrowserSettings",
                 "DeleteIdentityProvider",
+                "DeleteIpAccessSettings",
                 "DeleteNetworkSettings",
                 "DeletePortal",
                 "DeleteTrustStore",
                 "DeleteUserAccessLoggingSettings",
                 "DeleteUserSettings",
                 "DisassociateBrowserSettings",
+                "DisassociateIpAccessSettings",
                 "DisassociateNetworkSettings",
                 "DisassociateTrustStore",
                 "DisassociateUserAccessLoggingSettings",
                 "DisassociateUserSettings",
                 "GetBrowserSettings",
                 "GetIdentityProvider",
+                "GetIpAccessSettings",
                 "GetNetworkSettings",
                 "GetPortal",
                 "GetPortalServiceProviderMetadata",
                 "GetTrustStore",
                 "GetTrustStoreCertificate",
                 "GetUserAccessLoggingSettings",
                 "GetUserSettings",
                 "ListBrowserSettings",
                 "ListIdentityProviders",
+                "ListIpAccessSettings",
                 "ListNetworkSettings",
                 "ListPortals",
                 "ListTagsForResource",
                 "ListTrustStoreCertificates",
                 "ListTrustStores",
                 "ListUserAccessLoggingSettings",
                 "ListUserSettings",
                 "TagResource",
                 "UntagResource",
                 "UpdateBrowserSettings",
                 "UpdateIdentityProvider",
+                "UpdateIpAccessSettings",
                 "UpdateNetworkSettings",
                 "UpdatePortal",
                 "UpdateTrustStore",
                 "UpdateUserAccessLoggingSettings",
                 "UpdateUserSettings"
             ],
             "HasResource": true,
```

### Comparing `iam_actions-1.2.20230531/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230601/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985863095238096%*

 * *Differences: {"'deepracer'": "{'evaluation_job': {'arn_pattern': 'arn:*:deepracer:*:*:evaluation_job/*'}}",*

 * * "'securitylake'": "{replace: OrderedDict([('data-lake', OrderedDict([('arn_pattern', "*

 * *                   "'arn:*:securitylake:*:*:data-lake/default'), ('condition_keys', None)])), "*

 * *                   "('subscriber', OrderedDict([('arn_pattern', "*

 * *                   "'arn:*:securitylake:*:*:subscriber/*'), ('condition_keys', None)]))])}"}*

```diff
@@ -1632,15 +1632,15 @@
     },
     "deepracer": {
         "car": {
             "arn_pattern": "arn:*:deepracer:*:*:car/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "evaluation_job": {
-            "arn_pattern": "arn:*:deepracer:*:*: evaluation_job/*",
+            "arn_pattern": "arn:*:deepracer:*:*:evaluation_job/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "leaderboard": {
             "arn_pattern": "arn:*:deepracer:*::leaderboard/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "leaderboard_evaluation_job": {
@@ -5798,15 +5798,24 @@
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "product": {
             "arn_pattern": "arn:*:securityhub:*:*:product/*/*",
             "condition_keys": null
         }
     },
-    "securitylake": {},
+    "securitylake": {
+        "data-lake": {
+            "arn_pattern": "arn:*:securitylake:*:*:data-lake/default",
+            "condition_keys": null
+        },
+        "subscriber": {
+            "arn_pattern": "arn:*:securitylake:*:*:subscriber/*",
+            "condition_keys": null
+        }
+    },
     "serverlessrepo": {
         "applications": {
             "arn_pattern": "arn:*:serverlessrepo:*:*:applications/*",
             "condition_keys": null
         }
     },
     "servicecatalog": {
```

### Comparing `iam_actions-1.2.20230531/iam_actions/services.json` & `iam_actions-1.2.20230601/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999821732652192%*

 * *Differences: {"'appflow'": "{'Actions': {insert: [(0, 'CancelFlowExecutions')]}}",*

 * * "'workspaces-web'": "{'Actions': {insert: [(1, 'AssociateIpAccessSettings'), (8, "*

 * *                     "'CreateIpAccessSettings'), (16, 'DeleteIpAccessSettings'), (23, "*

 * *                     "'DisassociateIpAccessSettings'), (30, 'GetIpAccessSettings'), (40, "*

 * *                     "'ListIpAccessSettings'), (52, 'UpdateIpAccessSettings')]}}"}*

```diff
@@ -707,14 +707,15 @@
         "ARNFormats": [
             "arn:aws:appflow:${Region}:${Account}:${ResourceType}/${ResourceName}"
         ],
         "ARNRegexes": [
             "^arn:aws:appflow:.+:.+:.+"
         ],
         "Actions": [
+            "CancelFlowExecutions",
             "CreateConnectorProfile",
             "CreateFlow",
             "DeleteConnectorProfile",
             "DeleteFlow",
             "DescribeConnector",
             "DescribeConnectorEntity",
             "DescribeConnectorFields",
@@ -21430,59 +21431,66 @@
             "arn:aws:workspaces-web:${Region}:${Account}:${ResourceType}/${ResourceIdentifier}"
         ],
         "ARNRegexes": [
             "^arn:aws:workspaces-web:.+"
         ],
         "Actions": [
             "AssociateBrowserSettings",
+            "AssociateIpAccessSettings",
             "AssociateNetworkSettings",
             "AssociateTrustStore",
             "AssociateUserAccessLoggingSettings",
             "AssociateUserSettings",
             "CreateBrowserSettings",
             "CreateIdentityProvider",
+            "CreateIpAccessSettings",
             "CreateNetworkSettings",
             "CreatePortal",
             "CreateTrustStore",
             "CreateUserAccessLoggingSettings",
             "CreateUserSettings",
             "DeleteBrowserSettings",
             "DeleteIdentityProvider",
+            "DeleteIpAccessSettings",
             "DeleteNetworkSettings",
             "DeletePortal",
             "DeleteTrustStore",
             "DeleteUserAccessLoggingSettings",
             "DeleteUserSettings",
             "DisassociateBrowserSettings",
+            "DisassociateIpAccessSettings",
             "DisassociateNetworkSettings",
             "DisassociateTrustStore",
             "DisassociateUserAccessLoggingSettings",
             "DisassociateUserSettings",
             "GetBrowserSettings",
             "GetIdentityProvider",
+            "GetIpAccessSettings",
             "GetNetworkSettings",
             "GetPortal",
             "GetPortalServiceProviderMetadata",
             "GetTrustStore",
             "GetTrustStoreCertificate",
             "GetUserAccessLoggingSettings",
             "GetUserSettings",
             "ListBrowserSettings",
             "ListIdentityProviders",
+            "ListIpAccessSettings",
             "ListNetworkSettings",
             "ListPortals",
             "ListTagsForResource",
             "ListTrustStoreCertificates",
             "ListTrustStores",
             "ListUserAccessLoggingSettings",
             "ListUserSettings",
             "TagResource",
             "UntagResource",
             "UpdateBrowserSettings",
             "UpdateIdentityProvider",
+            "UpdateIpAccessSettings",
             "UpdateNetworkSettings",
             "UpdatePortal",
             "UpdateTrustStore",
             "UpdateUserAccessLoggingSettings",
             "UpdateUserSettings"
         ],
         "ConditionKeys": [
```

### Comparing `iam_actions-1.2.20230531/pyproject.toml` & `iam_actions-1.2.20230601/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230531"
+version = "1.2.20230601"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230531/setup.py` & `iam_actions-1.2.20230601/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230531',
+    'version': '1.2.20230601',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230531/PKG-INFO` & `iam_actions-1.2.20230601/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230531
+Version: 1.2.20230601
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

