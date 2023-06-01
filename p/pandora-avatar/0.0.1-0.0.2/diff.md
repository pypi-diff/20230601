# Comparing `tmp/pandora-avatar-0.0.1.tar.gz` & `tmp/pandora-avatar-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandora-avatar-0.0.1.tar", last modified: Fri May 12 21:39:18 2023, max compression
+gzip compressed data, was "pandora-avatar-0.0.2.tar", last modified: Thu Jun  1 17:48:29 2023, max compression
```

## Comparing `pandora-avatar-0.0.1.tar` & `pandora-avatar-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,12 @@
--rw-r--r--   0        0        0      968 2023-05-12 21:07:54.430231 pandora-avatar-0.0.1/README.md
--rw-r--r--   0        0        0     7886 2023-05-12 21:39:06.485296 pandora-avatar-0.0.1/avatar/__init__.py
--rw-r--r--   0        0        0     1561 2023-05-12 16:01:44.774248 pandora-avatar-0.0.1/avatar/aio.py
--rw-r--r--   0        0        0     4824 2023-05-12 16:01:44.774248 pandora-avatar-0.0.1/avatar/bumble_device.py
--rw-r--r--   0        0        0     3460 2023-05-12 16:01:44.774248 pandora-avatar-0.0.1/avatar/bumble_server/__init__.py
--rw-r--r--   0        0        0     1956 2023-05-12 16:01:44.774248 pandora-avatar-0.0.1/avatar/bumble_server/config.py
--rw-r--r--   0        0        0    30682 2023-05-12 16:01:44.778249 pandora-avatar-0.0.1/avatar/bumble_server/host.py
--rw-r--r--   0        0        0        0 2023-05-12 16:01:44.778249 pandora-avatar-0.0.1/avatar/bumble_server/py.typed
--rw-r--r--   0        0        0    19757 2023-05-12 16:01:44.778249 pandora-avatar-0.0.1/avatar/bumble_server/security.py
--rw-r--r--   0        0        0     3837 2023-05-12 16:01:44.778249 pandora-avatar-0.0.1/avatar/bumble_server/utils.py
--rw-r--r--   0        0        0      631 2023-05-12 16:01:44.778249 pandora-avatar-0.0.1/avatar/controllers/__init__.py
--rw-r--r--   0        0        0     1404 2023-05-12 16:01:44.778249 pandora-avatar-0.0.1/avatar/controllers/bumble_device.py
--rw-r--r--   0        0        0     1668 2023-05-12 16:01:44.778249 pandora-avatar-0.0.1/avatar/controllers/pandora_device.py
--rw-r--r--   0        0        0        0 2023-05-12 16:01:44.778249 pandora-avatar-0.0.1/avatar/controllers/py.typed
--rw-r--r--   0        0        0     7531 2023-05-12 16:01:44.778249 pandora-avatar-0.0.1/avatar/pandora_client.py
--rw-r--r--   0        0        0     4890 2023-05-12 16:01:44.778249 pandora-avatar-0.0.1/avatar/pandora_server.py
--rw-r--r--   0        0        0        0 2023-05-12 16:01:44.778249 pandora-avatar-0.0.1/avatar/py.typed
--rw-r--r--   0        0        0     1834 2023-05-12 20:48:36.735921 pandora-avatar-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1968 1970-01-01 00:00:00.000000 pandora-avatar-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      841 2023-06-01 17:48:15.945634 pandora-avatar-0.0.2/README.md
+-rw-r--r--   0        0        0     7886 2023-06-01 17:48:15.945634 pandora-avatar-0.0.2/avatar/__init__.py
+-rw-r--r--   0        0        0     1561 2023-06-01 17:48:15.945634 pandora-avatar-0.0.2/avatar/aio.py
+-rw-r--r--   0        0        0      608 2023-06-01 17:48:15.945634 pandora-avatar-0.0.2/avatar/controllers/__init__.py
+-rw-r--r--   0        0        0     1464 2023-06-01 17:48:15.945634 pandora-avatar-0.0.2/avatar/controllers/bumble_device.py
+-rw-r--r--   0        0        0     1668 2023-06-01 17:48:15.945634 pandora-avatar-0.0.2/avatar/controllers/pandora_device.py
+-rw-r--r--   0        0        0        0 2023-06-01 17:48:15.945634 pandora-avatar-0.0.2/avatar/controllers/py.typed
+-rw-r--r--   0        0        0     7520 2023-06-01 17:48:15.945634 pandora-avatar-0.0.2/avatar/pandora_client.py
+-rw-r--r--   0        0        0     4933 2023-06-01 17:48:15.949634 pandora-avatar-0.0.2/avatar/pandora_server.py
+-rw-r--r--   0        0        0        0 2023-06-01 17:48:15.949634 pandora-avatar-0.0.2/avatar/py.typed
+-rw-r--r--   0        0        0     1622 2023-06-01 17:48:15.949634 pandora-avatar-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1847 1970-01-01 00:00:00.000000 pandora-avatar-0.0.2/PKG-INFO
```

### Comparing `pandora-avatar-0.0.1/README.md` & `pandora-avatar-0.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -3,44 +3,41 @@
 Avatar aims to provide a scalable multi-platform Bluetooth testing tool capable
 of running any Bluetooth test cases virtually and physically. It aims to
 complete PTS-bot in the Pandora testing suite.
 
 ## Install
 
 ```bash
-git submodule update --init
 python -m venv venv
 source venv/bin/activate.fish # or any other shell
-pip install bumble
-pip install bt-test-interfaces
 pip install [-e] .
 ```
 
 ## Usage
 
 ```bash
-python examples/example.py -c examples/simulated_bumble_android.yml --verbose
+python cases/host_test.py -c cases/config.yml --verbose
 ```
 
 ## Development
 
 1. Make sure to have a `root-canal` instance running somewhere.
 ```bash
 root-canal
 ```
 
 1. Run the example using Bumble vs Bumble config file. The default `6402` HCI port of `root-canal` may be changed in this config file.
 ```
-python examples/example.py -c examples/simulated_bumble_bumble.yml --verbose
+python cases/host_test.py -c cases/config.yml --verbose
 ```
 
 3. Lint with `pyright` and `mypy`
 ```
 pyright
 mypy
 ```
 
 3. Format & imports style
 ```
-black avatar/ examples/
-isort avatar/ examples/
+black avatar/ cases/
+isort avatar/ cases/
 ```
