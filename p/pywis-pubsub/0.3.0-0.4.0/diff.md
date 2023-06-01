# Comparing `tmp/pywis-pubsub-0.3.0.tar.gz` & `tmp/pywis-pubsub-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pywis-pubsub-0.3.0.tar", last modified: Sun Mar 12 22:40:21 2023, max compression
+gzip compressed data, was "dist/pywis-pubsub-0.4.0.tar", last modified: Thu Jun  1 10:44:17 2023, max compression
```

## Comparing `pywis-pubsub-0.3.0.tar` & `pywis-pubsub-0.4.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2023-03-12 22:40:21.000000 pywis-pubsub-0.3.0/
--rw-rw-r--   0 tomkralidis   (501) staff       (20)    11357 2022-10-11 15:29:10.000000 pywis-pubsub-0.3.0/LICENSE
--rw-rw-r--   0 tomkralidis   (501) staff       (20)       43 2022-11-11 18:07:23.000000 pywis-pubsub-0.3.0/MANIFEST.in
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     7213 2023-03-12 22:40:21.000000 pywis-pubsub-0.3.0/PKG-INFO
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     4888 2023-03-12 22:39:40.000000 pywis-pubsub-0.3.0/README.md
-drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2023-03-12 22:40:21.000000 pywis-pubsub-0.3.0/pywis_pubsub/
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     1390 2023-03-12 22:38:51.000000 pywis-pubsub-0.3.0/pywis_pubsub/__init__.py
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     1675 2023-02-06 11:11:15.000000 pywis-pubsub-0.3.0/pywis_pubsub/cli_options.py
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     1680 2022-11-15 22:54:12.000000 pywis-pubsub-0.3.0/pywis_pubsub/geometry.py
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     1898 2023-02-06 11:11:15.000000 pywis-pubsub-0.3.0/pywis_pubsub/hook.py
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     4652 2023-02-16 11:39:56.000000 pywis-pubsub-0.3.0/pywis_pubsub/mqtt.py
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     6290 2023-02-17 21:37:16.000000 pywis-pubsub-0.3.0/pywis_pubsub/publish.py
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     2161 2022-12-15 11:45:09.000000 pywis-pubsub-0.3.0/pywis_pubsub/schema.py
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     2521 2023-02-05 23:24:11.000000 pywis-pubsub-0.3.0/pywis_pubsub/storage.py
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     7651 2023-03-12 22:35:45.000000 pywis-pubsub-0.3.0/pywis_pubsub/subscribe.py
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     4328 2023-02-24 09:58:51.000000 pywis-pubsub-0.3.0/pywis_pubsub/util.py
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     2579 2023-02-16 11:27:12.000000 pywis-pubsub-0.3.0/pywis_pubsub/validation.py
-drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2023-03-12 22:40:21.000000 pywis-pubsub-0.3.0/pywis_pubsub.egg-info/
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     7213 2023-03-12 22:40:21.000000 pywis-pubsub-0.3.0/pywis_pubsub.egg-info/PKG-INFO
--rw-rw-r--   0 tomkralidis   (501) staff       (20)      538 2023-03-12 22:40:21.000000 pywis-pubsub-0.3.0/pywis_pubsub.egg-info/SOURCES.txt
--rw-rw-r--   0 tomkralidis   (501) staff       (20)        1 2023-03-12 22:40:21.000000 pywis-pubsub-0.3.0/pywis_pubsub.egg-info/dependency_links.txt
--rw-rw-r--   0 tomkralidis   (501) staff       (20)       51 2023-03-12 22:40:21.000000 pywis-pubsub-0.3.0/pywis_pubsub.egg-info/entry_points.txt
--rw-rw-r--   0 tomkralidis   (501) staff       (20)       59 2023-03-12 22:40:21.000000 pywis-pubsub-0.3.0/pywis_pubsub.egg-info/requires.txt
--rw-rw-r--   0 tomkralidis   (501) staff       (20)       13 2023-03-12 22:40:21.000000 pywis-pubsub-0.3.0/pywis_pubsub.egg-info/top_level.txt
--rw-rw-r--   0 tomkralidis   (501) staff       (20)       59 2022-12-15 11:45:09.000000 pywis-pubsub-0.3.0/requirements.txt
--rw-rw-r--   0 tomkralidis   (501) staff       (20)       38 2023-03-12 22:40:21.000000 pywis-pubsub-0.3.0/setup.cfg
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     3327 2023-02-07 17:12:51.000000 pywis-pubsub-0.3.0/setup.py
+drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2023-06-01 10:44:17.000000 pywis-pubsub-0.4.0/
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)    11357 2022-10-11 15:29:10.000000 pywis-pubsub-0.4.0/LICENSE
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)       43 2022-11-11 18:07:23.000000 pywis-pubsub-0.4.0/MANIFEST.in
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     7208 2023-06-01 10:44:17.000000 pywis-pubsub-0.4.0/PKG-INFO
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     4883 2023-05-23 21:42:52.000000 pywis-pubsub-0.4.0/README.md
+drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2023-06-01 10:44:17.000000 pywis-pubsub-0.4.0/pywis_pubsub/
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     1390 2023-06-01 10:43:13.000000 pywis-pubsub-0.4.0/pywis_pubsub/__init__.py
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     1675 2023-02-06 11:11:15.000000 pywis-pubsub-0.4.0/pywis_pubsub/cli_options.py
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     1680 2022-11-15 22:54:12.000000 pywis-pubsub-0.4.0/pywis_pubsub/geometry.py
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     1898 2023-02-06 11:11:15.000000 pywis-pubsub-0.4.0/pywis_pubsub/hook.py
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     4652 2023-05-23 21:42:52.000000 pywis-pubsub-0.4.0/pywis_pubsub/mqtt.py
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     6405 2023-03-16 14:37:41.000000 pywis-pubsub-0.4.0/pywis_pubsub/publish.py
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     2175 2023-06-01 10:42:47.000000 pywis-pubsub-0.4.0/pywis_pubsub/schema.py
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     2521 2023-05-23 21:42:52.000000 pywis-pubsub-0.4.0/pywis_pubsub/storage.py
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     8094 2023-05-23 21:42:52.000000 pywis-pubsub-0.4.0/pywis_pubsub/subscribe.py
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     4328 2023-02-24 09:58:51.000000 pywis-pubsub-0.4.0/pywis_pubsub/util.py
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     2539 2023-06-01 10:42:47.000000 pywis-pubsub-0.4.0/pywis_pubsub/validation.py
+drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2023-06-01 10:44:17.000000 pywis-pubsub-0.4.0/pywis_pubsub.egg-info/
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     7208 2023-06-01 10:44:17.000000 pywis-pubsub-0.4.0/pywis_pubsub.egg-info/PKG-INFO
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)      538 2023-06-01 10:44:17.000000 pywis-pubsub-0.4.0/pywis_pubsub.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)        1 2023-06-01 10:44:17.000000 pywis-pubsub-0.4.0/pywis_pubsub.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)       51 2023-06-01 10:44:17.000000 pywis-pubsub-0.4.0/pywis_pubsub.egg-info/entry_points.txt
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)       69 2023-06-01 10:44:17.000000 pywis-pubsub-0.4.0/pywis_pubsub.egg-info/requires.txt
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)       13 2023-06-01 10:44:17.000000 pywis-pubsub-0.4.0/pywis_pubsub.egg-info/top_level.txt
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)       69 2023-05-23 21:42:52.000000 pywis-pubsub-0.4.0/requirements.txt
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)       38 2023-06-01 10:44:17.000000 pywis-pubsub-0.4.0/setup.cfg
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     3327 2023-02-07 17:12:51.000000 pywis-pubsub-0.4.0/setup.py
```

### Comparing `pywis-pubsub-0.3.0/LICENSE` & `pywis-pubsub-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pywis-pubsub-0.3.0/PKG-INFO` & `pywis-pubsub-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywis-pubsub
-Version: 0.3.0
+Version: 0.4.0
 Summary: pywis-pubsub provides subscription and download capability of WMO data from WIS2 infrastructure services
 Home-page: https://github.com/wmo-im/pywis-pubsub
 Author: Antje Schremmer
 Author-email: antje.schremmer@dwd.de
 Maintainer: Tom Kralidis
 Maintainer-email: tomkraldis@gmail.com
 License: Apache Software License
