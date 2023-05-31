# Comparing `tmp/runtimepy-1.5.3.tar.gz` & `tmp/runtimepy-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runtimepy-1.5.3.tar", last modified: Fri May  5 01:04:04 2023, max compression
+gzip compressed data, was "runtimepy-1.5.4.tar", last modified: Wed May 31 22:10:17 2023, max compression
```

## Comparing `runtimepy-1.5.3.tar` & `runtimepy-1.5.4.tar`

### file list

```diff
@@ -1,137 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:04:04.522317 runtimepy-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-05 01:02:15.000000 runtimepy-1.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-05 01:04:04.522317 runtimepy-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-05 01:02:15.000000 runtimepy-1.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-05 01:02:15.000000 runtimepy-1.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:04:04.502317 runtimepy-1.5.3/runtimepy/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:04:04.506317 runtimepy-1.5.3/runtimepy/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:04:04.506317 runtimepy-1.5.3/runtimepy/channel/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/channel/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/channel/environment/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/channel/environment/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/channel/environment/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/channel/environment/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/channel/environment/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/channel/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:04:04.506317 runtimepy-1.5.3/runtimepy/codec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/codec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:04:04.506317 runtimepy-1.5.3/runtimepy/codec/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/codec/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/codec/protocol/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/codec/protocol/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:04:04.506317 runtimepy-1.5.3/runtimepy/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/commands/arbiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/commands/tui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:04:04.498317 runtimepy-1.5.3/runtimepy/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:04:04.510317 runtimepy-1.5.3/runtimepy/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/data/schemas/BitFields.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/data/schemas/Channel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/data/schemas/ChannelRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/data/schemas/ClientConnectionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/data/schemas/EnumRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/data/schemas/RuntimeEnum.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/data/schemas/ServerConnectionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:04:04.510317 runtimepy-1.5.3/runtimepy/enum/
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/enum/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/enum/type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:04:04.510317 runtimepy-1.5.3/runtimepy/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/mixins/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/mixins/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/names.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:04:04.510317 runtimepy-1.5.3/runtimepy/net/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:04:04.510317 runtimepy-1.5.3/runtimepy/net/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/net/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:04:04.514317 runtimepy-1.5.3/runtimepy/net/arbiter/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/net/arbiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/net/arbiter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/net/arbiter/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/net/arbiter/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/net/arbiter/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/net/arbiter/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/net/arbiter/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/net/arbiter/udp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/net/arbiter/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/net/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:04:04.514317 runtimepy-1.5.3/runtimepy/net/factories/
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/net/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/net/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/net/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:04:04.514317 runtimepy-1.5.3/runtimepy/net/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/net/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/net/tcp/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:04:04.514317 runtimepy-1.5.3/runtimepy/net/tcp/telnet/
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/net/tcp/telnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/net/tcp/telnet/codes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:04:04.514317 runtimepy-1.5.3/runtimepy/net/udp/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/net/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/net/udp/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/net/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:04:04.514317 runtimepy-1.5.3/runtimepy/net/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/net/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/net/websocket/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:04:04.514317 runtimepy-1.5.3/runtimepy/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/primitives/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/primitives/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/primitives/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/primitives/byte_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:04:04.518317 runtimepy-1.5.3/runtimepy/primitives/field/
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/primitives/field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/primitives/field/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:04:04.518317 runtimepy-1.5.3/runtimepy/primitives/field/manager/
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/primitives/field/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/primitives/field/manager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/primitives/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/primitives/int.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/primitives/string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:04:04.518317 runtimepy-1.5.3/runtimepy/primitives/type/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/primitives/type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/primitives/type/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/primitives/type/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/primitives/type/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/primitives/type/int.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:04:04.518317 runtimepy-1.5.3/runtimepy/registry/
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/registry/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/registry/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/registry/name.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:04:04.518317 runtimepy-1.5.3/runtimepy/task/
--rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:04:04.518317 runtimepy-1.5.3/runtimepy/task/basic/
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/task/basic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:04:04.518317 runtimepy-1.5.3/runtimepy/telemetry/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/telemetry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:04:04.518317 runtimepy-1.5.3/runtimepy/tui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/tui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:04:04.518317 runtimepy-1.5.3/runtimepy/tui/channels/
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/tui/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-05 01:02:15.000000 runtimepy-1.5.3/runtimepy/tui/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:04:04.502317 runtimepy-1.5.3/runtimepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-05 01:04:04.000000 runtimepy-1.5.3/runtimepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-05 01:04:04.000000 runtimepy-1.5.3/runtimepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 01:04:04.000000 runtimepy-1.5.3/runtimepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-05 01:04:04.000000 runtimepy-1.5.3/runtimepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-05 01:04:04.000000 runtimepy-1.5.3/runtimepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 01:04:04.000000 runtimepy-1.5.3/runtimepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 01:04:04.522317 runtimepy-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-05 01:02:15.000000 runtimepy-1.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:04:04.518317 runtimepy-1.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-05 01:02:15.000000 runtimepy-1.5.3/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-05 01:02:15.000000 runtimepy-1.5.3/tests/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-05 01:02:15.000000 runtimepy-1.5.3/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.342651 runtimepy-1.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-31 22:08:49.000000 runtimepy-1.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-31 22:10:17.342651 runtimepy-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-31 22:08:49.000000 runtimepy-1.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-31 22:08:49.000000 runtimepy-1.5.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.330651 runtimepy-1.5.4/runtimepy/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.330651 runtimepy-1.5.4/runtimepy/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.330651 runtimepy-1.5.4/runtimepy/channel/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/channel/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/channel/environment/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/channel/environment/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/channel/environment/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/channel/environment/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/channel/environment/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/channel/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.330651 runtimepy-1.5.4/runtimepy/codec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/codec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.330651 runtimepy-1.5.4/runtimepy/codec/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/codec/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/codec/protocol/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/codec/protocol/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.334651 runtimepy-1.5.4/runtimepy/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/commands/arbiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/commands/tui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.326651 runtimepy-1.5.4/runtimepy/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.334651 runtimepy-1.5.4/runtimepy/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/data/schemas/BitFields.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/data/schemas/Channel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/data/schemas/ChannelRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/data/schemas/ClientConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/data/schemas/EnumRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/data/schemas/RuntimeEnum.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/data/schemas/ServerConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.334651 runtimepy-1.5.4/runtimepy/enum/
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/enum/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/enum/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.334651 runtimepy-1.5.4/runtimepy/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/mixins/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/mixins/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.334651 runtimepy-1.5.4/runtimepy/net/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.334651 runtimepy-1.5.4/runtimepy/net/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.338651 runtimepy-1.5.4/runtimepy/net/arbiter/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/arbiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/arbiter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/arbiter/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/arbiter/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/arbiter/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/arbiter/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/arbiter/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/arbiter/udp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/arbiter/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.338651 runtimepy-1.5.4/runtimepy/net/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.338651 runtimepy-1.5.4/runtimepy/net/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/tcp/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.338651 runtimepy-1.5.4/runtimepy/net/tcp/telnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/tcp/telnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/tcp/telnet/codes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.338651 runtimepy-1.5.4/runtimepy/net/udp/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/udp/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.338651 runtimepy-1.5.4/runtimepy/net/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/websocket/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.338651 runtimepy-1.5.4/runtimepy/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/byte_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.338651 runtimepy-1.5.4/runtimepy/primitives/field/
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/field/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.338651 runtimepy-1.5.4/runtimepy/primitives/field/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/field/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/field/manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.338651 runtimepy-1.5.4/runtimepy/primitives/type/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/type/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/type/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/type/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/type/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.342651 runtimepy-1.5.4/runtimepy/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/registry/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/registry/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/registry/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.342651 runtimepy-1.5.4/runtimepy/task/
+-rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.342651 runtimepy-1.5.4/runtimepy/task/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/task/basic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.342651 runtimepy-1.5.4/runtimepy/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/telemetry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.342651 runtimepy-1.5.4/runtimepy/tui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/tui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.342651 runtimepy-1.5.4/runtimepy/tui/channels/
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/tui/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/tui/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.330651 runtimepy-1.5.4/runtimepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-31 22:10:17.000000 runtimepy-1.5.4/runtimepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-31 22:10:17.000000 runtimepy-1.5.4/runtimepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 22:10:17.000000 runtimepy-1.5.4/runtimepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-31 22:10:17.000000 runtimepy-1.5.4/runtimepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-31 22:10:17.000000 runtimepy-1.5.4/runtimepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-31 22:10:17.000000 runtimepy-1.5.4/runtimepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 22:10:17.342651 runtimepy-1.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-31 22:08:49.000000 runtimepy-1.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.342651 runtimepy-1.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-31 22:08:49.000000 runtimepy-1.5.4/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-31 22:08:49.000000 runtimepy-1.5.4/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-31 22:08:49.000000 runtimepy-1.5.4/tests/test_resources.py
```

### Comparing `runtimepy-1.5.3/LICENSE` & `runtimepy-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/PKG-INFO` & `runtimepy-1.5.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 1.5.3
+Version: 1.5.4
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=cde638b7567222966c038f6c0d5719e0
+    hash=3bc7656b5df806d21148ec2b5b2c0082
     =====================================
 -->
 
