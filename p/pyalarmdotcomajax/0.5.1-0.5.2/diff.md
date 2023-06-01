# Comparing `tmp/pyalarmdotcomajax-0.5.1.tar.gz` & `tmp/pyalarmdotcomajax-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalarmdotcomajax-0.5.1.tar", last modified: Wed May 31 00:06:38 2023, max compression
+gzip compressed data, was "pyalarmdotcomajax-0.5.2.tar", last modified: Thu Jun  1 16:05:14 2023, max compression
```

## Comparing `pyalarmdotcomajax-0.5.1.tar` & `pyalarmdotcomajax-0.5.2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:06:38.627253 pyalarmdotcomajax-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-05-31 00:06:38.627253 pyalarmdotcomajax-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:06:38.623253 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/
--rw-r--r--   0 runner    (1001) docker     (123)    46790 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20995 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:06:38.627253 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/
--rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/garage_door.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/image_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)    14829 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/thermostat.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/water_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22829 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:06:38.627253 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:06:38.627253 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/garage_door.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/thermostat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/water_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:06:38.623253 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-05-31 00:06:38.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-31 00:06:38.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 00:06:38.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-31 00:06:38.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-31 00:06:38.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-31 00:06:38.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 00:06:38.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-31 00:06:38.631253 pyalarmdotcomajax-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:06:38.627253 pyalarmdotcomajax-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:06:38.627253 pyalarmdotcomajax-0.5.1/tests/responses/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/tests/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/tests/test_device_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/tests/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/tests/test_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/tests/test_thermostat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:05:14.499249 pyalarmdotcomajax-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-06-01 16:05:14.499249 pyalarmdotcomajax-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:05:14.491249 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/
+-rw-r--r--   0 runner    (1001) docker     (123)    46790 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20986 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:05:14.495249 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/garage_door.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/image_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14829 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/water_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22829 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:05:14.495249 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:05:14.499249 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/garage_door.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/water_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:05:14.491249 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-06-01 16:05:14.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-01 16:05:14.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 16:05:14.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 16:05:14.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-01 16:05:14.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 16:05:14.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 16:05:14.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-01 16:05:14.499249 pyalarmdotcomajax-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:05:14.499249 pyalarmdotcomajax-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:05:14.499249 pyalarmdotcomajax-0.5.2/tests/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/tests/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/tests/test_device_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/tests/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/tests/test_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/tests/test_thermostat.py
```

### Comparing `pyalarmdotcomajax-0.5.1/LICENSE` & `pyalarmdotcomajax-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/PKG-INFO` & `pyalarmdotcomajax-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalarmdotcomajax
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python Interface for Alarm.com
 Home-page: https://github.com/pyalarmdotcom/pyalarmdotcomajax
 Author: Justin Wong
 Author-email: 46082645+uvjustin@users.noreply.github.com
 Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com, 466460+elahd@users.noreply.github.com
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.1 Summary: Python
+Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.2 Summary: Python
 Interface for Alarm.com Home-page: https://github.com/pyalarmdotcom/
 pyalarmdotcomajax Author: Justin Wong Author-email:
 46082645+uvjustin@users.noreply.github.com Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com,
 466460+elahd@users.noreply.github.com License: MIT Keywords: Alarm.com,Security
 System,Home Assistant Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English Classifier: Environment :: Web
```

### Comparing `pyalarmdotcomajax-0.5.1/README.md` & `pyalarmdotcomajax-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/__init__.py` & `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     CameraSkybellControllerExtension,
     ConfigurationOption,
     ControllerExtensions_t,
     ExtendedProperties,
 )
 from pyalarmdotcomajax.websockets.client import WebSocketClient, WebSocketState
 
-__version__ = "0.5.1"
+__version__ = "0.5.2"
 
 log = logging.getLogger(__name__)
 
 
 class ExtensionResults(TypedDict):
     """Results of multi-device extension calls."""
```

### Comparing `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/cli.py` & `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,15 +405,15 @@
             cprint(
                 "Streaming real-time updates...",
                 "grey",
                 "on_yellow",
                 attrs=["bold"],
             )
             cprint(
-                "(Press Ctrl+C or Cmd+C to exit.)",
+                "(Press Ctrl+C to exit.)",
                 attrs=["bold"],
             )
 
             await _async_stream_realtime(alarm)
 
 
 #############
