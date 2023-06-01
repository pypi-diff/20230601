# Comparing `tmp/python-selve-new-2.0.9.tar.gz` & `tmp/python-selve-new-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-selve-new-2.0.9.tar", last modified: Fri Nov  4 10:00:53 2022, max compression
+gzip compressed data, was "python-selve-new-2.1.0.tar", last modified: Thu Jun  1 17:30:11 2023, max compression
```

## Comparing `python-selve-new-2.0.9.tar` & `python-selve-new-2.1.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 10:00:53.497413 python-selve-new-2.0.9/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      905 2022-11-04 10:00:53.497413 python-selve-new-2.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 10:00:53.497413 python-selve-new-2.0.9/python_selve_new.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      905 2022-11-04 10:00:53.000000 python-selve-new-2.0.9/python_selve_new.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-11-04 10:00:53.000000 python-selve-new-2.0.9/python_selve_new.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-04 10:00:53.000000 python-selve-new-2.0.9/python_selve_new.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-11-04 10:00:53.000000 python-selve-new-2.0.9/python_selve_new.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-04 10:00:53.000000 python-selve-new-2.0.9/python_selve_new.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 10:00:53.497413 python-selve-new-2.0.9/selve/
--rw-r--r--   0 runner    (1001) docker     (121)    43489 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 10:00:53.497413 python-selve-new-2.0.9/selve/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6656 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/commands/command.py
--rw-r--r--   0 runner    (1001) docker     (121)     5230 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/commands/device.py
--rw-r--r--   0 runner    (1001) docker     (121)      624 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/commands/event.py
--rw-r--r--   0 runner    (1001) docker     (121)     1561 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/commands/group.py
--rw-r--r--   0 runner    (1001) docker     (121)     4554 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/commands/iveo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2748 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/commands/param.py
--rw-r--r--   0 runner    (1001) docker     (121)     5956 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/commands/senSim.py
--rw-r--r--   0 runner    (1001) docker     (121)     3574 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/commands/sender.py
--rw-r--r--   0 runner    (1001) docker     (121)     3677 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/commands/sensor.py
--rw-r--r--   0 runner    (1001) docker     (121)     2341 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/commands/service.py
--rw-r--r--   0 runner    (1001) docker     (121)     1338 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/device.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/gateway.py
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/group.py
--rw-r--r--   0 runner    (1001) docker     (121)      814 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/iveo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/senSim.py
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/sender.py
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 10:00:53.497413 python-selve-new-2.0.9/selve/util/
--rw-r--r--   0 runner    (1001) docker     (121)     9741 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      776 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/util/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     3342 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/util/protocol.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-04 10:00:53.497413 python-selve-new-2.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2791 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:30:11.431332 python-selve-new-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-01 17:30:11.431332 python-selve-new-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:30:11.431332 python-selve-new-2.1.0/python_selve_new.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-01 17:30:11.000000 python-selve-new-2.1.0/python_selve_new.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-01 17:30:11.000000 python-selve-new-2.1.0/python_selve_new.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 17:30:11.000000 python-selve-new-2.1.0/python_selve_new.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 17:30:11.000000 python-selve-new-2.1.0/python_selve_new.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-01 17:30:11.000000 python-selve-new-2.1.0/python_selve_new.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:30:11.431332 python-selve-new-2.1.0/selve/
+-rw-r--r--   0 runner    (1001) docker     (123)    50840 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:30:11.431332 python-selve-new-2.1.0/selve/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/commands/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/commands/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/commands/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/commands/iveo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/commands/param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/commands/senSim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/commands/sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/commands/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/commands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/iveo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/senSim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:30:11.431332 python-selve-new-2.1.0/selve/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/util/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/util/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 17:30:11.431332 python-selve-new-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/setup.py
```

### Comparing `python-selve-new-2.0.9/LICENSE` & `python-selve-new-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.9/python_selve_new.egg-info/SOURCES.txt` & `python-selve-new-2.1.0/python_selve_new.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.9/selve/commands/command.py` & `python-selve-new-2.1.0/selve/commands/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,12 +132,12 @@
         self.executed = bool(parameters[0][1])
         self.ids = [ b for b in Util.true_in_list(Util.b64bytes_to_bitlist(parameters[1][1]))]
 
 
 class CommandResultResponse(MethodResponse):
     def __init__(self, name, parameters):
         super().__init__(name, parameters)
