# Comparing `tmp/hecho-events-1.3.3.tar.gz` & `tmp/hecho-events-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hecho-events-1.3.3.tar", last modified: Thu May 26 13:43:12 2022, max compression
+gzip compressed data, was "hecho-events-1.3.4.tar", last modified: Thu Jun  1 13:13:54 2023, max compression
```

## Comparing `hecho-events-1.3.3.tar` & `hecho-events-1.3.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-05-26 13:43:12.796811 hecho-events-1.3.3/
--rw-rw-rw-   0        0        0     1081 2022-05-25 18:21:05.000000 hecho-events-1.3.3/LICENSE
--rw-rw-rw-   0        0        0      988 2022-05-26 13:43:12.794639 hecho-events-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0      685 2022-05-26 13:42:56.000000 hecho-events-1.3.3/README.md
-drwxrwxrwx   0        0        0        0 2022-05-26 13:43:12.728536 hecho-events-1.3.3/hecho_events/
--rw-rw-rw-   0        0        0     5603 2022-05-25 18:21:05.000000 hecho-events-1.3.3/hecho_events/main.py
-drwxrwxrwx   0        0        0        0 2022-05-26 13:43:12.790136 hecho-events-1.3.3/hecho_events.egg-info/
--rw-rw-rw-   0        0        0      988 2022-05-26 13:43:12.000000 hecho-events-1.3.3/hecho_events.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2022-05-26 13:43:12.000000 hecho-events-1.3.3/hecho_events.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       33 2022-05-26 13:43:12.000000 hecho-events-1.3.3/hecho_events.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2022-05-26 13:43:12.000000 hecho-events-1.3.3/hecho_events.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-05-26 13:43:12.000000 hecho-events-1.3.3/hecho_events.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-05-26 13:43:12.797631 hecho-events-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0      568 2022-05-26 13:43:03.000000 hecho-events-1.3.3/setup.py
+drwxrwxr-x   0 matheus.vieira  (1001) matheus.vieira  (1001)        0 2023-06-01 13:13:54.403475 hecho-events-1.3.4/
+-rw-rw-r--   0 matheus.vieira  (1001) matheus.vieira  (1001)     1061 2023-06-01 12:33:09.000000 hecho-events-1.3.4/LICENSE
+-rw-rw-r--   0 matheus.vieira  (1001) matheus.vieira  (1001)     1320 2023-06-01 13:13:54.403475 hecho-events-1.3.4/PKG-INFO
+-rw-rw-r--   0 matheus.vieira  (1001) matheus.vieira  (1001)      771 2023-06-01 12:47:56.000000 hecho-events-1.3.4/README.md
+drwxrwxr-x   0 matheus.vieira  (1001) matheus.vieira  (1001)        0 2023-06-01 13:13:54.403475 hecho-events-1.3.4/hecho_events/
+-rw-rw-r--   0 matheus.vieira  (1001) matheus.vieira  (1001)     6068 2023-06-01 12:37:01.000000 hecho-events-1.3.4/hecho_events/main.py
+drwxrwxr-x   0 matheus.vieira  (1001) matheus.vieira  (1001)        0 2023-06-01 13:13:54.403475 hecho-events-1.3.4/hecho_events.egg-info/
+-rw-rw-r--   0 matheus.vieira  (1001) matheus.vieira  (1001)     1320 2023-06-01 13:13:54.000000 hecho-events-1.3.4/hecho_events.egg-info/PKG-INFO
+-rw-rw-r--   0 matheus.vieira  (1001) matheus.vieira  (1001)      226 2023-06-01 13:13:54.000000 hecho-events-1.3.4/hecho_events.egg-info/SOURCES.txt
+-rw-rw-r--   0 matheus.vieira  (1001) matheus.vieira  (1001)       33 2023-06-01 13:13:54.000000 hecho-events-1.3.4/hecho_events.egg-info/dependency_links.txt
+-rw-rw-r--   0 matheus.vieira  (1001) matheus.vieira  (1001)       15 2023-06-01 13:13:54.000000 hecho-events-1.3.4/hecho_events.egg-info/requires.txt
+-rw-rw-r--   0 matheus.vieira  (1001) matheus.vieira  (1001)       13 2023-06-01 13:13:54.000000 hecho-events-1.3.4/hecho_events.egg-info/top_level.txt
+-rw-rw-r--   0 matheus.vieira  (1001) matheus.vieira  (1001)       38 2023-06-01 13:13:54.403475 hecho-events-1.3.4/setup.cfg
+-rw-rw-r--   0 matheus.vieira  (1001) matheus.vieira  (1001)      552 2023-06-01 13:13:49.000000 hecho-events-1.3.4/setup.py
```

### Comparing `hecho-events-1.3.3/LICENSE` & `hecho-events-1.3.4/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 hecho
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2021 hecho
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `hecho-events-1.3.3/PKG-INFO` & `hecho-events-1.3.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,34 @@
-Metadata-Version: 2.1
-Name: hecho-events
-Version: 1.3.3
-Summary: Event Broker Rasa
-Home-page: UNKNOWN
-Author: Compasso UOL
-Author-email: hecho.teste@outlook.com
-License: MIT License
-Keywords: Pacote hecho
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Hecho-events
-
-Event Broker for Rasa Chatbot to send metrics to [Hecho Dashboard](https://hecho.ml).
-
-Start **monitoring** your **Rasa Chatbot** right now, access [https://hecho.ml](https://hecho.ml)!!
-
-## Getting Started
-
-```
-pip install hecho-events
-```
-
-Register at [https://hecho.ml](https://hecho.ml) to get an api key.
-
-After install add this entries to `endpoints.yml`:
-```yaml
-# endpoints.yml
-event_broker:
-  type: hecho_events.main.RasaEventBroker
-  api_key: "<your-api-key>"
-  api_url : "https://hecho.ml/api"
-```
-
-
-## About Hecho
-
-**Hecho Dashboard** is a platform to store and show messaging, users, intents and much more from your **chatbot**.
-
-
+# Hecho-events
+
+Event Broker for Rasa Chatbot to send metrics to [Hecho Dashboard](https://hecho.ml).
+
+Start **monitoring** your **Rasa Chatbot** right now, access [https://hecho.ml](https://hecho.ml)!!
+
+## Getting Started
+
+```
+pip install hecho-events aiohttp
+```
+
+Register at [https://hecho.ml](https://hecho.ml) to get an api key.
+
+After install add this entries to `endpoints.yml`:
+```yaml
+# endpoints.yml
+event_broker:
+  type: hecho-events.main.RasaEventBroker
+  api_key: "<your-api-key>"
+  api_url : "https://localhost:6000"
+```
+Get bridge-endpoint uri and change the api_url with him.
+
+## Dependencies
+
+```
+pip install aiohttp
+```
+
+
+## About Hecho
+
+**Hecho Dashboard** is a platform to store and show messaging, users, intents and much more from your **chatbot**.
```

