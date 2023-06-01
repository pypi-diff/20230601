# Comparing `tmp/qldebugger-0.1.0.tar.gz` & `tmp/qldebugger-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qldebugger-0.1.0.tar", max compression
+gzip compressed data, was "qldebugger-0.2.0.tar", max compression
```

## Comparing `qldebugger-0.1.0.tar` & `qldebugger-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1084 2022-08-22 01:00:47.477744 qldebugger-0.1.0/LICENSE
--rw-r--r--   0        0        0       73 2022-08-22 01:00:47.477744 qldebugger-0.1.0/README.md
--rw-r--r--   0        0        0     2643 2022-08-22 01:00:47.477744 qldebugger-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-08-22 01:00:47.477744 qldebugger-0.1.0/qldebugger/__init__.py
--rw-r--r--   0        0        0       28 2022-08-22 01:00:47.477744 qldebugger-0.1.0/qldebugger/__main__.py
--rw-r--r--   0        0        0      240 2022-08-22 01:00:47.477744 qldebugger-0.1.0/qldebugger/actions/__init__.py
--rw-r--r--   0        0        0     2140 2022-08-22 01:00:47.481744 qldebugger-0.1.0/qldebugger/actions/event_source_mapping.py
--rw-r--r--   0        0        0      354 2022-08-22 01:00:47.481744 qldebugger-0.1.0/qldebugger/actions/infra.py
--rw-r--r--   0        0        0     1362 2022-08-22 01:00:47.481744 qldebugger-0.1.0/qldebugger/actions/lambda_.py
--rw-r--r--   0        0        0     1857 2022-08-22 01:00:47.481744 qldebugger-0.1.0/qldebugger/actions/message.py
--rw-r--r--   0        0        0     2553 2022-08-22 01:00:47.481744 qldebugger-0.1.0/qldebugger/aws.py
--rw-r--r--   0        0        0     1806 2022-08-22 01:00:47.481744 qldebugger-0.1.0/qldebugger/cli.py
--rw-r--r--   0        0        0      598 2022-08-22 01:00:47.481744 qldebugger-0.1.0/qldebugger/config/__init__.py
--rw-r--r--   0        0        0     1420 2022-08-22 01:00:47.481744 qldebugger-0.1.0/qldebugger/config/file_parser.py
--rw-r--r--   0        0        0        0 2022-08-22 01:00:47.481744 qldebugger-0.1.0/qldebugger/example/__init__.py
--rw-r--r--   0        0        0      392 2022-08-22 01:00:47.481744 qldebugger-0.1.0/qldebugger/example/lambdas.py
--rw-r--r--   0        0        0        0 2022-08-22 01:00:47.481744 qldebugger-0.1.0/qldebugger/py.typed
--rw-r--r--   0        0        0      996 2022-08-22 01:00:57.893921 qldebugger-0.1.0/setup.py
--rw-r--r--   0        0        0     1424 2022-08-22 01:00:57.894204 qldebugger-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-06-01 03:42:46.844432 qldebugger-0.2.0/LICENSE
+-rw-r--r--   0        0        0       73 2023-06-01 03:42:46.844432 qldebugger-0.2.0/README.md
+-rw-r--r--   0        0        0     2352 2023-06-01 03:42:46.844432 qldebugger-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-01 03:42:46.844432 qldebugger-0.2.0/qldebugger/__init__.py
+-rw-r--r--   0        0        0       28 2023-06-01 03:42:46.844432 qldebugger-0.2.0/qldebugger/__main__.py
+-rw-r--r--   0        0        0      146 2023-06-01 03:42:46.844432 qldebugger-0.2.0/qldebugger/actions/__init__.py
+-rw-r--r--   0        0        0     2099 2023-06-01 03:42:46.844432 qldebugger-0.2.0/qldebugger/actions/event_source_mapping.py
+-rw-r--r--   0        0        0     2910 2023-06-01 03:42:46.844432 qldebugger-0.2.0/qldebugger/actions/infra.py
+-rw-r--r--   0        0        0     1366 2023-06-01 03:42:46.844432 qldebugger-0.2.0/qldebugger/actions/lambda_.py
+-rw-r--r--   0        0        0     2359 2023-06-01 03:42:46.844432 qldebugger-0.2.0/qldebugger/actions/message.py
+-rw-r--r--   0        0        0     2978 2023-06-01 03:42:46.844432 qldebugger-0.2.0/qldebugger/aws.py
+-rw-r--r--   0        0        0     3008 2023-06-01 03:42:46.844432 qldebugger-0.2.0/qldebugger/cli.py
+-rw-r--r--   0        0        0      620 2023-06-01 03:42:46.844432 qldebugger-0.2.0/qldebugger/config/__init__.py
+-rw-r--r--   0        0        0     2232 2023-06-01 03:42:46.844432 qldebugger-0.2.0/qldebugger/config/file_parser.py
+-rw-r--r--   0        0        0        0 2023-06-01 03:42:46.844432 qldebugger-0.2.0/qldebugger/example/__init__.py
+-rw-r--r--   0        0        0      482 2023-06-01 03:42:46.844432 qldebugger-0.2.0/qldebugger/example/lambdas.py
+-rw-r--r--   0        0        0        0 2023-06-01 03:42:46.844432 qldebugger-0.2.0/qldebugger/py.typed
+-rw-r--r--   0        0        0     1305 1970-01-01 00:00:00.000000 qldebugger-0.2.0/PKG-INFO
```

### Comparing `qldebugger-0.1.0/LICENSE` & `qldebugger-0.2.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2022 Eduardo Klosowski
+Copyright (c) 2022-2023 Eduardo Klosowski
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `qldebugger-0.1.0/qldebugger/actions/event_source_mapping.py` & `qldebugger-0.2.0/qldebugger/actions/event_source_mapping.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import logging
 from typing import TYPE_CHECKING
 
-from ..aws import get_client
-from ..config import get_config
+from qldebugger.aws import get_account_id, get_client
+from qldebugger.config import get_config
+
 from .lambda_ import run_lambda
 from .message import delete_messages, receive_message
 
 if TYPE_CHECKING:
     from aws_lambda_typing.events import SQSEvent
     from mypy_boto3_sqs.type_defs import ReceiveMessageResultTypeDef
 
 logger = logging.getLogger(__name__)
 
 
 def receive_messages_and_run_lambda(*, event_source_mapping_name: str) -> None:
-    logger.debug('Execute %r event source mapping...', event_source_mapping_name)
-    sts = get_client('sts')
     sqs = get_client('sqs')
     event_source_mapping = get_config().event_source_mapping[event_source_mapping_name]
 
-    account_id = sts.get_caller_identity()['Account']
-    queue_arn = f'arn:{sqs.meta.partition}:sqs:{sqs.meta.region_name}:{account_id}:{event_source_mapping.queue}'
+    queue_arn = f'arn:{sqs.meta.partition}:sqs:{sqs.meta.region_name}:{get_account_id()}:{event_source_mapping.queue}'
 
+    logger.debug('Execute %r event source mapping...', event_source_mapping_name)
     messages = receive_message(
         queue_name=event_source_mapping.queue,
         batch_size=event_source_mapping.batch_size,
         maximum_batching_window=event_source_mapping.maximum_batching_window,
     )
     event = convert_sqs_messages_to_event(
         aws_region=sqs.meta.region_name,
```