@@ -141,15 +141,15 @@
                 url='http://www.meteo.xx/stationXYZ-20221111085500.bufr4', 
                 identifier='stationXYZ-20221111085500', 
                 geometry=[33.8, -11.8, 123],
                 wigos_station_identifier='0-20000-12345'
         )
         
         m = MQTTPubSubClient('mqtt://localhost:1883')
-        client.pub(topic, json.dumps(message))
+        m.pub(topic, json.dumps(message))
         ```
         
         ## Development
         
         ### Running Tests
         
         ```bash
```

### Comparing `pywis-pubsub-0.3.0/README.md` & `pywis-pubsub-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         url='http://www.meteo.xx/stationXYZ-20221111085500.bufr4', 
         identifier='stationXYZ-20221111085500', 
         geometry=[33.8, -11.8, 123],
         wigos_station_identifier='0-20000-12345'
 )
 
 m = MQTTPubSubClient('mqtt://localhost:1883')
-client.pub(topic, json.dumps(message))
+m.pub(topic, json.dumps(message))
 ```
 
 ## Development
 
 ### Running Tests
 
 ```bash
```

### Comparing `pywis-pubsub-0.3.0/pywis_pubsub/__init__.py` & `pywis-pubsub-0.4.0/pywis_pubsub/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
 ###############################################################################
 
