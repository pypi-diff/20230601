# Comparing `tmp/redreactor-0.1.0.tar.gz` & `tmp/redreactor-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redreactor-0.1.0.tar", max compression
+gzip compressed data, was "redreactor-0.1.1.tar", max compression
```

## Comparing `redreactor-0.1.0.tar` & `redreactor-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1067 2023-05-23 17:08:35.624665 redreactor-0.1.0/LICENSE
--rw-r--r--   0        0        0     3409 2023-05-23 17:08:35.624665 redreactor-0.1.0/README.md
--rw-r--r--   0        0        0     3199 2023-05-23 17:08:57.428958 redreactor-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       60 2023-05-23 17:08:35.624665 redreactor-0.1.0/src/redreactor/__init__.py
--rw-r--r--   0        0        0     3997 2023-05-23 17:08:35.624665 redreactor-0.1.0/src/redreactor/__main__.py
--rw-r--r--   0        0        0       97 2023-05-23 17:08:35.624665 redreactor-0.1.0/src/redreactor/components/commander/__init__.py
--rw-r--r--   0        0        0     6688 2023-05-23 17:08:35.624665 redreactor-0.1.0/src/redreactor/components/commander/commander.py
--rw-r--r--   0        0        0      121 2023-05-23 17:08:35.624665 redreactor-0.1.0/src/redreactor/components/homeassistant/__init__.py
--rw-r--r--   0        0        0      526 2023-05-23 17:08:35.624665 redreactor-0.1.0/src/redreactor/components/homeassistant/binary_sensor.py
--rw-r--r--   0        0        0      646 2023-05-23 17:08:35.624665 redreactor-0.1.0/src/redreactor/components/homeassistant/button.py
--rw-r--r--   0        0        0     4954 2023-05-23 17:08:35.624665 redreactor-0.1.0/src/redreactor/components/homeassistant/common.py
--rw-r--r--   0        0        0     7744 2023-05-23 17:08:35.624665 redreactor-0.1.0/src/redreactor/components/homeassistant/homeassistant.py
--rw-r--r--   0        0        0     1224 2023-05-23 17:08:35.624665 redreactor-0.1.0/src/redreactor/components/homeassistant/number.py
--rw-r--r--   0        0        0      707 2023-05-23 17:08:35.624665 redreactor-0.1.0/src/redreactor/components/homeassistant/sensor.py
--rw-r--r--   0        0        0       99 2023-05-23 17:08:35.624665 redreactor-0.1.0/src/redreactor/components/monitor/__init__.py
--rw-r--r--   0        0        0     1601 2023-05-23 17:08:35.624665 redreactor-0.1.0/src/redreactor/components/monitor/data.py
--rw-r--r--   0        0        0    12761 2023-05-23 17:08:35.624665 redreactor-0.1.0/src/redreactor/components/monitor/monitor.py
--rw-r--r--   0        0        0       84 2023-05-23 17:08:35.624665 redreactor-0.1.0/src/redreactor/components/mqtt/__init__.py
--rw-r--r--   0        0        0     6086 2023-05-23 17:08:35.624665 redreactor-0.1.0/src/redreactor/components/mqtt/mqtt.py
--rw-r--r--   0        0        0     8497 2023-05-23 17:08:35.624665 redreactor-0.1.0/src/redreactor/configuration.py
--rw-r--r--   0        0        0      708 2023-05-23 17:08:35.624665 redreactor-0.1.0/src/redreactor/const.py
--rw-r--r--   0        0        0       37 2023-05-23 17:08:35.624665 redreactor-0.1.0/src/redreactor/helpers/__init__.py
--rw-r--r--   0        0        0      902 2023-05-23 17:08:35.624665 redreactor-0.1.0/src/redreactor/helpers/emitter.py
--rw-r--r--   0        0        0     1116 2023-05-23 17:08:35.624665 redreactor-0.1.0/src/redreactor/helpers/repeater.py
--rw-r--r--   0        0        0      685 2023-05-23 17:08:35.624665 redreactor-0.1.0/src/redreactor/helpers/utils.py
--rw-r--r--   0        0        0     4342 1970-01-01 00:00:00.000000 redreactor-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-01 08:17:19.223168 redreactor-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3409 2023-06-01 08:17:19.223168 redreactor-0.1.1/README.md
+-rw-r--r--   0        0        0     3199 2023-06-01 08:17:33.679257 redreactor-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       60 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/__init__.py
+-rw-r--r--   0        0        0     3997 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/__main__.py
+-rw-r--r--   0        0        0       97 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/components/commander/__init__.py
+-rw-r--r--   0        0        0     6734 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/components/commander/commander.py
+-rw-r--r--   0        0        0      121 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/components/homeassistant/__init__.py
+-rw-r--r--   0        0        0      526 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/components/homeassistant/binary_sensor.py
+-rw-r--r--   0        0        0      646 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/components/homeassistant/button.py
+-rw-r--r--   0        0        0     4954 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/components/homeassistant/common.py
+-rw-r--r--   0        0        0     7744 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/components/homeassistant/homeassistant.py
+-rw-r--r--   0        0        0     1224 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/components/homeassistant/number.py
+-rw-r--r--   0        0        0      707 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/components/homeassistant/sensor.py
+-rw-r--r--   0        0        0       99 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/components/monitor/__init__.py
+-rw-r--r--   0        0        0     1601 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/components/monitor/data.py
+-rw-r--r--   0        0        0    12761 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/components/monitor/monitor.py
+-rw-r--r--   0        0        0       84 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/components/mqtt/__init__.py
+-rw-r--r--   0        0        0     6086 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/components/mqtt/mqtt.py
+-rw-r--r--   0        0        0     8497 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/configuration.py
+-rw-r--r--   0        0        0      708 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/const.py
+-rw-r--r--   0        0        0       37 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/helpers/__init__.py
+-rw-r--r--   0        0        0      902 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/helpers/emitter.py
+-rw-r--r--   0        0        0     1116 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/helpers/repeater.py
+-rw-r--r--   0        0        0      685 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/helpers/utils.py
+-rw-r--r--   0        0        0     4342 1970-01-01 00:00:00.000000 redreactor-0.1.1/PKG-INFO
```

### Comparing `redreactor-0.1.0/LICENSE` & `redreactor-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.0/README.md` & `redreactor-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.0/pyproject.toml` & `redreactor-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redreactor"
-version = "0.1.0"
+version = "0.1.1"
 description = "Red Reactor Battery Monitoring service with MQTT, and Home Assistant support"
 documentation = "https://github.com/mreditor97/redreactor"
 repository = "https://github.com/mreditor97/redreactor"
 homepage = "https://github.com/mreditor97/redreactor"
 authors = ["MrEditor97 <dev@mreditor97.co.uk>"]
 license = "MIT"
 readme = "README.md"