```

### Comparing `pandora-avatar-0.0.1/avatar/__init__.py` & `pandora-avatar-0.0.2/avatar/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 """
 Avatar is a scalable multi-platform Bluetooth testing tool capable of running
 any Bluetooth test cases virtually and physically.
 """
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 import enum
 import functools
 import grpc
 import grpc.aio
 import importlib
 import logging
```

### Comparing `pandora-avatar-0.0.1/avatar/aio.py` & `pandora-avatar-0.0.2/avatar/aio.py`

 * *Files identical despite different names*

### Comparing `pandora-avatar-0.0.1/avatar/controllers/bumble_device.py` & `pandora-avatar-0.0.2/avatar/controllers/bumble_device.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,30 +13,30 @@
 # limitations under the License.
 
 """Bumble device Mobly controller."""
 
 import asyncio
 import avatar.aio
 
-from avatar.bumble_device import BumbleDevice
+from bumble.pandora.device import PandoraDevice as BumblePandoraDevice
 from typing import Any, Dict, List, Optional
 
 MOBLY_CONTROLLER_CONFIG_NAME = 'BumbleDevice'
 
 
-def create(configs: List[Dict[str, Any]]) -> List[BumbleDevice]:
+def create(configs: List[Dict[str, Any]]) -> List[BumblePandoraDevice]:
     """Create a list of `BumbleDevice` from configs."""
-    return [BumbleDevice(config) for config in configs]
+    return [BumblePandoraDevice(config) for config in configs]
 
 
-def destroy(devices: List[BumbleDevice]) -> None:
+def destroy(devices: List[BumblePandoraDevice]) -> None:
     """Destroy each `BumbleDevice`"""
 
     async def close_devices() -> None:
         await asyncio.gather(*(device.close() for device in devices))
 
     avatar.aio.run_until_complete(close_devices())
 
 
-def get_info(devices: List[BumbleDevice]) -> List[Optional[Dict[str, str]]]:
-    """Return the device info for each `BumbleDevice`."""
+def get_info(devices: List[BumblePandoraDevice]) -> List[Optional[Dict[str, str]]]:
+    """Return the device info for each `BumblePandoraDevice`."""
     return [device.info() for device in devices]
```

### Comparing `pandora-avatar-0.0.1/avatar/controllers/pandora_device.py` & `pandora-avatar-0.0.2/avatar/controllers/pandora_device.py`

 * *Files identical despite different names*

### Comparing `pandora-avatar-0.0.1/avatar/pandora_client.py` & `pandora-avatar-0.0.2/avatar/pandora_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 import avatar.aio
 import bumble
 import bumble.device
 import grpc
 import grpc.aio
 import logging
 
-from avatar import bumble_server
-from avatar.bumble_device import BumbleDevice
+from bumble import pandora as bumble_server
 from bumble.hci import Address as BumbleAddress
+from bumble.pandora.device import PandoraDevice as BumblePandoraDevice
 from dataclasses import dataclass
 from pandora import host_grpc, host_grpc_aio, security_grpc, security_grpc_aio
 from typing import Any, Dict, MutableMapping, Optional, Tuple, Union
 
 
 class Address(bytes):
     def __new__(cls, address: Union[bytes, str, BumbleAddress]) -> 'Address':
