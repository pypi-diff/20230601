# Comparing `tmp/python-selve-new-2.1.2.tar.gz` & `tmp/python-selve-new-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-selve-new-2.1.2.tar", last modified: Thu Jun  1 18:33:04 2023, max compression
+gzip compressed data, was "python-selve-new-2.1.3.tar", last modified: Thu Jun  1 18:44:03 2023, max compression
```

## Comparing `python-selve-new-2.1.2.tar` & `python-selve-new-2.1.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:33:04.522957 python-selve-new-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-01 18:32:59.000000 python-selve-new-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-01 18:33:04.522957 python-selve-new-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-01 18:32:59.000000 python-selve-new-2.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:33:04.522957 python-selve-new-2.1.2/python_selve_new.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-01 18:33:04.000000 python-selve-new-2.1.2/python_selve_new.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-01 18:33:04.000000 python-selve-new-2.1.2/python_selve_new.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 18:33:04.000000 python-selve-new-2.1.2/python_selve_new.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 18:33:04.000000 python-selve-new-2.1.2/python_selve_new.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-01 18:33:04.000000 python-selve-new-2.1.2/python_selve_new.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:33:04.522957 python-selve-new-2.1.2/selve/
--rw-r--r--   0 runner    (1001) docker     (123)    50891 2023-06-01 18:32:59.000000 python-selve-new-2.1.2/selve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:33:04.522957 python-selve-new-2.1.2/selve/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:32:59.000000 python-selve-new-2.1.2/selve/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-06-01 18:32:59.000000 python-selve-new-2.1.2/selve/commands/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-06-01 18:32:59.000000 python-selve-new-2.1.2/selve/commands/device.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-01 18:32:59.000000 python-selve-new-2.1.2/selve/commands/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-01 18:32:59.000000 python-selve-new-2.1.2/selve/commands/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-01 18:32:59.000000 python-selve-new-2.1.2/selve/commands/iveo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-01 18:32:59.000000 python-selve-new-2.1.2/selve/commands/param.py
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-01 18:32:59.000000 python-selve-new-2.1.2/selve/commands/senSim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-06-01 18:32:59.000000 python-selve-new-2.1.2/selve/commands/sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-06-01 18:32:59.000000 python-selve-new-2.1.2/selve/commands/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-01 18:32:59.000000 python-selve-new-2.1.2/selve/commands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-01 18:32:59.000000 python-selve-new-2.1.2/selve/device.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:32:59.000000 python-selve-new-2.1.2/selve/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-01 18:32:59.000000 python-selve-new-2.1.2/selve/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-01 18:32:59.000000 python-selve-new-2.1.2/selve/iveo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-01 18:32:59.000000 python-selve-new-2.1.2/selve/senSim.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-01 18:32:59.000000 python-selve-new-2.1.2/selve/sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-01 18:32:59.000000 python-selve-new-2.1.2/selve/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:33:04.522957 python-selve-new-2.1.2/selve/util/
--rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-06-01 18:32:59.000000 python-selve-new-2.1.2/selve/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-01 18:32:59.000000 python-selve-new-2.1.2/selve/util/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-01 18:32:59.000000 python-selve-new-2.1.2/selve/util/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 18:33:04.522957 python-selve-new-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-01 18:32:59.000000 python-selve-new-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:44:03.701396 python-selve-new-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-01 18:43:50.000000 python-selve-new-2.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-01 18:44:03.701396 python-selve-new-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-01 18:43:50.000000 python-selve-new-2.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:44:03.697395 python-selve-new-2.1.3/python_selve_new.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-01 18:44:03.000000 python-selve-new-2.1.3/python_selve_new.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-01 18:44:03.000000 python-selve-new-2.1.3/python_selve_new.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 18:44:03.000000 python-selve-new-2.1.3/python_selve_new.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 18:44:03.000000 python-selve-new-2.1.3/python_selve_new.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-01 18:44:03.000000 python-selve-new-2.1.3/python_selve_new.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:44:03.697395 python-selve-new-2.1.3/selve/
+-rw-r--r--   0 runner    (1001) docker     (123)    50863 2023-06-01 18:43:50.000000 python-selve-new-2.1.3/selve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:44:03.701396 python-selve-new-2.1.3/selve/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:43:50.000000 python-selve-new-2.1.3/selve/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-06-01 18:43:50.000000 python-selve-new-2.1.3/selve/commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-06-01 18:43:50.000000 python-selve-new-2.1.3/selve/commands/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-01 18:43:50.000000 python-selve-new-2.1.3/selve/commands/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-01 18:43:50.000000 python-selve-new-2.1.3/selve/commands/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-01 18:43:50.000000 python-selve-new-2.1.3/selve/commands/iveo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-01 18:43:50.000000 python-selve-new-2.1.3/selve/commands/param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-01 18:43:50.000000 python-selve-new-2.1.3/selve/commands/senSim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-06-01 18:43:50.000000 python-selve-new-2.1.3/selve/commands/sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-06-01 18:43:50.000000 python-selve-new-2.1.3/selve/commands/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-01 18:43:50.000000 python-selve-new-2.1.3/selve/commands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-01 18:43:50.000000 python-selve-new-2.1.3/selve/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:43:50.000000 python-selve-new-2.1.3/selve/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-01 18:43:50.000000 python-selve-new-2.1.3/selve/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-01 18:43:50.000000 python-selve-new-2.1.3/selve/iveo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-01 18:43:50.000000 python-selve-new-2.1.3/selve/senSim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-01 18:43:50.000000 python-selve-new-2.1.3/selve/sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-01 18:43:50.000000 python-selve-new-2.1.3/selve/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:44:03.701396 python-selve-new-2.1.3/selve/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-06-01 18:43:50.000000 python-selve-new-2.1.3/selve/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-01 18:43:50.000000 python-selve-new-2.1.3/selve/util/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-01 18:43:50.000000 python-selve-new-2.1.3/selve/util/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 18:44:03.701396 python-selve-new-2.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-01 18:43:50.000000 python-selve-new-2.1.3/setup.py
```

### Comparing `python-selve-new-2.1.2/LICENSE` & `python-selve-new-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.2/PKG-INFO` & `python-selve-new-2.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-selve-new
-Version: 2.1.2
+Version: 2.1.3
 Summary: Python library for interfacing with selve devices using the USB-RF controller. Written completely new.
 Home-page: https://github.com/Kannix2005/python-selve-new
 Author: Stefan Altheimer
 Author-email: me@stefan-altheimer.de
 Keywords: selve blind awning shutter usb rf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