### Comparing `qldebugger-0.1.0/qldebugger/actions/lambda_.py` & `qldebugger-0.2.0/qldebugger/actions/lambda_.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 import logging
 from importlib import import_module
 from traceback import format_exc
 from typing import TYPE_CHECKING, Any, Callable
 from unittest.mock import patch
 
 from qldebugger.aws import inject_aws_config_in_client
-
-from ..config import get_config
+from qldebugger.config import get_config
 
 if TYPE_CHECKING:
     from aws_lambda_typing.events import SQSEvent
 
 logger = logging.getLogger(__name__)
 
 
 def get_lambda_function(*, lambda_name: str) -> Callable[['SQSEvent', None], Any]:
-    logger.debug('Importing lambda_handler of %r...', lambda_name)
     module_name, function_name = get_config().lambdas[lambda_name].handler
+    logger.debug('Importing lambda_handler of %r...', lambda_name)
     lambda_handler: Callable[['SQSEvent', None], Any] = \
         getattr(import_module(module_name), function_name)
     return lambda_handler
 
 
 def run_lambda(*, lambda_name: str, event: 'SQSEvent') -> Any:
     environment = get_config().lambdas[lambda_name].environment
     with patch('boto3.client', inject_aws_config_in_client):
         lambda_handler = get_lambda_function(lambda_name=lambda_name)
         logger.info('Running %r lambda...', lambda_name)
         try:
             with patch.dict('os.environ', environment, True):
                 result = lambda_handler(event, None)
-            logger.info('Result: %r', result)
-            return result
         except Exception:
-            logger.error('Error on execute lambda:\n%s', format_exc())
+            logger.exception('Error on execute lambda:\n%s', format_exc())
             raise
