# Comparing `tmp/avenieca-python-0.1.2.tar.gz` & `tmp/avenieca-python-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avenieca-python-0.1.2.tar", last modified: Tue Jan 17 15:38:28 2023, max compression
+gzip compressed data, was "avenieca-python-0.1.3.tar", last modified: Thu Jun  1 16:50:35 2023, max compression
```

## Comparing `avenieca-python-0.1.2.tar` & `avenieca-python-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:38:28.779889 avenieca-python-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-17 15:38:15.000000 avenieca-python-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-01-17 15:38:28.779889 avenieca-python-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-01-17 15:38:15.000000 avenieca-python-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:38:28.779889 avenieca-python-0.1.2/avenieca/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-01-17 15:38:15.000000 avenieca-python-0.1.2/avenieca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-01-17 15:38:15.000000 avenieca-python-0.1.2/avenieca/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-01-17 15:38:15.000000 avenieca-python-0.1.2/avenieca/producer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:38:28.779889 avenieca-python-0.1.2/avenieca/producers/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-17 15:38:15.000000 avenieca-python-0.1.2/avenieca/producers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-01-17 15:38:15.000000 avenieca-python-0.1.2/avenieca/producers/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-01-17 15:38:15.000000 avenieca-python-0.1.2/avenieca/producers/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:38:28.779889 avenieca-python-0.1.2/avenieca/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-17 15:38:15.000000 avenieca-python-0.1.2/avenieca/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-01-17 15:38:15.000000 avenieca-python-0.1.2/avenieca/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-01-17 15:38:15.000000 avenieca-python-0.1.2/avenieca/utils/signal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:38:28.779889 avenieca-python-0.1.2/avenieca_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-01-17 15:38:28.000000 avenieca-python-0.1.2/avenieca_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-01-17 15:38:28.000000 avenieca-python-0.1.2/avenieca_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 15:38:28.000000 avenieca-python-0.1.2/avenieca_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-17 15:38:28.000000 avenieca-python-0.1.2/avenieca_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-17 15:38:28.000000 avenieca-python-0.1.2/avenieca_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 15:38:28.779889 avenieca-python-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-01-17 15:38:15.000000 avenieca-python-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:38:28.779889 avenieca-python-0.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-01-17 15:38:15.000000 avenieca-python-0.1.2/test/test_producers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-01-17 15:38:15.000000 avenieca-python-0.1.2/test/test_signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:50:35.000709 avenieca-python-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-06-01 16:50:35.000709 avenieca-python-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:50:34.992709 avenieca-python-0.1.3/avenieca/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:50:34.992709 avenieca-python-0.1.3/avenieca/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/api/cortex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/api/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/api/eca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/api/ecaresponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/api/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/api/ess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/api/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/api/retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/api/sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:50:34.992709 avenieca-python-0.1.3/avenieca/api/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/api/utils/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:50:34.996709 avenieca-python-0.1.3/avenieca/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/config/broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/config/cortex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/config/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/config/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/config/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/config/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/config/ras.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/config/retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/config/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/config/twin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/config/vse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/producer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:50:34.996709 avenieca-python-0.1.3/avenieca/producers/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/producers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/producers/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/producers/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:50:34.996709 avenieca-python-0.1.3/avenieca/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/utils/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/utils/signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:50:34.996709 avenieca-python-0.1.3/avenieca_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-06-01 16:50:34.000000 avenieca-python-0.1.3/avenieca_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-01 16:50:34.000000 avenieca-python-0.1.3/avenieca_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 16:50:34.000000 avenieca-python-0.1.3/avenieca_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-01 16:50:34.000000 avenieca-python-0.1.3/avenieca_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-01 16:50:34.000000 avenieca-python-0.1.3/avenieca_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 16:50:35.000709 avenieca-python-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:50:35.000709 avenieca-python-0.1.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/test/test_producers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/test/test_signal.py
```

### Comparing `avenieca-python-0.1.2/LICENSE` & `avenieca-python-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `avenieca-python-0.1.2/avenieca/producer.py` & `avenieca-python-0.1.3/avenieca/producer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import json
+
+from avenieca.config.broker import Broker
 from kafka import KafkaProducer
 
 
 class Producer:
     """
     Base producer for publishing messages.
 
     :param config: configuration dictionary
     """
     def __init__(self,
-                 config: dict,
+                 config: Broker,
                  ):
         self.config = config
-        self.topic = config["topic"]
-        self.client = KafkaProducer(bootstrap_servers=config["bootstrap_servers"])
+        self.topic = config.sub_topic
+        self.client = KafkaProducer(bootstrap_servers=config.url)
 
     def send(self, data: dict):
         """
         :param data: serialized signal dictionary
         :return: FutureRecordMetadata
         """
         json_object = json.dumps(data).encode("utf-8")
         result = self.client.send(self.topic, json_object)
         return result
-
```