-        self.command = DriveCommandIveo(int(parameters[0][1]))
+        self.command = DriveCommandCommeo(int(parameters[0][1]))
         self.commandType = DeviceCommandType(int(parameters[1][1]))
         self.executed = bool(parameters[2][1])
         self.successIds = [ b for b in Util.true_in_list(Util.b64bytes_to_bitlist(parameters[3][1]))]
         self.failedIds = [ b for b in Util.true_in_list(Util.b64bytes_to_bitlist(parameters[4][1]))]
```

### Comparing `python-selve-new-2.0.9/selve/commands/device.py` & `python-selve-new-2.1.0/selve/commands/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,17 +89,17 @@
         super().__init__(name, parameters)
         self.ids = [b for b in Util.true_in_list(Util.b64bytes_to_bitlist(parameters[0][1]))]
 
 
 class DeviceGetInfoResponse(MethodResponse):
     def __init__(self, name, parameters):
         super().__init__(name, parameters)
-        self.name = parameters[0][1]
+        self.name = parameters[0][1] if parameters[0][1] else "None"
         self.rfAddress = parameters[2][1]
-        self.deviceType = DeviceType(int(parameters[3][1]))
+        self.deviceType = DeviceType(int(parameters[3][1])) if int(parameters[3][1]) else DeviceType(0)
         self.state = DeviceState(int(parameters[4][1]))
 
 
 class DeviceGetValuesResponse(MethodResponse):
     def __init__(self, name, parameters):
         super().__init__(name, parameters)
         self.name = parameters[0][1] if parameters[0][1] else ""
```

### Comparing `python-selve-new-2.0.9/selve/commands/event.py` & `python-selve-new-2.1.0/selve/commands/event.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.9/selve/commands/group.py` & `python-selve-new-2.1.0/selve/commands/group.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.9/selve/commands/iveo.py` & `python-selve-new-2.1.0/selve/commands/iveo.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,23 +44,23 @@
 
 class IveoLearn(GatewayCommand):
     def __init__(self, id: int):
         super().__init__(IveoCommand.LEARN, [(ParameterType.INT, id)])
 
 
 class IveoManual(GatewayCommand):
-    def __init__(self, actorIds: dict, command: DriveCommandIveo):
+    def __init__(self, actorId: int, command: DriveCommandIveo):
         super().__init__(IveoCommand.MANUAL,
-                         [(ParameterType.BASE64, Util.multimask(actorIds)), (ParameterType.INT, command.value)])
+                         [(ParameterType.BASE64, Util.singlemask(actorId)), (ParameterType.INT, command.value)])
 
 
 class IveoAutomatic(GatewayCommand):
-    def __init__(self, actorIds: dict, command: DriveCommandIveo):
+    def __init__(self, actorId: int, command: DriveCommandIveo):
         super().__init__(IveoCommand.AUTOMATIC,
-                         [(ParameterType.BASE64, Util.multimask(actorIds)), (ParameterType.INT, command.value)])
+                         [(ParameterType.BASE64, Util.singlemask(actorId)), (ParameterType.INT, command.value)])
 
 
 class IveoResult(GatewayCommand):
     def __init__(self):
         super().__init__(IveoCommand.RESULT)
 
 
@@ -132,9 +132,9 @@
         self.executed = bool(parameters[0][1])
 
 
 class IveoResultResponse(MethodResponse):
     def __init__(self, name, parameters):
         super().__init__(name, parameters)
         self.command = DriveCommandIveo(int(parameters[0][1]))