+        logger.info('Result: %r', result)
+        return result
```

### Comparing `qldebugger-0.1.0/qldebugger/actions/message.py` & `qldebugger-0.2.0/qldebugger/actions/message.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,52 +1,69 @@
 import logging
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Mapping
 
-from ..aws import get_client
+from qldebugger.aws import get_account_id, get_client
 
 if TYPE_CHECKING:
+    from mypy_boto3_sns.type_defs import MessageAttributeValueTypeDef
     from mypy_boto3_sqs.type_defs import ReceiveMessageResultTypeDef
 
 
 logger = logging.getLogger(__name__)
 
 
+def publish_message(
+    *,
+    topic_name: str,
+    message: str,
+    attributes: Mapping[str, 'MessageAttributeValueTypeDef'] = {},
+) -> None:
+    sns = get_client('sns')
+    arn = f'arn:aws:sns:{sns.meta.region_name}:{get_account_id()}:{topic_name}'
+    logger.info('Sending message to %r topic...', topic_name)
+    sns.publish(
+        TopicArn=arn,
+        Message=message,
+        MessageAttributes=attributes,
+    )
+
+
 def send_message(*, queue_name: str, message: str) -> None:
+    sqs = get_client('sqs')
+    queue_url = sqs.get_queue_url(QueueName=queue_name)['QueueUrl']
     logger.info('Sending message to %r queue...', queue_name)
-    client = get_client('sqs')
-    queue_url = client.get_queue_url(QueueName=queue_name)['QueueUrl']
-    client.send_message(QueueUrl=queue_url, MessageBody=message)
+    sqs.send_message(QueueUrl=queue_url, MessageBody=message)
 
 
 def receive_message(
     *,
     queue_name: str,
     batch_size: int,
     maximum_batching_window: int,
 ) -> 'ReceiveMessageResultTypeDef':
+    sqs = get_client('sqs')
+    queue_url = sqs.get_queue_url(QueueName=queue_name)['QueueUrl']
     logger.debug('Receiving messages from %r queue...', queue_name)