### Comparing `avenieca-python-0.1.2/avenieca/producers/event.py` & `avenieca-python-0.1.3/avenieca/producers/event.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,37 @@
+from avenieca.data import Signal
+
+from avenieca.config.broker import Broker
 from avenieca.producer import Producer
 from avenieca.utils.signal import verify_signal
 
 
 class Event(Producer):
     """
     Event producer class for syncing from an event driven source.
     Use this class if you want to handle the outer syncing logic, then pass the
     signal to the publish method to publish.
 
     :param config: configuration dictionary
     """
-    def __init__(self, config: dict):
+    def __init__(self, config: Broker):
         super().__init__(config)
         self.config = config
         self.sync = True
 
-    def publish(self, signal: dict):
+    def publish(self, signal: Signal):
         """
-        call this method with the signal dictionary to publish once to a digital twin
+        call this method with the Signal dataclass to publish once to a digital twin
 
         :param signal: signal data
         :return: None
         """
         if self.sync:
-            verify_signal(signal)
-            return self.send(signal)
+            verify_signal(signal.__dict__)
+            return self.send(signal.__dict__)
 
     @property
     def config(self):
         return self.config
 
     @config.setter
     def config(self, value):
```

### Comparing `avenieca-python-0.1.2/avenieca/producers/stream.py` & `avenieca-python-0.1.3/avenieca/producers/stream.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 import time
+
+from avenieca.config.broker import Broker
+
 from avenieca.producer import Producer
 from avenieca.utils.signal import verify_signal
 
 
 class Stream(Producer):
     """
     Stream producer class for continuous syncing at a sync_rate. Use this class if you want the
     library to handle the syncing logic for you. Provide a handler that returns the signal
     data for publishing.
 
     :param config: config dictionary
-    :param sync_rate: int (seconds) or float (sub-seconds)
+    :param sync_rate: float (time unit in seconds or sub-seconds)
     """
 
-    def __init__(self, config: dict, sync_rate: [int, float]):
+    def __init__(self, config: Broker, sync_rate: float):
         super().__init__(config)
         self.config = config
         self.sync_rate = sync_rate
         self.sync = True
 
-    def publish(self, func, sync_once=False):
+    def publish(self, func, handler_params=None, sync_once=False):
         """
         Basic publish stream timed by the sync_rate
 
-        :param func: handler to return the signal (dict data) for publishing
+        :param func: handler to return the Signal dataclass for publishing
+        :param handler_params: optional tuple of params to pass to the provided handler.
         :param sync_once: run the sync loop once
         :return: none
         """
         while self.sync:
-            signal = func()
+            if handler_params is None:
+                signal = func()
+            else:
+                signal = func(handler_params)
             verify_signal(signal)
             self.send(signal)
             if sync_once:
                 break
             time.sleep(self.sync_rate)
 
     @property
```

### Comparing `avenieca-python-0.1.2/avenieca/utils/signal.py` & `avenieca-python-0.1.3/avenieca/utils/signal.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,11 @@
 import json
 
 import numpy as np
 
-Signal = {
-    "valence": None,
-    "score": None,
-    "state": None,
-}
-
 DEFAULT_STATE_DIM = 1
 
 
 def get_state_as_array(signal, dtype=np.float64):
     state = signal["state"]
     if type(state) == str:
         state = json.loads(state)
@@ -25,36 +19,36 @@
         state = json.loads(state)
     arr = np.array(state, dtype=dtype)
     signal["state"] = arr.tolist()
 
 
 def verify_signal(signal):
     assert type(signal) == dict
-    assert len(signal) == 3
+    assert len(signal) == 4
 
     if signal["state"] is None:
         raise Exception("signal state cannot be None")
 
     if type(signal["state"]) == str:
         verify_str_shape(signal["state"])
+        signal["state"] = json.loads(signal["state"])
 
     if type(signal["state"]) == list:
         arr_list = signal["state"]
         verify_list_shape(arr_list)
         if all(isinstance(item, (int, float)) for item in arr_list):
-            signal["state"] = json.dumps(arr_list)
             return
         else:
             raise Exception("signal state values must be int or float")
 
     if type(signal["state"]) == np.ndarray:
         try:
+            verify_np_shape(signal["state"])
             arr_list = signal["state"].tolist()
-            verify_list_shape(arr_list)
-            signal["state"] = json.dumps(arr_list)
+            signal["state"] = arr_list
             return
         except Exception as e:
             raise Exception("error converting state signal from numpy array to byte string: {}".format(e))
 
 
 def verify_str_shape(state):
     if state == "":
```

### Comparing `avenieca-python-0.1.2/setup.py` & `avenieca-python-0.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,27 +6,33 @@
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).resolve().parent
 
 # The text of the README file is used as a description
 README = (HERE / "README.md").read_text()
 