```

### Comparing `python-selve-new-2.1.2/python_selve_new.egg-info/PKG-INFO` & `python-selve-new-2.1.3/python_selve_new.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-selve-new
-Version: 2.1.2
+Version: 2.1.3
 Summary: Python library for interfacing with selve devices using the USB-RF controller. Written completely new.
 Home-page: https://github.com/Kannix2005/python-selve-new
 Author: Stefan Altheimer
 Author-email: me@stefan-altheimer.de
 Keywords: selve blind awning shutter usb rf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
```

### Comparing `python-selve-new-2.1.2/python_selve_new.egg-info/SOURCES.txt` & `python-selve-new-2.1.3/python_selve_new.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.2/selve/__init__.py` & `python-selve-new-2.1.3/selve/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -580,21 +580,21 @@
                         return False
                     
                     if isinstance(resp, ErrorResponse):
                         self._LOGGER.error(resp.message)
                         # retry
                         return False
 
-                        return resp
-                    # When no data is waiting in the input buffer after 10s we can assume, the message was not correctly sent or no input is necessary
-                    if time.time() - start_time < 10:
-                        time.sleep(0.05)
-                    else:
-                        await self.startWorker()
-                        return False
+                    return resp
+                # When no data is waiting in the input buffer after 10s we can assume, the message was not correctly sent or no input is necessary
+                if time.time() - start_time < 10:
+                    time.sleep(0.05)
+                else:
+                    await self.startWorker()
+                    return False
         
 
 
     async def discover(self):
 
         self._pauseWorker = True
```

### Comparing `python-selve-new-2.1.2/selve/commands/command.py` & `python-selve-new-2.1.3/selve/commands/command.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.2/selve/commands/device.py` & `python-selve-new-2.1.3/selve/commands/device.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.2/selve/commands/event.py` & `python-selve-new-2.1.3/selve/commands/event.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.2/selve/commands/group.py` & `python-selve-new-2.1.3/selve/commands/group.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.2/selve/commands/iveo.py` & `python-selve-new-2.1.3/selve/commands/iveo.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.2/selve/commands/param.py` & `python-selve-new-2.1.3/selve/commands/param.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.2/selve/commands/senSim.py` & `python-selve-new-2.1.3/selve/commands/senSim.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.2/selve/commands/sender.py` & `python-selve-new-2.1.3/selve/commands/sender.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.2/selve/commands/sensor.py` & `python-selve-new-2.1.3/selve/commands/sensor.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.2/selve/commands/service.py` & `python-selve-new-2.1.3/selve/commands/service.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.2/selve/device.py` & `python-selve-new-2.1.3/selve/device.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.2/selve/group.py` & `python-selve-new-2.1.3/selve/group.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.2/selve/iveo.py` & `python-selve-new-2.1.3/selve/iveo.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.2/selve/senSim.py` & `python-selve-new-2.1.3/selve/senSim.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.2/selve/sender.py` & `python-selve-new-2.1.3/selve/sender.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.2/selve/sensor.py` & `python-selve-new-2.1.3/selve/sensor.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.2/selve/util/__init__.py` & `python-selve-new-2.1.3/selve/util/__init__.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.2/selve/util/errors.py` & `python-selve-new-2.1.3/selve/util/errors.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.2/selve/util/protocol.py` & `python-selve-new-2.1.3/selve/util/protocol.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.2/setup.py` & `python-selve-new-2.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     
     name='python-selve-new',  # Required    
-    version='2.1.2',  # Required
+    version='2.1.3',  # Required
     description='Python library for interfacing with selve devices using the USB-RF controller. Written completely new.',  # Required   
     long_description=long_description,  # Optional 
     long_description_content_type="text/markdown",   
     url='https://github.com/Kannix2005/python-selve-new',  # Optional
     author='Stefan Altheimer',  # Optional
    
     author_email='me@stefan-altheimer.de',  # Optional
```