-# runtimepy ([1.5.3](https://pypi.org/project/runtimepy/))
+# runtimepy ([1.5.4](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-1.5.3/README.md` & `runtimepy-1.5.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=cde638b7567222966c038f6c0d5719e0
+    hash=3bc7656b5df806d21148ec2b5b2c0082
     =====================================
 -->
 
-# runtimepy ([1.5.3](https://pypi.org/project/runtimepy/))
+# runtimepy ([1.5.4](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-1.5.3/pyproject.toml` & `runtimepy-1.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "runtimepy"
-version = "1.5.3"
+version = "1.5.4"
 description = "A framework for implementing Python services."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `runtimepy-1.5.3/runtimepy/app.py` & `runtimepy-1.5.4/runtimepy/app.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/channel/__init__.py` & `runtimepy-1.5.4/runtimepy/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/channel/environment/__init__.py` & `runtimepy-1.5.4/runtimepy/channel/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/channel/environment/array.py` & `runtimepy-1.5.4/runtimepy/channel/environment/array.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/channel/environment/base.py` & `runtimepy-1.5.4/runtimepy/channel/environment/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/channel/environment/create.py` & `runtimepy-1.5.4/runtimepy/channel/environment/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/channel/environment/file.py` & `runtimepy-1.5.4/runtimepy/channel/environment/file.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/channel/environment/names.py` & `runtimepy-1.5.4/runtimepy/channel/environment/names.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/channel/registry.py` & `runtimepy-1.5.4/runtimepy/channel/registry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/codec/protocol/base.py` & `runtimepy-1.5.4/runtimepy/codec/protocol/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/codec/protocol/json.py` & `runtimepy-1.5.4/runtimepy/codec/protocol/json.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/commands/all.py` & `runtimepy-1.5.4/runtimepy/commands/all.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/commands/arbiter.py` & `runtimepy-1.5.4/runtimepy/commands/arbiter.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/commands/tui.py` & `runtimepy-1.5.4/runtimepy/commands/tui.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/data/schemas/BitFields.yaml` & `runtimepy-1.5.4/runtimepy/data/schemas/BitFields.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/data/schemas/ConnectionArbiterConfig.yaml` & `runtimepy-1.5.4/runtimepy/data/schemas/ConnectionArbiterConfig.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/entry.py` & `runtimepy-1.5.4/runtimepy/entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/enum/__init__.py` & `runtimepy-1.5.4/runtimepy/enum/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/enum/registry.py` & `runtimepy-1.5.4/runtimepy/enum/registry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/enum/type.py` & `runtimepy-1.5.4/runtimepy/enum/type.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/mapping.py` & `runtimepy-1.5.4/runtimepy/mapping.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/mixins/enum.py` & `runtimepy-1.5.4/runtimepy/mixins/enum.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/mixins/regex.py` & `runtimepy-1.5.4/runtimepy/mixins/regex.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/net/__init__.py` & `runtimepy-1.5.4/runtimepy/net/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/net/arbiter/__init__.py` & `runtimepy-1.5.4/runtimepy/net/arbiter/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/net/arbiter/base.py` & `runtimepy-1.5.4/runtimepy/net/arbiter/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/net/arbiter/config.py` & `runtimepy-1.5.4/runtimepy/net/arbiter/config.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/net/arbiter/factory.py` & `runtimepy-1.5.4/runtimepy/net/arbiter/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 """
 
 # built-in
 import asyncio as _asyncio
 from typing import Dict as _Dict
 from typing import List as _List
 
+# third-party
+from vcorelib.names import obj_class_to_snake
+
 # internal
-from runtimepy.names import obj_class_to_snake
 from runtimepy.net.arbiter.base import (
     BaseConnectionArbiter as _BaseConnectionArbiter,
 )
 from runtimepy.net.arbiter.base import ServerTask as _ServerTask
 from runtimepy.net.connection import Connection as _Connection
 from runtimepy.net.manager import ConnectionManager as _ConnectionManager
```