-__version__ = '0.3.0'
+__version__ = '0.4.0'
 
 import click
 
 from pywis_pubsub.publish import publish
 from pywis_pubsub.schema import schema
 from pywis_pubsub.subscribe import subscribe
 from pywis_pubsub.validation import message
```

### Comparing `pywis-pubsub-0.3.0/pywis_pubsub/cli_options.py` & `pywis-pubsub-0.4.0/pywis_pubsub/cli_options.py`

 * *Files identical despite different names*

### Comparing `pywis-pubsub-0.3.0/pywis_pubsub/geometry.py` & `pywis-pubsub-0.4.0/pywis_pubsub/geometry.py`

 * *Files identical despite different names*

### Comparing `pywis-pubsub-0.3.0/pywis_pubsub/hook.py` & `pywis-pubsub-0.4.0/pywis_pubsub/hook.py`

 * *Files identical despite different names*

### Comparing `pywis-pubsub-0.3.0/pywis_pubsub/mqtt.py` & `pywis-pubsub-0.4.0/pywis_pubsub/mqtt.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
 ###############################################################################
 
+from copy import deepcopy
 import logging
 import random
 from typing import Any, Callable
-
-from copy import deepcopy
 from urllib.parse import urlparse
+
 from paho.mqtt import client as mqtt_client
 from pywis_pubsub import util
 
 LOGGER = logging.getLogger(__name__)
 
 
 class MQTTPubSubClient:
```

### Comparing `pywis-pubsub-0.3.0/pywis_pubsub/publish.py` & `pywis-pubsub-0.4.0/pywis_pubsub/publish.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,24 +35,28 @@
 from pywis_pubsub.validation import validate_
 
 
 LOGGER = logging.getLogger(__name__)
 
 
 class SecureHashAlgorithms(Enum):
-    SHA512 = 'sha512'
-    MD5 = 'md5'
+    sha256 = 'sha256'
+    sha384 = 'sha_384'
+    sha512 = 'sha512'
+    sha3_256 = 'sha3_256'
+    sha3_384 = 'sha3_384'
+    sha3_512 = 'sha3_512'
 
 
 def generate_checksum(data: bytes, algorithm: SecureHashAlgorithms) -> str:
     """
     Generate a checksum of message file
 
     :param data: bytes of data
-    :param algorithm: secure hash algorithm (md5, sha512)
+    :param algorithm: secure hash algorithm (SecureHashAlgorithm)
 
     :returns: hexdigest
     """
 
     sh = getattr(hashlib, algorithm)()
     sh.update(data)
 
