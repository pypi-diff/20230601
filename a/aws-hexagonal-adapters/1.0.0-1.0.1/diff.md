# Comparing `tmp/aws_hexagonal_adapters-1.0.0.tar.gz` & `tmp/aws_hexagonal_adapters-1.0.1.tar.gz`

## Comparing `aws_hexagonal_adapters-1.0.0.tar` & `aws_hexagonal_adapters-1.0.1.tar`

### file list

```diff
@@ -1,42 +1,46 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.DS_Store
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/ruff.toml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.pytest_cache/README.md
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.ruff_cache/content/168cc38b04774c1d
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.ruff_cache/content/618c6b6cc269398a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.ruff_cache/content/81d6bea09b3bfddc
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.ruff_cache/content/8f6d8158c77dd870
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.ruff_cache/content/a5ccc3b3108d4277
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.ruff_cache/content/c285b1f3993c3cc4
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.ruff_cache/content/c5082269dd966539
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.ruff_cache/content/c82b673ec67750f8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.ruff_cache/content/df318c36e6722395
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.ruff_cache/content/fc051c84047f8578
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.ruff_cache/content/fff176ebb881786c
--rw-r--r--   0        0        0     7021 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/aws_hexagonal_adapters/dynamo_db_service.py
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/aws_hexagonal_adapters/event_bridge_service.py
--rw-r--r--   0        0        0    10809 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/aws_hexagonal_adapters/s3_service.py
--rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/aws_hexagonal_adapters/ses_service.py
--rw-r--r--   0        0        0     8374 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/aws_hexagonal_adapters/sqs_service.py
--rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/aws_hexagonal_adapters/ssm_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/tests/nonexistent.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/tests/test.txt
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/tests/test_s3_service.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/LICENSE
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/README.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.DS_Store
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/ruff.toml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.pytest_cache/README.md
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/content/168cc38b04774c1d
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/content/618c6b6cc269398a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/content/75d3689fa3a76235
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/content/7c78c5206be80766
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/content/81d6bea09b3bfddc
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/content/8f6d8158c77dd870
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/content/a41f533a26961e6
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/content/a5ccc3b3108d4277
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/content/c285b1f3993c3cc4
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/content/c5082269dd966539
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/content/c521446dd63755a4
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/content/c82b673ec67750f8
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/content/df318c36e6722395
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/content/fc051c84047f8578
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/content/fff176ebb881786c
+-rw-r--r--   0        0        0     7021 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/aws_hexagonal_adapters/dynamo_db_service.py
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/aws_hexagonal_adapters/event_bridge_service.py
+-rw-r--r--   0        0        0    10809 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/aws_hexagonal_adapters/s3_service.py
+-rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/aws_hexagonal_adapters/ses_service.py
+-rw-r--r--   0        0        0     8233 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/aws_hexagonal_adapters/sqs_service.py
+-rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/aws_hexagonal_adapters/ssm_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/tests/nonexistent.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/tests/test.txt
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/tests/test_s3_service.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/README.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/PKG-INFO
```

### Comparing `aws_hexagonal_adapters-1.0.0/.DS_Store` & `aws_hexagonal_adapters-1.0.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `aws_hexagonal_adapters-1.0.0/.ruff_cache/content/618c6b6cc269398a` & `aws_hexagonal_adapters-1.0.1/.ruff_cache/content/618c6b6cc269398a`

 * *Files identical despite different names*

### Comparing `aws_hexagonal_adapters-1.0.0/aws_hexagonal_adapters/dynamo_db_service.py` & `aws_hexagonal_adapters-1.0.1/aws_hexagonal_adapters/dynamo_db_service.py`

 * *Files identical despite different names*

### Comparing `aws_hexagonal_adapters-1.0.0/aws_hexagonal_adapters/event_bridge_service.py` & `aws_hexagonal_adapters-1.0.1/aws_hexagonal_adapters/event_bridge_service.py`

 * *Files identical despite different names*

### Comparing `aws_hexagonal_adapters-1.0.0/aws_hexagonal_adapters/s3_service.py` & `aws_hexagonal_adapters-1.0.1/aws_hexagonal_adapters/s3_service.py`

 * *Files identical despite different names*

### Comparing `aws_hexagonal_adapters-1.0.0/aws_hexagonal_adapters/ses_service.py` & `aws_hexagonal_adapters-1.0.1/aws_hexagonal_adapters/ses_service.py`

 * *Files identical despite different names*

### Comparing `aws_hexagonal_adapters-1.0.0/aws_hexagonal_adapters/sqs_service.py` & `aws_hexagonal_adapters-1.0.1/aws_hexagonal_adapters/sqs_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # -*- coding: utf-8 -*-
-"""Simplify operations against AWS Simple Queue Service - SQS using AWS Python SDK boto3."""
 import os
 import json
 import boto3
 from botocore.exceptions import ClientError
 from aws_lambda_powertools import Logger
 
 LOGGER = Logger(sampling_rate=float(os.environ["LOG_SAMPLING_RATE"]))