```

### Comparing `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/const.py` & `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/const.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/__init__.py` & `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Alarm.com device base devices."""
 from __future__ import annotations
 
+import contextlib
 import logging
 from abc import ABC
 from collections.abc import Callable
 from dataclasses import dataclass
 from enum import Enum
 from typing import Any, TypedDict
 
@@ -154,20 +155,20 @@
         """Return whether entity reports state."""
         return self._attribs_raw.get("hasState", False)
 
     @property
     def state(self) -> Enum | None:
         """Return state."""
 
-        try:
-            state = self.DeviceState(self._attribs_raw.get("state"))
-        except ValueError:
-            return None
+        # Devices that don't report state on Alarm.com still have a value in the state field.
+        if self.has_state:
+            with contextlib.suppress(ValueError):
+                return self.DeviceState(self._attribs_raw.get("state"))
 
-        return state
+        return None
 
     @property
     def settings(self) -> dict:
         """Return user-changable settings."""
 
         return {
             config_option.slug: config_option
```

### Comparing `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/garage_door.py` & `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/garage_door.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/gate.py` & `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/gate.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/image_sensor.py` & `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/image_sensor.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/light.py` & `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/light.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/lock.py` & `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/lock.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/partition.py` & `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/partition.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/registry.py` & `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/registry.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/sensor.py` & `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/sensor.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/system.py` & `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/system.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/thermostat.py` & `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/thermostat.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/exceptions.py` & `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/extensions.py` & `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/extensions.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/helpers.py` & `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/helpers.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/client.py` & `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/client.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/const.py` & `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/const.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,101 +21,112 @@
     PropertyChangeType.HeatSetPoint,
     PropertyChangeType.CoolSetPoint,
     PropertyChangeType.LightColor,
 ]
 
 
 class EventType(Enum):
-    """Enum for monitoring event types."""
+    """Enum for event types."""
 
-    #
     # Supported
-    #
     ArmedAway = 10
     ArmedNight = 113
     ArmedStay = 9
     Closed = 0
     Disarmed = 8
     DoorLocked = 91
     DoorUnlocked = 90
-    ImageSensorUpload = 99
     LightTurnedOff = 316
     LightTurnedOn = 315
     Opened = 15
     OpenedClosed = 100
-    SupervisionFaultArming = 48
-    SupervisionFaultDisarming = 47
     SwitchLevelChanged = 317
     ThermostatFanModeChanged = 120
     ThermostatModeChanged = 95
     ThermostatOffset = 105
     ThermostatSetPointChanged = 94
 
-    #
-    # Not Supported
-    #
+    # Unsupported
     Alarm = 1
-    BypassStart = 13
-    BypassEnd = 35
-    SumpPumpAlertCriticalIssueMalfunction = 118
-    SumpPumpAlertCriticalIssueOff = 117
-    SumpPumpAlertIdle = 114
-    SumpPumpAlertNormalOperation = 115
-    SumpPumpAlertPossibleIssue = 116
-    VideoCameraTriggered = 71
-    VideoEventTriggered = 76
+    AccessControlDoorAccessGranted = 298
     AlarmCancelled = 238
+    ArmingSupervisionFault = 48
     AuxiliaryPanic = 17
     AuxPanicPendingAlarm = 61
     AuxPanicSuspectedAlarm = 65
+    BadLockUserCode = 93
+    Bypassed = 13
     CommercialClosedOnTime = 127
     CommercialClosedUnexpectedly = 177
     CommercialEarlyClose = 125
     CommercialEarlyOpen = 122
     CommercialLateClose = 126
     CommercialLateOpen = 123
     CommercialOpenOnTime = 124
+    DisarmingSupervisionFault = 47
+    DoorAccessed = 92
+    DoorAccessedDoubleSwipe = 236
     DoorBuzzedFromWebsite = 182
+    DoorFailedAccess = 180
+    DoorForcedOpen = 181
+    DoorHeldOpen = 184
+    EndOfBypass = 35
+    ExitButtonPressed = 141
     FirePanic = 24
+    GoogleSdmEvent = 346
+    ImageSensorUpload = 99
     InAppAuxiliaryPanic = 201
     InAppFirePanic = 200
     InAppPolicePanic = 202
     InAppSilentPolicePanic = 203
-    MonitoringPanic = 2009
     NetworkDhcpReservationsUpdated = 433
     NetworkDhcpSettingsUpdated = 432
     NetworkMapUpdated = 391
     NetworkPortForwardingUpdated = 434
     PackageDeliveryAlert = 363
     PackageRetrievalAlert = 364
     PendingAlarm = 62
     PolicePanic = 22
     PolicePanicSuspectedAlarm = 64
+    RouterHostsUpdated = 450
+    RouterProfilesUpdated = 451
     SilentPolicePanic = 73
     SilentPolicePanicSuspectedAlarm = 172
+    SpeedTestResultsUpdated = 454
+    SumpPumpAlertCriticalIssueMalfunction = 118
+    SumpPumpAlertCriticalIssueOff = 117
+    SumpPumpAlertIdle = 114
+    SumpPumpAlertNormalOperation = 115
+    SumpPumpAlertPossibleIssue = 116
+    Tamper = 7
+    UnknownCardFormatRead = 185
+    VideoAnalytics2Detection = 302
+    VideoAnalyticsDetection = 210
+    VideoCameraTriggered = 71
+    VideoEventTriggered = 76
     ViewedByCentralStation = 158
+    WrongPinCode = 398
 
     # Undocumented
     UserLoggedIn = 55
+    DoorLeftOpenRestoral = 103  # When door is closed after being left open. Paired with a door closed event.
+    DoorLeftOpen = 101  # When door is left open for 30 minutes.
 
 
 SUPPORTED_MONITORING_EVENT_TYPES = [
     EventType.ArmedAway,
     EventType.ArmedNight,
     EventType.ArmedStay,
     EventType.Closed,
     EventType.Disarmed,
     EventType.DoorLocked,
     EventType.DoorUnlocked,
-    EventType.ImageSensorUpload,
     EventType.LightTurnedOff,
     EventType.LightTurnedOn,
     EventType.Opened,
     EventType.OpenedClosed,
-    EventType.SupervisionFaultArming,
-    EventType.SupervisionFaultDisarming,
     EventType.SwitchLevelChanged,
     EventType.ThermostatFanModeChanged,
     EventType.ThermostatModeChanged,
     EventType.ThermostatOffset,
     EventType.ThermostatSetPointChanged,
 ]
```

### Comparing `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/__init__.py` & `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/garage_door.py` & `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/garage_door.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/gate.py` & `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/gate.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/light.py` & `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/light.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/lock.py` & `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/lock.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/partition.py` & `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/partition.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/sensor.py` & `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/sensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Sensor websocket message handler."""
 
 from __future__ import annotations
 
