# Comparing `tmp/python-selve-new-2.1.8.tar.gz` & `tmp/python-selve-new-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-selve-new-2.1.8.tar", last modified: Thu Jun  1 20:42:05 2023, max compression
+gzip compressed data, was "python-selve-new-2.1.9.tar", last modified: Thu Jun  1 21:25:48 2023, max compression
```

## Comparing `python-selve-new-2.1.8.tar` & `python-selve-new-2.1.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:42:05.087584 python-selve-new-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-01 20:41:58.000000 python-selve-new-2.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-01 20:42:05.087584 python-selve-new-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-01 20:41:58.000000 python-selve-new-2.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:42:05.087584 python-selve-new-2.1.8/python_selve_new.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-01 20:42:04.000000 python-selve-new-2.1.8/python_selve_new.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-01 20:42:05.000000 python-selve-new-2.1.8/python_selve_new.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:42:05.000000 python-selve-new-2.1.8/python_selve_new.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 20:42:05.000000 python-selve-new-2.1.8/python_selve_new.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-01 20:42:05.000000 python-selve-new-2.1.8/python_selve_new.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:42:05.087584 python-selve-new-2.1.8/selve/
--rw-r--r--   0 runner    (1001) docker     (123)    50660 2023-06-01 20:41:58.000000 python-selve-new-2.1.8/selve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:42:05.087584 python-selve-new-2.1.8/selve/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:58.000000 python-selve-new-2.1.8/selve/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-06-01 20:41:58.000000 python-selve-new-2.1.8/selve/commands/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-06-01 20:41:58.000000 python-selve-new-2.1.8/selve/commands/device.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-01 20:41:58.000000 python-selve-new-2.1.8/selve/commands/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-01 20:41:58.000000 python-selve-new-2.1.8/selve/commands/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-01 20:41:58.000000 python-selve-new-2.1.8/selve/commands/iveo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-01 20:41:58.000000 python-selve-new-2.1.8/selve/commands/param.py
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-01 20:41:58.000000 python-selve-new-2.1.8/selve/commands/senSim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-06-01 20:41:58.000000 python-selve-new-2.1.8/selve/commands/sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-06-01 20:41:58.000000 python-selve-new-2.1.8/selve/commands/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-01 20:41:58.000000 python-selve-new-2.1.8/selve/commands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-01 20:41:58.000000 python-selve-new-2.1.8/selve/device.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:58.000000 python-selve-new-2.1.8/selve/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-01 20:41:58.000000 python-selve-new-2.1.8/selve/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-01 20:41:58.000000 python-selve-new-2.1.8/selve/iveo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-01 20:41:58.000000 python-selve-new-2.1.8/selve/senSim.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-01 20:41:58.000000 python-selve-new-2.1.8/selve/sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-01 20:41:58.000000 python-selve-new-2.1.8/selve/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:42:05.087584 python-selve-new-2.1.8/selve/util/
--rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-06-01 20:41:58.000000 python-selve-new-2.1.8/selve/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-01 20:41:58.000000 python-selve-new-2.1.8/selve/util/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-01 20:41:58.000000 python-selve-new-2.1.8/selve/util/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 20:42:05.087584 python-selve-new-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-01 20:41:58.000000 python-selve-new-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:25:48.202929 python-selve-new-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-01 21:25:48.202929 python-selve-new-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:25:48.198929 python-selve-new-2.1.9/python_selve_new.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-01 21:25:48.000000 python-selve-new-2.1.9/python_selve_new.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-01 21:25:48.000000 python-selve-new-2.1.9/python_selve_new.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 21:25:48.000000 python-selve-new-2.1.9/python_selve_new.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 21:25:48.000000 python-selve-new-2.1.9/python_selve_new.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-01 21:25:48.000000 python-selve-new-2.1.9/python_selve_new.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:25:48.198929 python-selve-new-2.1.9/selve/
+-rw-r--r--   0 runner    (1001) docker     (123)    50814 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:25:48.202929 python-selve-new-2.1.9/selve/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/commands/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/commands/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/commands/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/commands/iveo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/commands/param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/commands/senSim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/commands/sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/commands/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/commands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/iveo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/senSim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:25:48.202929 python-selve-new-2.1.9/selve/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/util/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/util/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 21:25:48.202929 python-selve-new-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/setup.py
```

### Comparing `python-selve-new-2.1.8/LICENSE` & `python-selve-new-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.8/PKG-INFO` & `python-selve-new-2.1.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-selve-new
-Version: 2.1.8
+Version: 2.1.9
 Summary: Python library for interfacing with selve devices using the USB-RF controller. Written completely new.
 Home-page: https://github.com/Kannix2005/python-selve-new
 Author: Stefan Altheimer
 Author-email: me@stefan-altheimer.de
 Keywords: selve blind awning shutter usb rf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
