# Comparing `tmp/hass_mqtt_things-0.5.4.tar.gz` & `tmp/hass_mqtt_things-0.5.5.tar.gz`

## Comparing `hass_mqtt_things-0.5.4.tar` & `hass_mqtt_things-0.5.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.4/.flake8
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.4/src/ham/__init__.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.4/src/ham/binary_sensor.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.4/src/ham/button.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.4/src/ham/light.py
--rw-r--r--   0        0        0     8191 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.4/src/ham/manager.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.4/src/ham/number.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.4/src/ham/sensor.py
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.4/src/ham/switch.py
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.4/src/ham/things.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.4/src/ham/utils.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.4/LICENSE
--rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.4/README.md
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/.flake8
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/src/ham/__init__.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/src/ham/binary_sensor.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/src/ham/button.py
+-rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/src/ham/fan.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/src/ham/light.py
+-rw-r--r--   0        0        0     8283 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/src/ham/manager.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/src/ham/number.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/src/ham/sensor.py
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/src/ham/switch.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/src/ham/things.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/src/ham/utils.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/LICENSE
+-rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/README.md
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/PKG-INFO
```

### Comparing `hass_mqtt_things-0.5.4/src/ham/binary_sensor.py` & `hass_mqtt_things-0.5.5/src/ham/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hass_mqtt_things-0.5.4/src/ham/button.py` & `hass_mqtt_things-0.5.5/src/ham/button.py`

 * *Files identical despite different names*

### Comparing `hass_mqtt_things-0.5.4/src/ham/light.py` & `hass_mqtt_things-0.5.5/src/ham/light.py`

 * *Files identical despite different names*

### Comparing `hass_mqtt_things-0.5.4/src/ham/manager.py` & `hass_mqtt_things-0.5.5/src/ham/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,14 +165,15 @@
     def availability_topic(self):
         return f"{ self.base_topic }/availability"
 
     @property
     def subscribe_topic(self):
         return [
             (f"{ self.base_topic }/+/set", 0),  # Most things use `set`
+            (f"{ self.base_topic }/+/+/set", 0),  # Some things are nested (at least: fans)
             (f"{ self.base_topic }/+/press", 0),  # Buttons use `press`
         ]
 
     def on_connect(self, _, userdata, flags, rc):
         logger.info("Connected with result code %d", rc)
 
         # Subscribing in on_connect() means that if we lose the connection and
```

### Comparing `hass_mqtt_things-0.5.4/src/ham/number.py` & `hass_mqtt_things-0.5.5/src/ham/number.py`

 * *Files identical despite different names*

### Comparing `hass_mqtt_things-0.5.4/src/ham/sensor.py` & `hass_mqtt_things-0.5.5/src/ham/sensor.py`

 * *Files identical despite different names*

### Comparing `hass_mqtt_things-0.5.4/src/ham/switch.py` & `hass_mqtt_things-0.5.5/src/ham/switch.py`

 * *Files identical despite different names*

### Comparing `hass_mqtt_things-0.5.4/src/ham/things.py` & `hass_mqtt_things-0.5.5/src/ham/things.py`

 * *Files identical despite different names*

### Comparing `hass_mqtt_things-0.5.4/.gitignore` & `hass_mqtt_things-0.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `hass_mqtt_things-0.5.4/LICENSE` & `hass_mqtt_things-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hass_mqtt_things-0.5.4/README.md` & `hass_mqtt_things-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `hass_mqtt_things-0.5.4/pyproject.toml` & `hass_mqtt_things-0.5.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hass_mqtt_things-0.5.4/PKG-INFO` & `hass_mqtt_things-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hass-mqtt-things
-Version: 0.5.4
+Version: 0.5.5
 Summary: Library for rapid development of things to be integrated with Home Assistant through MQTT
 Project-URL: Documentation, https://github.com/alexbarcelo/hass-mqtt-things#readme
 Project-URL: Issues, https://github.com/alexbarcelo/hass-mqtt-things/issues
 Project-URL: Source, https://github.com/alexbarcelo/hass-mqtt-things
 Author-email: Alex Barcelo <alex@betarho.net>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