-# This call to setup() does all the work
+# This call to set up() does all the work
 setup(
     name="avenieca-python",
-    version="0.1.2",
+    version="0.1.3",
     description="Python SDK for AveniECA",
     url="https://github.com/aveni-hub/avenieca-python",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Ogban Ugot",
     author_email="ogbanugot@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
-    packages=["avenieca", "avenieca/producers", "avenieca/utils"],
+    packages=[
+        "avenieca",
+        "avenieca/producers",
+        "avenieca/utils",
+        "avenieca/api",
+        "avenieca/api/utils",
+        "avenieca/config"],
     include_package_data=True,
-    install_requires=["kafka-python", "numpy"],
+    install_requires=["kafka-python", "numpy", "requests", "dataclass-wizard"],
 )
```

### Comparing `avenieca-python-0.1.2/test/test_producers.py` & `avenieca-python-0.1.3/test/test_producers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,66 @@
 import os
-import numpy as np
-from avenieca.utils import Config
-from avenieca.utils import Signal
+from avenieca.config.broker import Broker
+from avenieca.data import Signal
 from avenieca.producers import Stream
 from avenieca.producers import Event
 from avenieca.consumer import Consumer
 
 
 def consume(func, topic):
-    Config["bootstrap_servers"] = os.environ["KAFKA_URL"]
-    Config["topic"] = topic
-    client = Consumer(config=Config)
+    config = Broker(
+        url=os.environ["KAFKA_URL"],
+        sub_topic=topic,
+        group="test",
+        pub_topic=topic
+    )
+    client = Consumer(config=config)
     client.consume(func, True)
 
 
 def test_stream_publish():
     def verify(data):
         valence = data["valence"]
         state = data["state"]
-        assert valence == 10
+        assert valence == 10.0
         assert state == "[0.2, 0.3, 0.8]"
 
     def handler():
-        Signal["valence"] = 10
-        Signal["state"] = np.array([0.2, 0.3, 0.8])
-        return Signal
-
-    Config["bootstrap_servers"] = os.environ["KAFKA_URL"]
-    Config["topic"] = "test_topic_1"
-    stream = Stream(config=Config, sync_rate=1)
+        signal = Signal(
+            valence=10.0,
+            state=[0.2, 0.3, 0.8],
+        )
+        return signal
+
+    config = Broker(
+        url=os.environ["KAFKA_URL"],
+        sub_topic="test_topic_1",
+        group="test",
+        pub_topic="test_topic_1"
+    )
+    stream = Stream(config=config, sync_rate=1)
     stream.publish(handler, True)
-    consume(verify, Config["topic"])
+    consume(verify, config.sub_topic)
 
 
 def test_event_publish():
     def verify(data):
         valence = data["valence"]
         state = data["state"]
-        assert valence == 9
+        assert valence == 9.0
         assert state == "[0.1, 0.2, 0.1]"
 
     def handler():
-        Signal["valence"] = 9
-        Signal["state"] = "[0.1, 0.2, 0.1]"
-        return Signal
-
-    Config["bootstrap_servers"] = os.environ["KAFKA_URL"]
-    Config["topic"] = "test_topic_2"
-    event = Event(config=Config)
+        return Signal(
+            valence=9.0,
+            state=[0.1, 0.2, 0.1],
+        )
+
+    config = Broker(
+        url=os.environ["KAFKA_URL"],
+        sub_topic="test_topic_2",
+        group="test",
+        pub_topic="test_topic_2"
+    )
+    event = Event(config=config)
     event.publish(handler())
-    consume(verify, Config["topic"])
+    consume(verify, config.sub_topic)
```

### Comparing `avenieca-python-0.1.2/test/test_signal.py` & `avenieca-python-0.1.3/test/test_signal.py`

 * *Files 19% similar despite different names*

```diff
@@ -38,27 +38,30 @@
     assert signal["state"] == [9.1, 2.1, 0.3]
 
 
 def test_verify_signal():
     signal = {
         "valence": None,
         "score": None,
-        "state": "[9.1, 2.1, 0.3]"
+        "state": "[9.1, 2.1, 0.3]",
+        "embedding_input": None,
     }
     verify_signal(signal)
-    assert signal["state"] == "[9.1, 2.1, 0.3]"
+    assert signal["state"] == [9.1, 2.1, 0.3]
 
     signal = {
         "valence": None,
         "score": None,
-        "state": np.array([9.1, 2.1, 0.3])
+        "state": np.array([9.1, 2.1, 0.3]),
+        "embedding_input": None,
     }
     verify_signal(signal)
-    assert signal["state"] == "[9.1, 2.1, 0.3]"
+    assert signal["state"] == [9.1, 2.1, 0.3]
 
     signal = {
         "valence": None,
         "score": None,
-        "state": [9.1, 2.1, 0.3]
+        "state": [9.1, 2.1, 0.3],
+        "embedding_input": None,
     }
     verify_signal(signal)
-    assert signal["state"] == "[9.1, 2.1, 0.3]"
+    assert signal["state"] == [9.1, 2.1, 0.3]
```