@@ -51,14 +51,15 @@
         return ':'.join([f'{x:02X}' for x in self])
 
 
 class PandoraClient:
     """Provides Pandora interface access to a device via gRPC."""
 
     # public fields
+    name: str
     grpc_target: str  # Server address for the gRPC channel.
     log: 'PandoraClientLoggerAdapter'  # Logger adapter.
 
     # private fields
     _channel: grpc.Channel  # Synchronous gRPC channel.
     _address: Address  # Bluetooth device address
     _aio: Optional['PandoraClient.Aio']  # Asynchronous gRPC channel.
@@ -67,16 +68,17 @@
         """Creates a PandoraClient.
 
         Establishes a channel with the Pandora gRPC server.
 
         Args:
           grpc_target: Server address for the gRPC channel.
         """
+        self.name = name
         self.grpc_target = grpc_target
-        self.log = PandoraClientLoggerAdapter(logging.getLogger(), {'client': self, 'client_name': name})
+        self.log = PandoraClientLoggerAdapter(logging.getLogger(), {'client': self})
         self._channel = grpc.insecure_channel(grpc_target)  # type: ignore
         self._address = Address(b'\x00\x00\x00\x00\x00\x00')
         self._aio = None
 
     def close(self) -> None:
         """Closes the gRPC channels."""
         self._channel.close()
@@ -174,26 +176,25 @@
 class PandoraClientLoggerAdapter(logging.LoggerAdapter):  # type: ignore
     """Formats logs from the PandoraClient."""
 
     def process(self, msg: str, kwargs: MutableMapping[str, Any]) -> Tuple[str, MutableMapping[str, Any]]:
         assert self.extra
         client = self.extra['client']
         assert isinstance(client, PandoraClient)
-        client_name = self.extra.get('client_name', client.__class__.__name__)
         addr = ':'.join([f'{x:02X}' for x in client.address[4:]])
-        return (f'[{client_name}:{addr}] {msg}', kwargs)
+        return (f'[{client.name}:{addr}] {msg}', kwargs)
 
 
 class BumblePandoraClient(PandoraClient):
     """Special Pandora client which also give access to a Bumble device instance."""
 
-    _bumble: BumbleDevice  # Bumble device wrapper.
+    _bumble: BumblePandoraDevice  # Bumble device wrapper.
     _server_config: bumble_server.Config  # Bumble server config.
 
-    def __init__(self, grpc_target: str, bumble: BumbleDevice, server_config: bumble_server.Config) -> None:
+    def __init__(self, grpc_target: str, bumble: BumblePandoraDevice, server_config: bumble_server.Config) -> None:
         super().__init__(grpc_target, 'bumble')
         self._bumble = bumble
         self._server_config = server_config
 
     @property
     def server_config(self) -> bumble_server.Config:
         return self._server_config
```

### Comparing `pandora-avatar-0.0.1/avatar/pandora_server.py` & `pandora-avatar-0.0.2/avatar/pandora_server.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 import asyncio
 import avatar.aio
 import grpc
 import grpc.aio
 import threading
 import types
 
-from avatar import bumble_server
-from avatar.bumble_device import BumbleDevice
 from avatar.controllers import bumble_device, pandora_device
 from avatar.pandora_client import BumblePandoraClient, PandoraClient
+from bumble import pandora as bumble_server
+from bumble.pandora.device import PandoraDevice as BumblePandoraDevice
 from contextlib import suppress
 from mobly.controllers import android_device
 from mobly.controllers.android_device import AndroidDevice
 from typing import Generic, Optional, TypeVar
 
 ANDROID_SERVER_PACKAGE = 'com.android.pandora'
 ANDROID_SERVER_GRPC_PORT = 8999  # TODO: Use a dynamic port
@@ -59,15 +59,15 @@
         assert isinstance(self.device, PandoraClient)
         return self.device
 
     def stop(self) -> None:
         """Stops and cleans up the Pandora server on the device."""
 
 
-class BumblePandoraServer(PandoraServer[BumbleDevice]):
+class BumblePandoraServer(PandoraServer[BumblePandoraDevice]):
     """Manages the Pandora gRPC server on a BumbleDevice."""
 
     MOBLY_CONTROLLER_MODULE = bumble_device
 
     _task: Optional[asyncio.Task[None]] = None
 
     def start(self) -> BumblePandoraClient:
```

### Comparing `pandora-avatar-0.0.1/pyproject.toml` & `pandora-avatar-0.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [project]
 name = "pandora-avatar"
 authors = [{name = "Pandora", email = "pandora-core@google.com"}]
 readme = "README.md"
 dynamic = ["version", "description"]