@@ -12,33 +11,30 @@
 class BatchProcessingFailedException(Exception):
     """Raise for failed messages during processing in batch."""
 
 
 class SQSService:
     """Simplify queue operations via AWS Simple Queue Service."""
 
-    def __init__(
-        self,
-        region_name="eu-west-2",
-    ):
+    def __init__(self, region_name="eu-west-2"):
         """Initialize default region.
 
         :param region_name: the AWS region name, default eu-central-1
         """
-        self.__sqs = boto3.client("sqs", region_name=region_name)
+        self.sqs = boto3.client("sqs", region_name=region_name)
 
     def send_message_to_fifo(self, message, queue_url):
-        """Send message to the FIFO SQS queue.
+        """Send a message to the FIFO SQS queue.
 
-        :param message: message payload - string
+        :param message: Message payload - string
         :param queue_url: the AWS SQS queue URL
         :return: NotImplemented
         """
         try:
-            self.__sqs.send_message(
+            self.sqs.send_message(
                 QueueUrl=queue_url,
                 MessageBody=message["MessageBody"],
                 DelaySeconds=message["DelaySeconds"],
                 MessageAttributes=message["MessageAttributes"],
                 MessageGroupId=message["MessageGroupId"],
                 MessageDeduplicationId=message["Id"],
             )
@@ -51,27 +47,27 @@
         """Send a message to regular queue.
 
         :param message: message payload - string
         :param queue_url: the AWS SQS queue URL
         :return: NotImplemented
         """
         try:
-            self.__sqs.send_message(
+            self.sqs.send_message(
                 QueueUrl=queue_url,
                 MessageBody=message["MessageBody"],
                 DelaySeconds=message.get("DelaySeconds", 0),
                 MessageAttributes=message.get("MessageAttributes", {}),
             )
             LOGGER.info(f"Message sent to queue {queue_url}")
         except ClientError:
             LOGGER.error(f"Failed to send message to queue {queue_url}")
             raise
 
     @staticmethod
-    def __retry_failed_messages(queue_url, response, messages, retry, retry_function):
+    def _retry_failed_messages(queue_url, response, messages, retry, retry_function):
         """Retry failed messages.
 
         :param queue_url:
         :param response:
         :param messages:
         :param retry:
         :param retry_function:
@@ -88,52 +84,52 @@
         if failed:
             LOGGER.error(f"Failed to process message batch {queue_url} due to {json.dumps(failed)}")
             raise BatchProcessingFailedException()
 
     def send_messages(self, messages, queue_url, retry=3):
         """Send 10 messages in batch to the SQS queue.
 
-        :param messages: list of messages
+        :param messages: List of messages
         :param queue_url: the AWS SQS queue URL
         :param retry: number of times to retry
         :return: NotImplemented
         """
         try:
             chunk_size = 10
             for idx in range(0, len(messages), chunk_size):
                 chunk = messages[idx : idx + chunk_size]
-                response = self.__sqs.send_message_batch(QueueUrl=queue_url, Entries=chunk)
-                self.__retry_failed_messages(queue_url, response, chunk, retry, self.__sqs.send_message_batch)
+                response = self.sqs.send_message_batch(QueueUrl=queue_url, Entries=chunk)
+                self._retry_failed_messages(queue_url, response, chunk, retry, self.sqs.send_message_batch)
             LOGGER.info(f"Sent {len(messages)} message to queue {queue_url}")
         except ClientError:
             LOGGER.error(f"Failed to send message batch to queue {queue_url}")
             raise
 
     def receive_messages(self, queue_url, **kwargs):
-        """Receive defined number of messages from queue.
+        """Receive a defined number of messages from queue.
 