### Comparing `runtimepy-1.5.3/runtimepy/net/arbiter/imports.py` & `runtimepy-1.5.4/runtimepy/net/arbiter/imports.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/net/arbiter/info.py` & `runtimepy-1.5.4/runtimepy/net/arbiter/info.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/net/arbiter/tcp.py` & `runtimepy-1.5.4/runtimepy/net/arbiter/tcp.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/net/arbiter/udp.py` & `runtimepy-1.5.4/runtimepy/net/arbiter/udp.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/net/arbiter/websocket.py` & `runtimepy-1.5.4/runtimepy/net/arbiter/websocket.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/net/connection.py` & `runtimepy-1.5.4/runtimepy/net/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/net/factories/__init__.py` & `runtimepy-1.5.4/runtimepy/net/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/net/manager.py` & `runtimepy-1.5.4/runtimepy/net/manager.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/net/mixin.py` & `runtimepy-1.5.4/runtimepy/net/mixin.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/net/tcp/connection.py` & `runtimepy-1.5.4/runtimepy/net/tcp/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/net/tcp/telnet/__init__.py` & `runtimepy-1.5.4/runtimepy/net/tcp/telnet/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/net/tcp/telnet/codes.py` & `runtimepy-1.5.4/runtimepy/net/tcp/telnet/codes.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/net/udp/connection.py` & `runtimepy-1.5.4/runtimepy/net/udp/connection.py`

 * *Files 9% similar despite different names*