-requires-python = ">=3.10.9"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: Apache Software License"
 ]
 dependencies = [
     "bt-test-interfaces",
-    "bumble",
-    "grpcio==1.51.1",
+    "bumble==0.0.153",
+    "grpcio>=1.51.1",
     "mobly>=1.12",
     "bitstruct>=8.12",
 ]
 
 [project.urls]
 Source = "https://github.com/google/avatar"
 
 [project.optional-dependencies]
 dev = [
-    "grpcio-tools==1.51.1",
+    "grpcio-tools>=1.51.1",
     "black==22.10.0",
     "pyright==1.1.298",
     "mypy==1.0",
     "isort==5.12.0",
     "types-psutil>=5.9.5.6",
     "types-setuptools>=65.7.0.3",
     "types-protobuf>=4.21.0.3"
@@ -45,39 +45,33 @@
 no_sections = true
 lines_between_types = 1
 combine_as_imports = true
 
 [tool.mypy]
 strict = true
 warn_unused_ignores = false
-files = ["avatar", "examples"]
-mypy_path = '$MYPY_CONFIG_FILE_DIR/bt-test-interfaces/python:$MYPY_CONFIG_FILE_DIR/third-party/bumble'
-exclude = 'third-party/bumble'
+files = ["avatar", "cases"]
 
 [[tool.mypy.overrides]]
 module = "grpc.*"
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "mobly.*"
 ignore_missing_imports = true
 
 [tool.pyright]
-include = ["avatar", "examples"]
+include = ["avatar", "cases"]
 exclude = ["**/__pycache__"]
 typeCheckingMode = "strict"
 useLibraryCodeForTypes = true
 verboseOutput = false
-extraPaths = [
-    'bt-test-interfaces/python',
-    'third-party/bumble'
-]
 reportMissingTypeStubs = false
 reportUnknownLambdaType = false
 reportImportCycles = false
 
 [tool.pytype]
-inputs = ['avatar', 'examples']
+inputs = ['avatar', 'cases']
 
 [build-system]
 requires = ["flit_core==3.7.1"]
 build-backend = "flit_core.buildapi"
```

### Comparing `pandora-avatar-0.0.1/PKG-INFO` & `pandora-avatar-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pandora-avatar
-Version: 0.0.1
+Version: 0.0.2
 Summary: Avatar is a scalable multi-platform Bluetooth testing tool capable of running
 Author-email: Pandora <pandora-core@google.com>
-Requires-Python: >=3.10.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: bt-test-interfaces
-Requires-Dist: bumble
-Requires-Dist: grpcio==1.51.1
+Requires-Dist: bumble==0.0.153
+Requires-Dist: grpcio>=1.51.1
 Requires-Dist: mobly>=1.12
 Requires-Dist: bitstruct>=8.12
-Requires-Dist: grpcio-tools==1.51.1 ; extra == "dev"
+Requires-Dist: grpcio-tools>=1.51.1 ; extra == "dev"
 Requires-Dist: black==22.10.0 ; extra == "dev"
 Requires-Dist: pyright==1.1.298 ; extra == "dev"
 Requires-Dist: mypy==1.0 ; extra == "dev"
 Requires-Dist: isort==5.12.0 ; extra == "dev"
 Requires-Dist: types-psutil>=5.9.5.6 ; extra == "dev"
 Requires-Dist: types-setuptools>=65.7.0.3 ; extra == "dev"
 Requires-Dist: types-protobuf>=4.21.0.3 ; extra == "dev"
@@ -28,45 +28,42 @@
 Avatar aims to provide a scalable multi-platform Bluetooth testing tool capable
 of running any Bluetooth test cases virtually and physically. It aims to
 complete PTS-bot in the Pandora testing suite.
 
 ## Install
 
 ```bash
-git submodule update --init
 python -m venv venv
 source venv/bin/activate.fish # or any other shell
-pip install bumble
-pip install bt-test-interfaces
 pip install [-e] .
 ```
 
 ## Usage
 
 ```bash
-python examples/example.py -c examples/simulated_bumble_android.yml --verbose
+python cases/host_test.py -c cases/config.yml --verbose
 ```
 
 ## Development
 
 1. Make sure to have a `root-canal` instance running somewhere.
 ```bash
 root-canal
 ```
 
 1. Run the example using Bumble vs Bumble config file. The default `6402` HCI port of `root-canal` may be changed in this config file.
 ```
-python examples/example.py -c examples/simulated_bumble_bumble.yml --verbose
+python cases/host_test.py -c cases/config.yml --verbose
 ```
 
 3. Lint with `pyright` and `mypy`
 ```
 pyright
 mypy
 ```
 
 3. Format & imports style
 ```
-black avatar/ examples/
-isort avatar/ examples/
+black avatar/ cases/
+isort avatar/ cases/
 ```
```