@@ -24,23 +24,23 @@
 
 [tool.poetry.dev-dependencies]
 aresponses = "2.1.6"
 black = "23.3.0"
 blacken-docs = "1.13.0"
 codespell = "2.2.4"
 covdefaults = "2.3.0"
-coverage = {version = "7.2.5", extras = ["toml"]}
+coverage = {version = "7.2.7", extras = ["toml"]}
 mypy = "1.3.0"
 pre-commit = "3.3.2"
 pre-commit-hooks = "4.4.0"
 pylint = "2.17.4"
 pytest = "7.3.1"
 pytest-asyncio = "0.21.0"
-pytest-cov = "4.0.0"
-ruff = "0.0.269"
+pytest-cov = "4.1.0"
+ruff = "0.0.270"
 safety = "2.4.0b1"
 types-cachetools = "^5.3.0"
 yamllint = "1.32.0"
 types-pyyaml = "^6.0.12.10"
 
 [tool.coverage.run]
 plugins = ["covdefaults"]
```

### Comparing `redreactor-0.1.0/src/redreactor/__main__.py` & `redreactor-0.1.1/src/redreactor/__main__.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.0/src/redreactor/components/commander/commander.py` & `redreactor-0.1.1/src/redreactor/components/commander/commander.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,19 +63,19 @@
             # Only process fields that are of type button or number
             if self._static_configuration["fields"][field]["type"] in {
                 "number",
                 "button",
             }:
                 self.logger.info(
                     "Subscribing to the %s topic at: %s/%s/%s/%s",
-                    field,
+                    self._static_configuration["fields"][field]["pretty"],
                     self._static_configuration["mqtt"]["base_topic"],
                     self._static_configuration["hostname"]["name"],
                     self._static_configuration["mqtt"]["topic"]["set"],
-                    self._static_configuration["fields"][field]["pretty"],
+                    self._static_configuration["fields"][field]["name"],
                 )
 
                 # Subscribe to that specific topic
                 client.subscribe(
                     topic=f"{self._static_configuration['mqtt']['base_topic']}/{self._static_configuration['hostname']['name']}/{self._static_configuration['mqtt']['topic']['set']}/{self._static_configuration['fields'][field]['name']}",
                 )
```

### Comparing `redreactor-0.1.0/src/redreactor/components/homeassistant/binary_sensor.py` & `redreactor-0.1.1/src/redreactor/components/homeassistant/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.0/src/redreactor/components/homeassistant/button.py` & `redreactor-0.1.1/src/redreactor/components/homeassistant/button.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.0/src/redreactor/components/homeassistant/common.py` & `redreactor-0.1.1/src/redreactor/components/homeassistant/common.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.0/src/redreactor/components/homeassistant/homeassistant.py` & `redreactor-0.1.1/src/redreactor/components/homeassistant/homeassistant.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.0/src/redreactor/components/homeassistant/number.py` & `redreactor-0.1.1/src/redreactor/components/homeassistant/number.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.0/src/redreactor/components/homeassistant/sensor.py` & `redreactor-0.1.1/src/redreactor/components/homeassistant/sensor.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.0/src/redreactor/components/monitor/data.py` & `redreactor-0.1.1/src/redreactor/components/monitor/data.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.0/src/redreactor/components/monitor/monitor.py` & `redreactor-0.1.1/src/redreactor/components/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.0/src/redreactor/components/mqtt/mqtt.py` & `redreactor-0.1.1/src/redreactor/components/mqtt/mqtt.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.0/src/redreactor/configuration.py` & `redreactor-0.1.1/src/redreactor/configuration.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.0/src/redreactor/const.py` & `redreactor-0.1.1/src/redreactor/const.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.0/src/redreactor/helpers/emitter.py` & `redreactor-0.1.1/src/redreactor/helpers/emitter.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.0/src/redreactor/helpers/repeater.py` & `redreactor-0.1.1/src/redreactor/helpers/repeater.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.0/src/redreactor/helpers/utils.py` & `redreactor-0.1.1/src/redreactor/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.0/PKG-INFO` & `redreactor-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redreactor
-Version: 0.1.0
+Version: 0.1.1
 Summary: Red Reactor Battery Monitoring service with MQTT, and Home Assistant support
 Home-page: https://github.com/mreditor97/redreactor
 License: MIT
 Author: MrEditor97
 Author-email: dev@mreditor97.co.uk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