-        self.state = CommandResultState(int(parameters[2][1]))
-        self.executedIds = [ b for b in Util.true_in_list(Util.b64bytes_to_bitlist(parameters[1][1]))]
+        self.state = CommandResultState(int(parameters[1][1]))
+        self.executedIds = [ b for b in Util.true_in_list(Util.b64bytes_to_bitlist(parameters[2][1]))]
```

### Comparing `python-selve-new-2.0.9/selve/commands/param.py` & `python-selve-new-2.1.0/selve/commands/param.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.9/selve/commands/senSim.py` & `python-selve-new-2.1.0/selve/commands/senSim.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.9/selve/commands/sender.py` & `python-selve-new-2.1.0/selve/commands/sender.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.9/selve/commands/sensor.py` & `python-selve-new-2.1.0/selve/commands/sensor.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.9/selve/commands/service.py` & `python-selve-new-2.1.0/selve/commands/service.py`

 * *Files 16% similar despite different names*

```diff
@@ -47,17 +47,17 @@
         self.state = parameters[0][1]
 
 
 class ServiceGetVersionResponse(MethodResponse):
     def __init__(self, name, parameters):
         super().__init__(name, parameters)
         self.serial = str(parameters[0][1])
-        self.version = int(parameters[1][1]) + "." + int(parameters[2][1]) + "." + int(parameters[3][1]) + "." + int(
-            parameters[6][1])
-        self.spec = int(parameters[4][1]) + "." + int(parameters[5][1])
+        self.version = str(int(parameters[1][1])) + "." + str(int(parameters[2][1])) + "." + str(int(parameters[3][1])) + "." + str(int(
+            parameters[6][1]))
+        self.spec = str(int(parameters[4][1])) + "." + str(int(parameters[5][1]))
 
 
 class ServiceResetResponse(MethodResponse):
     def __init__(self, name, parameters):
         super().__init__(name, parameters)
         self.executed = bool(parameters[0][1])
```

### Comparing `python-selve-new-2.0.9/selve/device.py` & `python-selve-new-2.1.0/selve/device.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.9/selve/group.py` & `python-selve-new-2.1.0/selve/group.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.9/selve/iveo.py` & `python-selve-new-2.1.0/selve/iveo.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.9/selve/senSim.py` & `python-selve-new-2.1.0/selve/senSim.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.9/selve/sender.py` & `python-selve-new-2.1.0/selve/sender.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.9/selve/sensor.py` & `python-selve-new-2.1.0/selve/sensor.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.9/selve/util/__init__.py` & `python-selve-new-2.1.0/selve/util/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,32 +48,33 @@
         self.executed = bool(parameters[2][1])
         self.successIds = [ b for b in Util.true_in_list(Util.b64bytes_to_bitlist(parameters[3][1]))]
         self.failedIds = [ b for b in Util.true_in_list(Util.b64bytes_to_bitlist(parameters[4][1]))]
 
 class CommeoDeviceEventResponse(MethodResponse):
     def __init__(self, name, parameters):
         super().__init__(name, parameters)
-        self.name = str(parameters[0][1])
-        self.id = int(parameters[1][1])
-        self.actorState = MovementState(int(parameters[2][1]))
-        self.value = Util.valueToPercentage(int(parameters[3][1]))
-        self.targetValue = Util.valueToPercentage(int(parameters[4][1]))
-        bArr = Util.intToBoolarray(int(parameters[5][1]))
+        #self.name = parameters[0][1] if parameters[0][1] else ""
+        self.id = int(parameters[0][1])
+        self.actorState = MovementState(int(parameters[1][1])) if int(parameters[1][1]) and int(parameters[1][1]) < 4 else MovementState(0)        
+        self.value = Util.valueToPercentage(int(parameters[2][1]))
+        self.targetValue = Util.valueToPercentage(int(parameters[3][1]))
+        
+        bArr = Util.intToBoolarray(int(parameters[4][1]))
         self.unreachable = bArr[0]
         self.overload = bArr[1]
         self.obstructed = bArr[2]
         self.alarm = bArr[3]
         self.lostSensor = bArr[4]
         self.automaticMode = bArr[5]
         self.gatewayNotLearned = bArr[6]
         self.windAlarm = bArr[7]
         self.rainAlarm = bArr[8]
         self.freezingAlarm = bArr[9]