@@ -71,15 +75,15 @@
     """
 
     res = requests.get(public_data_url)
     # raise HTTPError, if on occurred:
     res.raise_for_status()
 
     filebytes = res.content
-    checksum_type = SecureHashAlgorithms.SHA512.value
+    checksum_type = SecureHashAlgorithms.sha512.value
     return {
         'filename': public_data_url.split('/')[-1],
         'checksum_value': generate_checksum(filebytes, checksum_type),
         'checksum_type': checksum_type,
         'size': len(filebytes)
     }
```

### Comparing `pywis-pubsub-0.3.0/pywis_pubsub/schema.py` & `pywis-pubsub-0.4.0/pywis_pubsub/schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 import shutil
 from urllib.request import urlopen
 
 from pywis_pubsub import cli_options
 
 LOGGER = logging.getLogger(__name__)
 
-MESSAGE_SCHEMA_URL = 'https://raw.githubusercontent.com/wmo-im/wis2-notification-message/main/schemas/notificationMessageGeoJSON.yaml'  # noqa
+MESSAGE_SCHEMA_URL = 'https://raw.githubusercontent.com/wmo-im/wis2-notification-message/main/schemas/wis2-notification-message-bundled.json'  # noqa
 USERDIR = Path.home() / '.pywis-pubsub'
-MESSAGE_SCHEMA = USERDIR / 'wis2-notification-message' / 'WIS2_Message_Format_Schema.yaml'  # noqa
+MESSAGE_SCHEMA = USERDIR / 'wis2-notification-message' / 'wis2-notification-message-bundled.json'  # noqa
 
 
 def sync_schema() -> None:
     """
     Sync WIS2 notification schema
 
     :returns: `None`
```

### Comparing `pywis-pubsub-0.3.0/pywis_pubsub/storage.py` & `pywis-pubsub-0.4.0/pywis_pubsub/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         LOGGER.debug(f'Creating directory {filepath.parent}')
         filepath.parent.mkdir(parents=True, exist_ok=True)
 
         LOGGER.debug(f'Saving data to {filepath}')
         with filepath.open('wb') as fh:
             fh.write(data)
 
-        LOGGER.info(f'Data saved to {filename}')
+        LOGGER.info(f'Data saved to {filepath}')
 
         return True
 
 
 class S3(Storage):
     def save(self, data: bytes, filename: Path) -> bool:
```

### Comparing `pywis-pubsub-0.3.0/pywis_pubsub/subscribe.py` & `pywis-pubsub-0.4.0/pywis_pubsub/subscribe.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 ###############################################################################
 
 import base64
 import enum
 import hashlib
 import json
 import logging
-from pathlib import Path
 
 import click
 from requests import Session
 from requests.adapters import HTTPAdapter, Retry
 
 from pywis_pubsub import cli_options
 from pywis_pubsub import util
@@ -39,16 +38,20 @@
 from pywis_pubsub.validation import validate_message
 
 
 LOGGER = logging.getLogger(__name__)
 
 
 class VerificationMethods(enum.Enum):
-    md5 = 'md5'
+    sha256 = 'sha256'
+    sha384 = 'sha_384'
     sha512 = 'sha512'
+    sha3_256 = 'sha3_256'
+    sha3_384 = 'sha3_384'
+    sha3_512 = 'sha3_512'
 
 
 def get_canonical_link(links: list):
     """
     Helper function to derive canonical link from a list of link objects
 
     :param links: `list` of link `dict`s
@@ -59,36 +62,40 @@
     try:
         return list(filter(lambda d: d['rel'] == 'canonical', links))[0]
     except IndexError:
         LOGGER.error('No canonical link found')
         return {}
 
 
-def get_data(msg_dict: dict) -> bytes:
+def get_data(msg_dict: dict, verify_certs=True) -> bytes:
     """
     Data downloading functionality
 
     :param msg_dict: `dict` of notification message