```

### Comparing `python-selve-new-2.1.8/python_selve_new.egg-info/PKG-INFO` & `python-selve-new-2.1.9/python_selve_new.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-selve-new
-Version: 2.1.8
+Version: 2.1.9
 Summary: Python library for interfacing with selve devices using the USB-RF controller. Written completely new.
 Home-page: https://github.com/Kannix2005/python-selve-new
 Author: Stefan Altheimer
 Author-email: me@stefan-altheimer.de
 Keywords: selve blind awning shutter usb rf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
```

### Comparing `python-selve-new-2.1.8/python_selve_new.egg-info/SOURCES.txt` & `python-selve-new-2.1.9/python_selve_new.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.8/selve/__init__.py` & `python-selve-new-2.1.9/selve/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
                                     self._serial.flush()
                             except Exception as e:
                                 self._LOGGER.error("error communicating: " + str(e))
 
                             self.txQ.task_done()
 
                             # always sleep after writing
-                            await asyncio.sleep(1)
+                            await asyncio.sleep(0.2)
                     else:
                         self._LOGGER.debug("Writer stopped")
                 await asyncio.sleep(0.01)
                 if self._stopThread:
                     self._LOGGER.debug('Exiting worker loop...')
                     break
             return True
@@ -218,16 +218,19 @@
 
     async def stopWorker(self):
         self._LOGGER.debug("Stopping worker")
         self._pauseReader = True
         self._pauseWriter = True
         self._pauseWorker = True
         self._stopThread = True
-        if self.workerTask is not None and not self.workerTask.cancelled() and not self.workerTask.done():
-            await self.workerTask
+        try:
+            if self.workerTask is not None and not self.workerTask.cancelled() and not self.workerTask.done():
+                await asyncio.wait_for(self.workerTask, timeout=5)
+        except Exception as e:
+            self._LOGGER.debug("Task stopping exception: " + str(e))
         self.workerTask = None
 
 
     async def stopGateway(self):
         # wait for the rx/tx thread to end, these need to be gathered to
         # collect all the exceptions
         self._LOGGER.debug("Preparing for termination")
@@ -255,15 +258,15 @@
         try:
             async with self._writeLock:
                 if not self._serial.is_open:
                     self._serial.open()
                 self._serial.write(commandstr)
                 self._serial.flush()
                 # always sleep after writing
-                await asyncio.sleep(1)
+                await asyncio.sleep(0.2)
         except Exception as e:
             self._LOGGER.error("error communicating: " + str(e))
 
     async def processResponse(self, xmlstr):
         """Processes an XML String into a response object. Returns False if something went wrong or the gateway returned an error."""
         # check which command was received
         # do something with the data
```

### Comparing `python-selve-new-2.1.8/selve/commands/command.py` & `python-selve-new-2.1.9/selve/commands/command.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.8/selve/commands/device.py` & `python-selve-new-2.1.9/selve/commands/device.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.8/selve/commands/event.py` & `python-selve-new-2.1.9/selve/commands/event.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.8/selve/commands/group.py` & `python-selve-new-2.1.9/selve/commands/group.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.8/selve/commands/iveo.py` & `python-selve-new-2.1.9/selve/commands/iveo.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.8/selve/commands/param.py` & `python-selve-new-2.1.9/selve/commands/param.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.8/selve/commands/senSim.py` & `python-selve-new-2.1.9/selve/commands/senSim.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.8/selve/commands/sender.py` & `python-selve-new-2.1.9/selve/commands/sender.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.8/selve/commands/sensor.py` & `python-selve-new-2.1.9/selve/commands/sensor.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.8/selve/commands/service.py` & `python-selve-new-2.1.9/selve/commands/service.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.8/selve/device.py` & `python-selve-new-2.1.9/selve/device.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.8/selve/group.py` & `python-selve-new-2.1.9/selve/group.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.8/selve/iveo.py` & `python-selve-new-2.1.9/selve/iveo.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.8/selve/senSim.py` & `python-selve-new-2.1.9/selve/senSim.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.8/selve/sender.py` & `python-selve-new-2.1.9/selve/sender.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.8/selve/sensor.py` & `python-selve-new-2.1.9/selve/sensor.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.8/selve/util/__init__.py` & `python-selve-new-2.1.9/selve/util/__init__.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.8/selve/util/errors.py` & `python-selve-new-2.1.9/selve/util/errors.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.8/selve/util/protocol.py` & `python-selve-new-2.1.9/selve/util/protocol.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.8/setup.py` & `python-selve-new-2.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     
     name='python-selve-new',  # Required    
-    version='2.1.8',  # Required
+    version='2.1.9',  # Required
     description='Python library for interfacing with selve devices using the USB-RF controller. Written completely new.',  # Required   
     long_description=long_description,  # Optional 
     long_description_content_type="text/markdown",   
     url='https://github.com/Kannix2005/python-selve-new',  # Optional
     author='Stefan Altheimer',  # Optional
    
     author_email='me@stefan-altheimer.de',  # Optional
```