-        self.dayMode = DayMode(int(parameters[6][1]))
-        self.deviceType = DeviceType(int(parameters[7][1]))
+        self.dayMode = DayMode(int(parameters[5][1]))
+        self.deviceType = DeviceType(int(parameters[6][1]))
 
 class LogEventResponse(MethodResponse):
     def __init__(self, name, parameters):
         super().__init__(name, parameters)
         self.logCode = str(parameters[0][1])
         self.logStamp = str(parameters[1][1])
         self.logValue = str(parameters[2][1])
@@ -117,24 +118,24 @@
 
 class Util():
     @classmethod
     def singlemask(self, id):
         #Obtains a base64 encoded to modify just one index
         mask =  64 * [0]
         #need to transform the position
-        newid = int((id // 8) * 8  + 7 - (id % 8))    
+        newid = int((int(id) // 8) * 8  + 7 - (int(id) % 8))    
         mask[newid] = 1
         bitstring = "".join(str(x) for x in mask)
         return base64.b64encode(self.bitstring_to_bytes(bitstring)).decode('utf8')
 
     @classmethod
     def multimask(self, ids):
         mask = 64 * [0]
         for id in ids:
-            newid = int((id // 8) * 8  + 7 - (id % 8))    
+            newid = int((int(id) // 8) * 8  + 7 - (int(id) % 8))    
             mask[newid] = 1
         bitstring = "".join(str(x) for x in mask)
         return base64.b64encode(self.bitstring_to_bytes(bitstring)).decode('utf8')
 
     @classmethod
     def bitstring_to_bytes(self, s):
         return int(s, 2).to_bytes(len(s) // 8, byteorder='big')
@@ -151,29 +152,29 @@
 
     @classmethod
     def true_in_list(self, l):
         return [i for i,v in enumerate(l) if v]
 
     @classmethod
     def valueToPercentage(self, value):
-        return int((value / 65535)*100)
+        return int((int(value) / 65535)*100)
     @classmethod
     def valueToDegrees(self, value):
-        return int((value / 65535)*360)
+        return int((int(value) / 65535)*360)
 
     @classmethod
     def percentageToValue(self, perc):
-        return int((65535/100)*(perc))
+        return int((65535/100)*(int(perc)))
     @classmethod
     def degreesToValue(self, perc):
-        return int((65535/360)*(perc))
+        return int((65535/360)*(int(perc)))
 
     @classmethod
     def intToBoolarray(self, value):
-        return [bool(bit) for bit in '{0:10b}'.format(value)]
+        return [bool(value & (1<<n)) for n in range(10)]
 
 from enum import Enum
 
 class CommeoServiceCommand(Enum):
     PING = "service.ping"
     GETSTATE = "service.getState"
     GETVERSION = "service.getVersion"
```

### Comparing `python-selve-new-2.0.9/selve/util/errors.py` & `python-selve-new-2.1.0/selve/util/errors.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.9/selve/util/protocol.py` & `python-selve-new-2.1.0/selve/util/protocol.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.9/setup.py` & `python-selve-new-2.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,41 +11,47 @@
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     
     name='python-selve-new',  # Required    
-    version='2.0.9',  # Required
+    version='2.1.0',  # Required
     description='Python library for interfacing with selve devices using the USB-RF controller. Written completely new.',  # Required   
     long_description=long_description,  # Optional 
     long_description_content_type="text/markdown",   
     url='https://github.com/Kannix2005/python-selve-new',  # Optional
     author='Stefan Altheimer',  # Optional
    
     author_email='me@stefan-altheimer.de',  # Optional
 
     # Classifiers help users find your project by categorizing it.
     #
     # For a list of valid classifiers, see
     # https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[  # Optional        
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'Topic :: Software Development :: Build Tools',
+        'Development Status :: 5 - Production/Stable',
+        'Intended Audience :: Information Technology',
+        'Topic :: Software Development :: Libraries :: Python Modules',
 
         # Pick your license as you wish
-        'License :: OSI Approved :: MIT License',
+        'License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)',
 
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12'
     ],
    
     keywords='selve blind awning shutter usb rf',  # Optional
 
     packages=find_packages(),  # Required
 
     # This field lists other packages that your project depends on to run.
```