-    client = get_client('sqs')
-    queue_url = client.get_queue_url(QueueName=queue_name)['QueueUrl']
-    messages = client.receive_message(
+    messages = sqs.receive_message(
         QueueUrl=queue_url,
         MaxNumberOfMessages=batch_size,
         WaitTimeSeconds=maximum_batching_window,
     )
     if 'Messages' not in messages:
         logger.warning('No messages received from %r queue', queue_name)
         raise RuntimeWarning('No messages received')
     logger.info('Receved %d messages from %r queue', len(messages['Messages']), queue_name)
     return messages
 
 
 def delete_messages(*, queue_name: str, messages: 'ReceiveMessageResultTypeDef') -> None:
+    sqs = get_client('sqs')
+    queue_url = sqs.get_queue_url(QueueName=queue_name)['QueueUrl']
     logger.debug('Deleting messages of %r queue...', queue_name)
-    client = get_client('sqs')
-    queue_url = client.get_queue_url(QueueName=queue_name)['QueueUrl']
-    client.delete_message_batch(
+    sqs.delete_message_batch(
         QueueUrl=queue_url,
         Entries=[
             {
                 'Id': message['MessageId'],
                 'ReceiptHandle': message['ReceiptHandle'],
             } for message in messages['Messages']
         ],
```

### Comparing `qldebugger-0.1.0/qldebugger/aws.py` & `qldebugger-0.2.0/qldebugger/aws.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,21 +4,31 @@
 
 import boto3
 from botocore.config import Config
 
 from .config import get_config
 
 if TYPE_CHECKING:
+    from mypy_boto3_secretsmanager import SecretsManagerClient
+    from mypy_boto3_sns import SNSClient
     from mypy_boto3_sqs import SQSClient
     from mypy_boto3_sts import STSClient
 
 logger = logging.getLogger(__name__)
 
 
 @overload
+def get_client(service_name: Literal['secretsmanager'], /) -> 'SecretsManagerClient': ...
+
+
+@overload
+def get_client(service_name: Literal['sns'], /) -> 'SNSClient': ...
+
+
+@overload
 def get_client(service_name: Literal['sqs'], /) -> 'SQSClient': ...
 
 
 @overload
 def get_client(service_name: Literal['sts'], /) -> 'STSClient': ...
 
 
@@ -34,15 +44,20 @@
     )
     return session.client(
         service_name=service_name,
         endpoint_url=aws_config.endpoint_url,
     )
 
 
-get_client = lru_cache(maxsize=None)(get_client)  # type: ignore
+get_client = lru_cache(maxsize=None)(get_client)  # type: ignore[assignment]
+
+
+def get_account_id() -> str:
+    sts = get_client('sts')
+    return sts.get_caller_identity()['Account']
 
 
 def inject_aws_config_in_client(
     service_name: str,
     region_name: Optional[str] = None,
     api_version: Optional[str] = None,
     use_ssl: Optional[bool] = True,
@@ -67,15 +82,15 @@
     session = boto3.Session(
         aws_access_key_id=aws_access_key_id,
         aws_secret_access_key=aws_secret_access_key,
         aws_session_token=aws_session_token,
         region_name=region_name,
         profile_name=aws_config.profile,
     )
-    return session.client(  # type: ignore
+    return session.client(  # type: ignore[call-overload,misc]
         service_name=service_name,
         api_version=api_version,
         use_ssl=use_ssl,
         verify=verify,
         endpoint_url=endpoint_url,
         config=config,
     )
```

### Comparing `qldebugger-0.1.0/qldebugger/cli.py` & `qldebugger-0.2.0/qldebugger/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,21 @@
+import json
 import logging
-import os
+from pathlib import Path
+from typing import TYPE_CHECKING, Mapping
 
 import click
 
 from . import actions
 from .config import load_config
 
-CONFIG_FILENAME = 'qldebugger.toml'
+if TYPE_CHECKING:
+    from mypy_boto3_sns.type_defs import MessageAttributeValueTypeDef
+
+CONFIG_FILENAME = Path('qldebugger.toml')
 
 
 @click.group()
 def cli() -> None:
     logging.basicConfig(level=logging.INFO, format='%(levelname)s:qldebugger:%(message)s')
 
 
@@ -34,18 +39,18 @@
 [lambdas.fail.environment]
 VARIABLE = "VALUE"
 
 [event_source_mapping]
 a = {queue = "myqueue", function_name = "print"}
 b = {queue = "myqueue", function_name = "fail", batch_size = 1, maximum_batching_window = 20}
 '''
-    if os.path.exists(CONFIG_FILENAME):
+    if CONFIG_FILENAME.exists():
         click.echo('Configuration file already exists')
         return
-    with open(CONFIG_FILENAME, 'w') as fp:
+    with CONFIG_FILENAME.open('w') as fp:
         fp.write(config)
     click.echo('Configuration file created')
 
 
 @cli.command()
 @click.argument('event_source_mapping_name')
 def run(event_source_mapping_name: str) -> None:
@@ -56,26 +61,62 @@
 # Infra
 
 @cli.group()
 def infra() -> None:
     ...
 
 
+@infra.command('create-secrets')
+def infra_create_secrets() -> None:
+    load_config(CONFIG_FILENAME)
+    actions.infra.create_secrets()
+
+
+@infra.command('create-topics')
+def infra_create_topics() -> None:
+    load_config(CONFIG_FILENAME)
+    actions.infra.create_topics()
+
+
 @infra.command('create-queues')
 def infra_create_queues() -> None:
     load_config(CONFIG_FILENAME)
     actions.infra.create_queues()
 
 
+@infra.command('create-all')
+def infra_create_all() -> None:
+    load_config(CONFIG_FILENAME)
+    actions.infra.create_secrets()
+    actions.infra.create_topics()
+    actions.infra.create_queues()
+    actions.infra.subscribe_topics()
+
+
+@infra.command('subscribe-topics')
+def infra_subscribe_topics() -> None:
+    load_config(CONFIG_FILENAME)
+    actions.infra.subscribe_topics()
+
+
 # Msg
 
 @cli.group()
 def msg() -> None:
     ...
 
 
+@msg.command('publish')
+@click.argument('topic_name')
+@click.argument('message')
+@click.argument('attributes', default='{}', type=json.loads)
+def msg_publish(topic_name: str, message: str, attributes: Mapping[str, 'MessageAttributeValueTypeDef']) -> None:
+    load_config(CONFIG_FILENAME)
+    actions.message.publish_message(topic_name=topic_name, message=message, attributes=attributes)
+
+
 @msg.command('send')
 @click.argument('queue_name')
 @click.argument('message')
 def msg_send(queue_name: str, message: str) -> None:
     load_config(CONFIG_FILENAME)
     actions.message.send_message(queue_name=queue_name, message=message)
```

### Comparing `qldebugger-0.1.0/qldebugger/config/__init__.py` & `qldebugger-0.2.0/qldebugger/config/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 logger = logging.getLogger(__name__)
 
 _current_config: Optional[Config] = None
 
 
 def load_config(filename: Union[str, Path], /) -> Config:
     logger.debug('Loading %r config...', str(filename))
-    global _current_config
-    with open(filename, 'rb') as fp:
+    global _current_config  # noqa: PLW0603
+    with Path(filename).open('rb') as fp:
         _current_config = Config.from_toml(fp)
     return _current_config
 
 
 def get_config() -> Config:
     if _current_config is None:
         raise RuntimeError('Configuration file is not loaded yet')
```

### Comparing `qldebugger-0.1.0/qldebugger/config/file_parser.py` & `qldebugger-0.2.0/qldebugger/config/file_parser.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,53 @@
-from typing import Any, BinaryIO, Dict, NamedTuple, Optional, Tuple
+from abc import ABC, abstractmethod
+from typing import Any, BinaryIO, Dict, List, NamedTuple, Optional, Tuple, Union
 
 import tomli
 from pydantic import BaseModel, Field, validator
 
 
 class ConfigAWS(BaseModel):
     profile: Optional[str]
     access_key_id: Optional[str]
     secret_access_key: Optional[str]
     session_token: Optional[str]
     region: Optional[str]
     endpoint_url: Optional[str]
 
 
+class ConfigSecret(BaseModel, ABC):
+    @abstractmethod
+    def get_value(self) -> Union[str, bytes]:
+        ...
+
+
+class ConfigSecretString(ConfigSecret):
+    string: str
+
+    def get_value(self) -> str:
+        return self.string
+
+
+class ConfigSecretBinary(ConfigSecret):
+    binary: bytes
+
+    def get_value(self) -> bytes:
+        return self.binary
+
+
+class ConfigTopicSubscriber(BaseModel):
+    queue: str
+    raw_message_delivery: bool = False
+    filter_policy: Optional[str] = None
+
+
+class ConfigTopic(BaseModel):
+    subscribers: List[ConfigTopicSubscriber] = Field(default_factory=list)
+
+
 class ConfigQueue(BaseModel):
     ...
 
 
 class NameHandlerTuple(NamedTuple):
     module: str
     function: str
@@ -25,15 +56,15 @@
 class ConfigLambda(BaseModel):
     handler: NameHandlerTuple
     environment: Dict[str, str] = Field(default_factory=dict)
 
     @validator('handler', pre=True)
     def _split_handler(cls, v: Any) -> Tuple[str, str]:
         if not isinstance(v, str):
-            raise ValueError('should be a str')
+            raise TypeError('should be a str')
         if '.' not in v:
             raise ValueError('should have a module and function names')
         module, function = v.rsplit('.', maxsplit=1)
         return module, function
 
 
 class ConfigEventSourceMapping(BaseModel):
@@ -41,14 +72,16 @@
     batch_size: int = 10
     maximum_batching_window: int = 0
     function_name: str
 
 
 class Config(BaseModel):
     aws: ConfigAWS = Field(default_factory=ConfigAWS)
+    secrets: Dict[str, Union[ConfigSecretString, ConfigSecretBinary]] = Field(default_factory=dict)
+    topics: Dict[str, ConfigTopic] = Field(default_factory=dict)
     queues: Dict[str, ConfigQueue]
     lambdas: Dict[str, ConfigLambda]
     event_source_mapping: Dict[str, ConfigEventSourceMapping]
 
     @classmethod
     def from_toml(cls, fp: BinaryIO, /) -> 'Config':
         return cls.parse_obj(tomli.load(fp))
```

### Comparing `qldebugger-0.1.0/PKG-INFO` & `qldebugger-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 Metadata-Version: 2.1
 Name: qldebugger
-Version: 0.1.0
+Version: 0.2.0
 Summary: Utility to debug AWS lambdas with SQS messages
 Home-page: https://github.com/eduardoklosowski/qldebugger
 License: MIT
 Author: Eduardo Klosowski
 Author-email: eduardo_klosowski@yahoo.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: System :: Emulators
 Classifier: Typing :: Typed
-Requires-Dist: boto3 (>=1.24,<2.0)
+Requires-Dist: boto3 (>=1.26,<2.0)
 Requires-Dist: click (>=8.1,<9.0)
-Requires-Dist: pydantic (>=1.9,<2.0)
+Requires-Dist: pydantic (>=1.10,<2.0)
 Requires-Dist: tomli (>=2.0,<3.0)
 Project-URL: Documentation, http://qldebugger.readthedocs.io/
 Project-URL: Repository, https://github.com/eduardoklosowski/qldebugger
 Description-Content-Type: text/markdown
 
 # Queue Lambda Debugger
```

