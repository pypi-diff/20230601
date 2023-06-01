# Comparing `tmp/python-selve-new-2.1.0.tar.gz` & `tmp/python-selve-new-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-selve-new-2.1.0.tar", last modified: Thu Jun  1 17:30:11 2023, max compression
+gzip compressed data, was "python-selve-new-2.1.1.tar", last modified: Thu Jun  1 18:06:35 2023, max compression
```

## Comparing `python-selve-new-2.1.0.tar` & `python-selve-new-2.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:30:11.431332 python-selve-new-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-01 17:30:11.431332 python-selve-new-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:30:11.431332 python-selve-new-2.1.0/python_selve_new.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-01 17:30:11.000000 python-selve-new-2.1.0/python_selve_new.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-01 17:30:11.000000 python-selve-new-2.1.0/python_selve_new.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 17:30:11.000000 python-selve-new-2.1.0/python_selve_new.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 17:30:11.000000 python-selve-new-2.1.0/python_selve_new.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-01 17:30:11.000000 python-selve-new-2.1.0/python_selve_new.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:30:11.431332 python-selve-new-2.1.0/selve/
--rw-r--r--   0 runner    (1001) docker     (123)    50840 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:30:11.431332 python-selve-new-2.1.0/selve/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/commands/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/commands/device.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/commands/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/commands/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/commands/iveo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/commands/param.py
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/commands/senSim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/commands/sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/commands/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/commands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/device.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/iveo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/senSim.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:30:11.431332 python-selve-new-2.1.0/selve/util/
--rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/util/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/selve/util/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 17:30:11.431332 python-selve-new-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-01 17:30:04.000000 python-selve-new-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:06:35.227110 python-selve-new-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-01 18:06:31.000000 python-selve-new-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-01 18:06:35.227110 python-selve-new-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-01 18:06:31.000000 python-selve-new-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:06:35.223109 python-selve-new-2.1.1/python_selve_new.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-01 18:06:35.000000 python-selve-new-2.1.1/python_selve_new.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-01 18:06:35.000000 python-selve-new-2.1.1/python_selve_new.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 18:06:35.000000 python-selve-new-2.1.1/python_selve_new.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 18:06:35.000000 python-selve-new-2.1.1/python_selve_new.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-01 18:06:35.000000 python-selve-new-2.1.1/python_selve_new.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:06:35.223109 python-selve-new-2.1.1/selve/
+-rw-r--r--   0 runner    (1001) docker     (123)    50846 2023-06-01 18:06:31.000000 python-selve-new-2.1.1/selve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:06:35.227110 python-selve-new-2.1.1/selve/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:06:31.000000 python-selve-new-2.1.1/selve/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-06-01 18:06:31.000000 python-selve-new-2.1.1/selve/commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-06-01 18:06:31.000000 python-selve-new-2.1.1/selve/commands/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-01 18:06:31.000000 python-selve-new-2.1.1/selve/commands/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-01 18:06:31.000000 python-selve-new-2.1.1/selve/commands/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-01 18:06:31.000000 python-selve-new-2.1.1/selve/commands/iveo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-01 18:06:31.000000 python-selve-new-2.1.1/selve/commands/param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-01 18:06:31.000000 python-selve-new-2.1.1/selve/commands/senSim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-06-01 18:06:31.000000 python-selve-new-2.1.1/selve/commands/sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-06-01 18:06:31.000000 python-selve-new-2.1.1/selve/commands/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-01 18:06:31.000000 python-selve-new-2.1.1/selve/commands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-01 18:06:31.000000 python-selve-new-2.1.1/selve/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:06:31.000000 python-selve-new-2.1.1/selve/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-01 18:06:31.000000 python-selve-new-2.1.1/selve/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-01 18:06:31.000000 python-selve-new-2.1.1/selve/iveo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-01 18:06:31.000000 python-selve-new-2.1.1/selve/senSim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-01 18:06:31.000000 python-selve-new-2.1.1/selve/sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-01 18:06:31.000000 python-selve-new-2.1.1/selve/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:06:35.227110 python-selve-new-2.1.1/selve/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-06-01 18:06:31.000000 python-selve-new-2.1.1/selve/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-01 18:06:31.000000 python-selve-new-2.1.1/selve/util/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-01 18:06:31.000000 python-selve-new-2.1.1/selve/util/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 18:06:35.227110 python-selve-new-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-01 18:06:31.000000 python-selve-new-2.1.1/setup.py
```

### Comparing `python-selve-new-2.1.0/LICENSE` & `python-selve-new-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.0/PKG-INFO` & `python-selve-new-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-selve-new
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python library for interfacing with selve devices using the USB-RF controller. Written completely new.
 Home-page: https://github.com/Kannix2005/python-selve-new
 Author: Stefan Altheimer
 Author-email: me@stefan-altheimer.de
 Keywords: selve blind awning shutter usb rf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