+    :param verify_certs: `bool` of whether to verify
+                         certificates (default true)
 
     :returns: `bytes` of data
     """
 
     canonical_link = get_canonical_link(msg_dict['links'])
 
     if canonical_link:
         LOGGER.debug(f'Found canonical link: {canonical_link}')
 
     if 'content' in msg_dict and 'value' in msg_dict['content']:
         LOGGER.debug('Decoding from inline data')
         data = base64.b64decode(msg_dict['content']['value'])
     else:
         LOGGER.debug(f"Downloading from {canonical_link['href']}")
+        LOGGER.debug(f'Certificate verification: {verify_certs}')
         http_session = get_http_session()
         try:
-            data = http_session.get(canonical_link['href']).content
+            data = http_session.get(canonical_link['href'],
+                                    verify=verify_certs).content
         except Exception as err:
             LOGGER.error(f"download error ({canonical_link['href']}): {err}")
             raise
 
     return data
 
 
@@ -164,15 +171,15 @@
     clink = get_canonical_link(msg_dict['links'])
     LOGGER.info(f"Received message with data-url {clink['href']}")
 
     if userdata.get('storage') is not None:
         LOGGER.debug('Saving data')
         try:
             LOGGER.debug('Downloading data')
-            data = get_data(msg_dict)
+            data = get_data(msg_dict, userdata.get('verify_certs'))
         except Exception as err:
             LOGGER.error(err)
             return
         if ('integrity' in msg_dict['properties'] and
                 userdata.get('verify_data', True)):
             LOGGER.debug('Verifying data')
 
@@ -185,16 +192,15 @@
 
             if not data_verified(data, size, method, value):
                 LOGGER.error('Data verification failed; not saving')
                 return
             else:
                 LOGGER.debug('Data verification passed')
 
-        link = Path(clink['href'])
-        filename = link.name
+        filename = msg_dict['properties']['data_id']
 
         storage_class = STORAGES[userdata.get('storage').get('type')]
         storage_object = storage_class(userdata['storage'])
         storage_object.save(data, filename)
 
     if userdata.get('hook') is not None:
         LOGGER.debug(f"Hook detected: {userdata['hook']}")
@@ -219,16 +225,19 @@
     if config is None:
         raise click.ClickException('missing --config')
     config = util.yaml_load(config)
 
     broker = config.get('broker')
     qos = int(config.get('qos', 1))
     subscribe_topics = config.get('subscribe_topics', [])
+    verify_certs = config.get('verify_certs', True)
 
-    options = {}
+    options = {
+        'verify_certs': verify_certs
+    }
 
     if bbox:
         options['bbox'] = [float(i) for i in bbox.split(',')]
 
     if download:
         options['storage'] = config['storage']
```

### Comparing `pywis-pubsub-0.3.0/pywis_pubsub/util.py` & `pywis-pubsub-0.4.0/pywis_pubsub/util.py`

 * *Files identical despite different names*

### Comparing `pywis-pubsub-0.3.0/pywis_pubsub/validation.py` & `pywis-pubsub-0.4.0/pywis_pubsub/validation.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 from typing import Tuple
 
 import click
 from jsonschema import validate
 
 from pywis_pubsub import cli_options
 from pywis_pubsub.schema import MESSAGE_SCHEMA
-from pywis_pubsub.util import yaml_load
 
 LOGGER = logging.getLogger(__name__)
 
 
 @click.group()
 def message():
     """Message utilities"""
@@ -54,15 +53,15 @@
 
     if not MESSAGE_SCHEMA.exists():
         msg = 'Schema not found. Please run pywis-pubsub schema sync'
         LOGGER.error(msg)
         raise RuntimeError(msg)
 
     with open(MESSAGE_SCHEMA) as fh:
-        schema = yaml_load(fh)
+        schema = json.load(fh)
 
     try:
         validate(instance, schema)
         success = True
     except Exception as err:
         error_message = repr(err)
```

### Comparing `pywis-pubsub-0.3.0/pywis_pubsub.egg-info/PKG-INFO` & `pywis-pubsub-0.4.0/pywis_pubsub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywis-pubsub
-Version: 0.3.0
+Version: 0.4.0
 Summary: pywis-pubsub provides subscription and download capability of WMO data from WIS2 infrastructure services
 Home-page: https://github.com/wmo-im/pywis-pubsub
 Author: Antje Schremmer
 Author-email: antje.schremmer@dwd.de
 Maintainer: Tom Kralidis
 Maintainer-email: tomkraldis@gmail.com
 License: Apache Software License
@@ -141,15 +141,15 @@
                 url='http://www.meteo.xx/stationXYZ-20221111085500.bufr4', 
                 identifier='stationXYZ-20221111085500', 
                 geometry=[33.8, -11.8, 123],
                 wigos_station_identifier='0-20000-12345'
         )
         
         m = MQTTPubSubClient('mqtt://localhost:1883')
-        client.pub(topic, json.dumps(message))
+        m.pub(topic, json.dumps(message))
         ```
         
         ## Development
         
         ### Running Tests
         
         ```bash
```

### Comparing `pywis-pubsub-0.3.0/pywis_pubsub.egg-info/SOURCES.txt` & `pywis-pubsub-0.4.0/pywis_pubsub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywis-pubsub-0.3.0/setup.py` & `pywis-pubsub-0.4.0/setup.py`

 * *Files identical despite different names*