```diff
@@ -95,23 +95,32 @@
     ) -> bool:
         """Process a datagram."""
 
     def sendto(
         self, data: bytes, addr: _Union[IpHost, _Tuple[str, int]] = None
     ) -> None:
         """Send to a specific address."""
-        self._transport.sendto(data, addr=addr)
+
+        try:
+            self._transport.sendto(data, addr=addr)
+
+        # Catch a bug in the underlying event loop implementation - we try to
+        # send, but the underlying socket is gone (e.g. attribute is 'None').
+        # This seems to be possible (but intermittent) when shutting down the
+        # application.
+        except AttributeError as exc:
+            self.disable(str(exc))
 
     def send_text(self, data: str) -> None:
         """Enqueue a text message to send."""
-        self._transport.sendto(data.encode(), addr=self.remote_address)
+        self.sendto(data.encode(), addr=self.remote_address)
 
     def send_binary(self, data: _BinaryMessage) -> None:
         """Enqueue a binary message tos end."""
-        self._transport.sendto(data, addr=self.remote_address)
+        self.sendto(data, addr=self.remote_address)
 
     @classmethod
     async def create_connection(
         cls: _Type[T], connect: bool = True, **kwargs
     ) -> T:
         """Create a UDP connection."""
```

### Comparing `runtimepy-1.5.3/runtimepy/net/util.py` & `runtimepy-1.5.4/runtimepy/net/util.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/net/websocket/connection.py` & `runtimepy-1.5.4/runtimepy/net/websocket/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/primitives/__init__.py` & `runtimepy-1.5.4/runtimepy/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/primitives/array.py` & `runtimepy-1.5.4/runtimepy/primitives/array.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/primitives/base.py` & `runtimepy-1.5.4/runtimepy/primitives/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/primitives/bool.py` & `runtimepy-1.5.4/runtimepy/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/primitives/byte_order.py` & `runtimepy-1.5.4/runtimepy/primitives/byte_order.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/primitives/field/__init__.py` & `runtimepy-1.5.4/runtimepy/primitives/field/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/primitives/field/fields.py` & `runtimepy-1.5.4/runtimepy/primitives/field/fields.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/primitives/field/manager/__init__.py` & `runtimepy-1.5.4/runtimepy/primitives/field/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/primitives/field/manager/base.py` & `runtimepy-1.5.4/runtimepy/primitives/field/manager/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/primitives/float.py` & `runtimepy-1.5.4/runtimepy/primitives/float.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/primitives/int.py` & `runtimepy-1.5.4/runtimepy/primitives/int.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/primitives/string.py` & `runtimepy-1.5.4/runtimepy/primitives/string.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/primitives/type/__init__.py` & `runtimepy-1.5.4/runtimepy/primitives/type/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/primitives/type/base.py` & `runtimepy-1.5.4/runtimepy/primitives/type/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/primitives/type/float.py` & `runtimepy-1.5.4/runtimepy/primitives/type/float.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/primitives/type/int.py` & `runtimepy-1.5.4/runtimepy/primitives/type/int.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/registry/__init__.py` & `runtimepy-1.5.4/runtimepy/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/registry/bool.py` & `runtimepy-1.5.4/runtimepy/registry/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/registry/item.py` & `runtimepy-1.5.4/runtimepy/registry/item.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/registry/name.py` & `runtimepy-1.5.4/runtimepy/registry/name.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/schemas.py` & `runtimepy-1.5.4/runtimepy/schemas.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/task/__init__.py` & `runtimepy-1.5.4/runtimepy/task/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/task/basic/__init__.py` & `runtimepy-1.5.4/runtimepy/task/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/tui/channels/__init__.py` & `runtimepy-1.5.4/runtimepy/tui/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy/tui/task.py` & `runtimepy-1.5.4/runtimepy/tui/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/runtimepy.egg-info/PKG-INFO` & `runtimepy-1.5.4/runtimepy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 1.5.3
+Version: 1.5.4
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=cde638b7567222966c038f6c0d5719e0
+    hash=3bc7656b5df806d21148ec2b5b2c0082
     =====================================
 -->
 
-# runtimepy ([1.5.3](https://pypi.org/project/runtimepy/))
+# runtimepy ([1.5.4](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-1.5.3/runtimepy.egg-info/SOURCES.txt` & `runtimepy-1.5.4/runtimepy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 setup.py
 runtimepy/__init__.py
 runtimepy/__main__.py
 runtimepy/app.py
 runtimepy/dev_requirements.txt
 runtimepy/entry.py
 runtimepy/mapping.py
-runtimepy/names.py
 runtimepy/py.typed
 runtimepy/requirements.txt
 runtimepy/schemas.py
 runtimepy.egg-info/PKG-INFO
 runtimepy.egg-info/SOURCES.txt
 runtimepy.egg-info/dependency_links.txt
 runtimepy.egg-info/entry_points.txt
```

### Comparing `runtimepy-1.5.3/setup.py` & `runtimepy-1.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/tests/test_entry.py` & `runtimepy-1.5.4/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.3/tests/test_mapping.py` & `runtimepy-1.5.4/tests/test_mapping.py`

 * *Files identical despite different names*