+import asyncio
 import logging
 
 from pyalarmdotcomajax.devices.sensor import Sensor
 from pyalarmdotcomajax.websockets.const import EventType
 from pyalarmdotcomajax.websockets.handler import BaseWebSocketHandler
 from pyalarmdotcomajax.websockets.messages import (
     EventMessage,
@@ -46,17 +47,29 @@
 
         if type(message.device) != Sensor:
             return
 
         match message:
             case EventMessage():
                 match message.event_type:
-                    case EventType.Closed | EventType.Opened | EventType.OpenedClosed:
+                    case EventType.Closed | EventType.Opened:
                         state = await self.async_get_state_from_event_type(message)
                         await message.device.async_handle_external_state_change(state)
+
+                    case EventType.OpenedClosed:
+                        # Lock ensures that state changes are executed in order.
+                        lock = asyncio.Lock()
+
+                        async with lock:
+                            await message.device.async_handle_external_state_change(Sensor.DeviceState.OPEN.value)
+
+                        async with lock:
+                            await message.device.async_handle_external_state_change(
+                                Sensor.DeviceState.CLOSED.value
+                            )
                     case _:
                         log.debug(
                             f"Support for event {message.event_type} ({message.event_type_id}) not yet implemented"
                             f" by {self.SUPPORTED_DEVICE_TYPE.__name__}."
                         )
             case _:
                 log.debug(
```

### Comparing `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/thermostat.py` & `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/thermostat.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/water_sensor.py` & `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/water_sensor.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/messages.py` & `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/messages.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax.egg-info/PKG-INFO` & `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalarmdotcomajax
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python Interface for Alarm.com
 Home-page: https://github.com/pyalarmdotcom/pyalarmdotcomajax
 Author: Justin Wong
 Author-email: 46082645+uvjustin@users.noreply.github.com
 Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com, 466460+elahd@users.noreply.github.com
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.1 Summary: Python
+Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.2 Summary: Python
 Interface for Alarm.com Home-page: https://github.com/pyalarmdotcom/
 pyalarmdotcomajax Author: Justin Wong Author-email:
 46082645+uvjustin@users.noreply.github.com Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com,
 466460+elahd@users.noreply.github.com License: MIT Keywords: Alarm.com,Security
 System,Home Assistant Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English Classifier: Environment :: Web
```

### Comparing `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax.egg-info/SOURCES.txt` & `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/pyproject.toml` & `pyalarmdotcomajax-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/setup.cfg` & `pyalarmdotcomajax-0.5.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/tests/__init__.py` & `pyalarmdotcomajax-0.5.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/tests/conftest.py` & `pyalarmdotcomajax-0.5.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/tests/test_controller.py` & `pyalarmdotcomajax-0.5.2/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/tests/test_device_extensions.py` & `pyalarmdotcomajax-0.5.2/tests/test_device_extensions.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/tests/test_partition.py` & `pyalarmdotcomajax-0.5.2/tests/test_partition.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/tests/test_sensors.py` & `pyalarmdotcomajax-0.5.2/tests/test_sensors.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.1/tests/test_thermostat.py` & `pyalarmdotcomajax-0.5.2/tests/test_thermostat.py`

 * *Files identical despite different names*