-        :param queue_url: the AWS SQS queue URL
+        :param queue_url: The AWS SQS queue URL
         :param kwargs: dictionary of key/value pairs to pass to SQS client
         :return: messages list
         """
         try:
             num_of_messages = kwargs.get("max_number_of_messages", 1)
             messages = []
 
             while num_of_messages > 0:
                 max_messages = min(num_of_messages, 10)
-                response = self.__sqs.receive_message(
+                response = self.sqs.receive_message(
                     QueueUrl=queue_url,
                     AttributeNames=[kwargs.get("attribute_names", "All")],
                     MaxNumberOfMessages=kwargs.get("max_messages", max_messages),
                     MessageAttributeNames=[kwargs.get("message_attribute_names", "All")],
                     WaitTimeSeconds=kwargs.get("wait_time", 3),
                 )
                 new_messages = response.get("Messages", [])
-                if len(new_messages) == 0:
+                if not new_messages:
                     LOGGER.info("No messages in queue")
                     return "No messages in queue"
                 messages.extend(new_messages)
                 num_of_messages -= max_messages
             LOGGER.info(f"Received {len(messages)} messages from queue {queue_url}")
             return messages
         except ClientError:
@@ -144,65 +140,65 @@
         """Delete a message from queue.
 
         :param queue_url: the AWS SQS queue URL
         :param receipt_handle: receipt_handle from sqs message
         :return: NotImplemented
         """
         try:
-            self.__sqs.delete_message(QueueUrl=queue_url, ReceiptHandle=receipt_handle)
+            self.sqs.delete_message(QueueUrl=queue_url, ReceiptHandle=receipt_handle)
             LOGGER.debug("Removed message from queue")
         except ClientError:
             LOGGER.error(f"Failed to delete message from queue {queue_url}")
             raise
 
     def delete_messages(self, queue_url, messages, retry=3):
         """Delete multiple messages (10) from the SQS queue.
 
-        :param queue_url: the AWS SQS queue URL
+        :param queue_url: The AWS SQS queue URL
         :param messages: list of SQS messages
         :param retry: number of times to retry
         :return: NotImplemented
         """
         try:
             chunk_size = 10
             for i in range(0, len(messages), chunk_size):
                 chunk = messages[i : i + chunk_size]
                 entries = [{"Id": x["MessageId"], "ReceiptHandle": x["ReceiptHandle"]} for x in chunk]
-                response = self.__sqs.delete_message_batch(QueueUrl=queue_url, Entries=entries)
-                self.__retry_failed_messages(queue_url, response, chunk, retry, self.__sqs.delete_message_batch)
+                response = self.sqs.delete_message_batch(QueueUrl=queue_url, Entries=entries)
+                self._retry_failed_messages(queue_url, response, chunk, retry, self.sqs.delete_message_batch)
             LOGGER.info(f"Deleted {len(messages)} message from queue {queue_url}")
         except ClientError:
             LOGGER.error(f"Failed to delete messages from queue {queue_url}")
             raise
 
     def get_queue_attr(self, queue_url, attribute_names):
         """Get SQS queue attributes.
 
         :param queue_url: the AWS SQS queue URL
         :param attribute_names: name of SQS queue attributes
         :return: attributes dict
         """
         try:
-            response = self.__sqs.get_queue_attributes(QueueUrl=queue_url, AttributeNames=attribute_names)
+            response = self.sqs.get_queue_attributes(QueueUrl=queue_url, AttributeNames=attribute_names)
             LOGGER.info(f"Got {attribute_names} attributes for queue {queue_url}")
             return response["Attributes"]
         except ClientError:
             LOGGER.error(f"Failed to get attributes for queue {queue_url}")
             raise
 
     def queue_has_messages(self, queue_name: str) -> int:
         """Check if a queue has messages.
 
-        :param queue_name: the AWS SQS queue name
+        :param queue_name: The AWS SQS queue name
         :return: number of messages
         """
         attr = self.get_queue_attr(queue_name, ["ApproximateNumberOfMessages"])
         return int(attr["ApproximateNumberOfMessages"]) > 0
 
     def queue_has_messages_in_flight(self, queue_name: str) -> int:
         """Check if a queue has messages in flight (actually processing).
 
-        :param queue_name: the AWS SQS queue name
+        :param queue_name: The AWS SQS queue name
         :return: number of messages
         """
         attr = self.get_queue_attr(queue_name, ["ApproximateNumberOfMessagesNotVisible"])
         return int(attr["ApproximateNumberOfMessagesNotVisible"]) > 0
```

### Comparing `aws_hexagonal_adapters-1.0.0/aws_hexagonal_adapters/ssm_service.py` & `aws_hexagonal_adapters-1.0.1/aws_hexagonal_adapters/ssm_service.py`

 * *Files identical despite different names*

### Comparing `aws_hexagonal_adapters-1.0.0/tests/test_s3_service.py` & `aws_hexagonal_adapters-1.0.1/tests/test_s3_service.py`

 * *Files identical despite different names*

### Comparing `aws_hexagonal_adapters-1.0.0/tests/.pytest_cache/v/cache/nodeids` & `aws_hexagonal_adapters-1.0.1/tests/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `aws_hexagonal_adapters-1.0.0/LICENSE` & `aws_hexagonal_adapters-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_hexagonal_adapters-1.0.0/pyproject.toml` & `aws_hexagonal_adapters-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aws_hexagonal_adapters"
 description = "Adapters following hexagonal architecture to connect various AWS services."
-version = "1.0.0"
+version = "1.0.1"
 authors = [{name = "Tomasz Szuster", email = "tomasz.szuster@gmail.com"}]
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 dependencies = [
         "boto3>=1.26.71,<2.0.0",
```