### Comparing `hecho-events-1.3.3/hecho_events/main.py` & `hecho-events-1.3.4/hecho_events/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,141 +1,174 @@
-import atexit
-import json
-import asyncio
-from aiohttp import ClientSession, TCPConnector
-
-# default send interval is in seconds
-DEFAULT_SEND_INTERVAL = 5
-
-# default max size before sending
-DEFAULT_MAX_QUEUE_SIZE = 100
-
-# default value for max retries on failure
-DEFAULT_MAX_RETRIES = 5
-
-
-class RasaEventBroker():
-    def __init__(self, api_key, api_url, max_queue_size = DEFAULT_MAX_QUEUE_SIZE, send_interval = DEFAULT_SEND_INTERVAL, max_retries = DEFAULT_MAX_RETRIES, enable_debug = False):
-        if max_retries < 0:
-            raise Exception("max_retries must be >= 0")
-        if max_queue_size <= 0:
-            raise Exception("max_queue_size must be > 0")
-        if send_interval <= 0:
-            raise Exception("send_interval must be > 0")
-
-        self.api_key = api_key
-        self.api_url = api_url
-        self.max_queue_size = max_queue_size
-        self.send_interval = send_interval
-        self.enable_debug = enable_debug
-        self.max_retries = max_retries
-
-        self.events_count = 0
-        self.send_events_count = 0
-        self.requests_count = 0
-
-        self.queue = list()
-        self.loop = asyncio.get_event_loop()
-        self.task = self.loop.create_task(self.start_loop())
-        connection_pool = TCPConnector(limit=15, limit_per_host=15)
-        self._http_client = ClientSession(connector=connection_pool, trust_env=True)
-
-        atexit.register(self._shutdown)
-
-    def debug(self, str):
-        if self.enable_debug:
-            print(str)
-
-    def insert_entities_text(self, text, entities):
-        for entity in entities:
-            entity["text"] = text[entity["start"]:entity["end"]]
-        return entities
-
-    def check_duplicate_entities(self, entities):
-        entities_start = list()
-        new_entities = list()
-        entities = sorted(entities, key=lambda entity: entity['start'])
-        for entity in entities:
-            if entity["start"] not in entities_start:
-                entities_start.append(entity["start"])
-                new_entities.append(entity)
-        return new_entities
-
-    ## called by Rasa on events
-    def publish(self, event):
-        try:
-            if event['event'] == 'user':
-                text = event['text']
-                new_text = text
-                event['parse_data']['entities'] = self.insert_entities_text(text, event["parse_data"]["entities"])
-                entities = self.check_duplicate_entities(event['parse_data']['entities'])
-                event['handled'] = event['parse_data']['intent']['name'] != 'nlu_fallback'
-                for entity in entities:
-                    dict_entity = {'entity': entity['entity'], 'value': entity['value']}
-                    new_text = new_text.replace(entity["text"], f"[{entity['text']}]{json.dumps(dict_entity)}", 1)
-                event['text'] = new_text
-            if event['event'] in ['session_started', 'user', 'bot']:
-                self.add_to_queue(event)
-        except:
-            print('Failed to add event to queue')
-
-    def add_to_queue(self, event):
-        self.events_count += 1
-        self.queue.append(event)
-        if len(self.queue) >= self.max_queue_size:
-            self.create_flush_task()
-
-    async def flush(self, events):
-        self.requests_count +=1
-        count = self.requests_count
-        for retry in range(self.max_retries + 1):
-            try:
-                url = f"{self.api_url}/track"
-                params = {
-                    "apiKey": self.api_key,
-                    "platform": "rasa"
-                }
-                async with self._http_client.post(url, params=params, json=events) as request:
-                    await request.read()
-                    if request.status == 201:
-                        self.send_events_count += len(events)
-                        self.debug(f"{count} Sent {len(events)} events to Hecho after {retry} retries!")
-                        return
-                    elif retry == self.max_retries:
-                        print(f"Failed sending {len(events)} events to Hecho after {retry} retries with status code:{request.status}")
-                        return
-                    self.debug(f"Failed sending {len(events)} events to Hecho after {retry} retries with status code:{request.status}, retrying...")
-            except RuntimeError as e:
-                if retry == self.max_retries:
-                    print(f"RuntimeError: Failed to send events to Hecho after {retry} retries", e)
-            except Exception as e:
-                if retry == self.max_retries:
-                    print(f"Exception: Failed to send events to Hecho after {retry} retries: {e.message}")
-
-    def create_flush_task(self):
-        if len(self.queue) <= 0:
-            return
-        events = self.queue
-        self.queue = list()
-        self.loop.create_task(self.flush(events))
-
-    async def start_loop(self):
-        try:
-            while True:
-                await asyncio.sleep(self.send_interval)
-                self.create_flush_task()
-        except:
-            self.debug('Exiting Hecho Events Broker...')
-
-    ## called by Rasa on close bot
-    async def close(self):
-        self.task.cancel()
-        self.create_flush_task()
-
-    def _shutdown(self):
-        asyncio.run(self._http_client.close())
-
-    @classmethod
-    async def from_endpoint_config(cls, broker_config):
-        if broker_config is None:
-            return None
-        return cls(**broker_config.kwargs)
+import atexit
+import json
+import asyncio
+from aiohttp import ClientSession, TCPConnector
+
+# default send interval is in seconds
+DEFAULT_SEND_INTERVAL = 5
+
+# default max size before sending
+DEFAULT_MAX_QUEUE_SIZE = 100
+
+# default value for max retries on failure
+DEFAULT_MAX_RETRIES = 5
+
+
+class RasaEventBroker:
+    def __init__(
+        self,
+        api_key,
+        api_url,
+        max_queue_size=DEFAULT_MAX_QUEUE_SIZE,
+        send_interval=DEFAULT_SEND_INTERVAL,
+        max_retries=DEFAULT_MAX_RETRIES,
+        enable_debug=False,
+    ):
+        if max_retries < 0:
+            raise Exception('max_retries must be >= 0')
+        if max_queue_size <= 0:
+            raise Exception('max_queue_size must be > 0')
+        if send_interval <= 0:
+            raise Exception('send_interval must be > 0')
+
+        self.api_key = api_key
+        self.api_url = api_url
+        self.max_queue_size = max_queue_size
+        self.send_interval = send_interval
+        self.enable_debug = enable_debug
+        self.max_retries = max_retries
+
+        self.events_count = 0
+        self.send_events_count = 0
+        self.requests_count = 0
+
+        self.queue = list()
+        self.loop = asyncio.get_event_loop()
+        self.task = self.loop.create_task(self.start_loop())
+        connection_pool = TCPConnector(limit=15, limit_per_host=15)
+        self._http_client = ClientSession(
+            connector=connection_pool, trust_env=True
+        )
+
+        atexit.register(self._shutdown)
+
+    def debug(self, str):
+        if self.enable_debug:
+            print(str)
+
+    def insert_entities_text(self, text, entities):
+        for entity in entities:
+            entity['text'] = text[entity['start'] : entity['end']]
+        return entities
+
+    def check_duplicate_entities(self, entities):
+        entities_start = list()
+        new_entities = list()
+        entities = sorted(entities, key=lambda entity: entity['start'])
+        for entity in entities:
+            if entity['start'] not in entities_start:
+                entities_start.append(entity['start'])
+                new_entities.append(entity)
+        return new_entities
+
+    ## called by Rasa on events
+    def publish(self, event):
+        try:
+            if event['event'] == 'user':
+                text = event['text']
+                new_text = text
+                event['parse_data']['entities'] = self.insert_entities_text(
+                    text, event['parse_data']['entities']
+                )
+                entities = self.check_duplicate_entities(
+                    event['parse_data']['entities']
+                )
+                event['handled'] = (
+                    event['parse_data']['intent']['name'] != 'nlu_fallback'
+                )
+                for entity in entities:
+                    dict_entity = {
+                        'entity': entity['entity'],
+                        'value': entity['value'],
+                    }
+                    new_text = new_text.replace(
+                        entity['text'],
+                        f"[{entity['text']}]{json.dumps(dict_entity)}",
+                        1,
+                    )
+                event['text'] = new_text
+            if event['event'] in ['session_started', 'user', 'bot']:
+                self.add_to_queue(event)
+        except:
+            print('Failed to add event to queue')
+
+    def add_to_queue(self, event):
+        self.events_count += 1
+        self.queue.append(event)
+        if len(self.queue) >= self.max_queue_size:
+            self.create_flush_task()
+
+    async def flush(self, events):
+        self.requests_count += 1
+        count = self.requests_count
+        for retry in range(self.max_retries + 1):
+            try:
+                url = f'{self.api_url}/'
+                params = {'apiKey': self.api_key, 'platform': 'rasa'}
+                async with self._http_client.post(
+                    url, params=params, json=events
+                ) as request:
+                    await request.read()
+                    if request.status == 201:
+                        self.send_events_count += len(events)
+                        self.debug(
+                            f'{count} Sent {len(events)} events to Hecho after {retry} retries!'
+                        )
+                        return
+                    elif retry == self.max_retries:
+                        print(
+                            f'Failed sending {len(events)} events to Hecho after {retry} retries with status code:{request.status}'
+                        )
+                        return
+                    self.debug(
+                        f'Failed sending {len(events)} events to Hecho after {retry} retries with status code:{request.status}, retrying...'
+                    )
+            except RuntimeError as e:
+                if retry == self.max_retries:
+                    print(
+                        f'RuntimeError: Failed to send events to Hecho after {retry} retries',
+                        e,
+                    )
+            except Exception as e:
+                if retry == self.max_retries:
+                    print(
+                        f'Exception: Failed to send events to Hecho after {retry} retries: {e.message}'
+                    )
+
+    def create_flush_task(self):
+        if len(self.queue) <= 0:
+            return
+        events = self.queue
+        self.queue = list()
+        self.loop.create_task(self.flush(events))
+
+    async def start_loop(self):
+        try:
+            while True:
+                await asyncio.sleep(self.send_interval)
+                self.create_flush_task()
+        except:
+            self.debug('Exiting Hecho Events Broker...')
+
+    ## called by Rasa on close bot
+    async def close(self):
+        self.task.cancel()
+        self.create_flush_task()
+
+    def _shutdown(self):
+        asyncio.run(self._http_client.close())
+
+    @classmethod
+    async def from_endpoint_config(cls, broker_config):
+        if broker_config is None:
+            return None
+        return cls(**broker_config.kwargs)
```