```

### Comparing `python-selve-new-2.1.0/python_selve_new.egg-info/PKG-INFO` & `python-selve-new-2.1.1/python_selve_new.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-selve-new
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python library for interfacing with selve devices using the USB-RF controller. Written completely new.
 Home-page: https://github.com/Kannix2005/python-selve-new
 Author: Stefan Altheimer
 Author-email: me@stefan-altheimer.de
 Keywords: selve blind awning shutter usb rf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
```

### Comparing `python-selve-new-2.1.0/python_selve_new.egg-info/SOURCES.txt` & `python-selve-new-2.1.1/python_selve_new.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.0/selve/__init__.py` & `python-selve-new-2.1.1/selve/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -557,15 +557,15 @@
         #self._serial.reset_input_buffer()
         #self._serial.reset_output_buffer()
 
         await self._sendCommandToGateway(command)
 
         start_time = time.time()
         while True:
-            with self._readLock:
+            async with self._readLock:
                 if self._serial.in_waiting > 0:
                     msg = ""
                     while True:
                         response = self._serial.readline().strip()
                         msg += response.decode()
                         if response.decode() == '':
                             break
```

### Comparing `python-selve-new-2.1.0/selve/commands/command.py` & `python-selve-new-2.1.1/selve/commands/command.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.0/selve/commands/device.py` & `python-selve-new-2.1.1/selve/commands/device.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.0/selve/commands/event.py` & `python-selve-new-2.1.1/selve/commands/event.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.0/selve/commands/group.py` & `python-selve-new-2.1.1/selve/commands/group.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.0/selve/commands/iveo.py` & `python-selve-new-2.1.1/selve/commands/iveo.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.0/selve/commands/param.py` & `python-selve-new-2.1.1/selve/commands/param.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.0/selve/commands/senSim.py` & `python-selve-new-2.1.1/selve/commands/senSim.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.0/selve/commands/sender.py` & `python-selve-new-2.1.1/selve/commands/sender.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.0/selve/commands/sensor.py` & `python-selve-new-2.1.1/selve/commands/sensor.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.0/selve/commands/service.py` & `python-selve-new-2.1.1/selve/commands/service.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.0/selve/device.py` & `python-selve-new-2.1.1/selve/device.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.0/selve/group.py` & `python-selve-new-2.1.1/selve/group.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.0/selve/iveo.py` & `python-selve-new-2.1.1/selve/iveo.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.0/selve/senSim.py` & `python-selve-new-2.1.1/selve/senSim.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.0/selve/sender.py` & `python-selve-new-2.1.1/selve/sender.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.0/selve/sensor.py` & `python-selve-new-2.1.1/selve/sensor.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.0/selve/util/__init__.py` & `python-selve-new-2.1.1/selve/util/__init__.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.0/selve/util/errors.py` & `python-selve-new-2.1.1/selve/util/errors.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.0/selve/util/protocol.py` & `python-selve-new-2.1.1/selve/util/protocol.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.0/setup.py` & `python-selve-new-2.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     
     name='python-selve-new',  # Required    
-    version='2.1.0',  # Required
+    version='2.1.1',  # Required
     description='Python library for interfacing with selve devices using the USB-RF controller. Written completely new.',  # Required   
     long_description=long_description,  # Optional 
     long_description_content_type="text/markdown",   
     url='https://github.com/Kannix2005/python-selve-new',  # Optional
     author='Stefan Altheimer',  # Optional
    
     author_email='me@stefan-altheimer.de',  # Optional
```

