# Comparing `tmp/piwwwaterflow-0.1.6.tar.gz` & `tmp/piwwwaterflow-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piwwwaterflow-0.1.6.tar", last modified: Fri May 26 12:01:48 2023, max compression
+gzip compressed data, was "piwwwaterflow-0.1.7.tar", last modified: Thu Jun  1 12:06:22 2023, max compression
```

## Comparing `piwwwaterflow-0.1.6.tar` & `piwwwaterflow-0.1.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:01:48.303708 piwwwaterflow-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-26 12:01:48.303708 piwwwaterflow-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:01:48.299708 piwwwaterflow-0.1.6/piwwwaterflow/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:01:48.303708 piwwwaterflow-0.1.6/piwwwaterflow/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:01:48.303708 piwwwaterflow-0.1.6/piwwwaterflow/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/static/css/iepngfix.htc
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/static/css/view.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:01:48.303708 piwwwaterflow-0.1.6/piwwwaterflow/static/img/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/static/img/blank.gif
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/static/img/bottom.png
--rw-r--r--   0 runner    (1001) docker     (123)    33683 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/static/img/icon-256.png
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/static/img/icon-32.png
--rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/static/img/piwaterflow.svg
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/static/img/play.png
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/static/img/shadow.gif
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/static/img/top.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:01:48.303708 piwwwaterflow-0.1.6/piwwwaterflow/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/static/js/code.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:01:48.303708 piwwwaterflow-0.1.6/piwwwaterflow/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/templates/form.html
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/webservice.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:01:48.303708 piwwwaterflow-0.1.6/piwwwaterflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-26 12:01:48.000000 piwwwaterflow-0.1.6/piwwwaterflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 12:01:48.000000 piwwwaterflow-0.1.6/piwwwaterflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:01:48.000000 piwwwaterflow-0.1.6/piwwwaterflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-26 12:01:48.000000 piwwwaterflow-0.1.6/piwwwaterflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-26 12:01:48.000000 piwwwaterflow-0.1.6/piwwwaterflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 12:01:48.303708 piwwwaterflow-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:01:48.303708 piwwwaterflow-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:06:22.849887 piwwwaterflow-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-01 12:06:22.849887 piwwwaterflow-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:06:22.845886 piwwwaterflow-0.1.7/piwwwaterflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:06:22.845886 piwwwaterflow-0.1.7/piwwwaterflow/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:06:22.849887 piwwwaterflow-0.1.7/piwwwaterflow/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/static/css/iepngfix.htc
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/static/css/view.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:06:22.849887 piwwwaterflow-0.1.7/piwwwaterflow/static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/static/img/blank.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/static/img/bottom.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33683 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/static/img/icon-256.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/static/img/icon-32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/static/img/piwaterflow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/static/img/play.png
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/static/img/shadow.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/static/img/top.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:06:22.849887 piwwwaterflow-0.1.7/piwwwaterflow/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/static/js/code.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:06:22.849887 piwwwaterflow-0.1.7/piwwwaterflow/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/templates/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/webservice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:06:22.845886 piwwwaterflow-0.1.7/piwwwaterflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-01 12:06:22.000000 piwwwaterflow-0.1.7/piwwwaterflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-01 12:06:22.000000 piwwwaterflow-0.1.7/piwwwaterflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 12:06:22.000000 piwwwaterflow-0.1.7/piwwwaterflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-01 12:06:22.000000 piwwwaterflow-0.1.7/piwwwaterflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-01 12:06:22.000000 piwwwaterflow-0.1.7/piwwwaterflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 12:06:22.849887 piwwwaterflow-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:06:22.849887 piwwwaterflow-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/tests/__init__.py
```

### Comparing `piwwwaterflow-0.1.6/PKG-INFO` & `piwwwaterflow-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwwwaterflow
-Version: 0.1.6
+Version: 0.1.7
 Summary: Raspberry Pi Waterflow resilient system
 Home-page: https://github.com/Phornee/piwwwaterflow
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # piwwwaterflow
         Flask/Gunicorn Webservice for piwaterflow system
```

### Comparing `piwwwaterflow-0.1.6/piwwwaterflow/static/css/iepngfix.htc` & `piwwwaterflow-0.1.7/piwwwaterflow/static/css/iepngfix.htc`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.6/piwwwaterflow/static/css/view.css` & `piwwwaterflow-0.1.7/piwwwaterflow/static/css/view.css`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.6/piwwwaterflow/static/img/icon-256.png` & `piwwwaterflow-0.1.7/piwwwaterflow/static/img/icon-256.png`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.6/piwwwaterflow/static/img/icon-32.png` & `piwwwaterflow-0.1.7/piwwwaterflow/static/img/icon-32.png`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.6/piwwwaterflow/static/img/piwaterflow.svg` & `piwwwaterflow-0.1.7/piwwwaterflow/static/img/piwaterflow.svg`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.6/piwwwaterflow/static/img/play.png` & `piwwwaterflow-0.1.7/piwwwaterflow/static/img/play.png`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.6/piwwwaterflow/static/js/code.js` & `piwwwaterflow-0.1.7/piwwwaterflow/static/js/code.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -2,14 +2,22 @@
 
 var socket = io();
 
 function _setEnableForceTriggers(enable) {
     forceTriggersEnabled = enable
 }
 
+function getProgramName(index) {
+    return document.getElementById('program' + (index + 1) + 'trigger').textContent
+}
+
+function getValveName(index) {
+    return document.getElementById('valve' + (index + 1) + 'trigger').textContent
+}
+
 function _resetForceTriggers() {
     document.getElementById('program1trigger').style.color = 'inherit';
     document.getElementById('program2trigger').style.color = 'inherit';
     document.getElementById('valve1trigger').style.color = 'inherit';
     document.getElementById('valve2trigger').style.color = 'inherit';
 }
 
@@ -172,39 +180,45 @@
         }
 
         // Controls update
         var configObj = response.config;
         if (configObj != null) {
             time1 = document.getElementById("time1");
             if (!time1.changed)
-                time1.value = configObj.programs["first"].start_time;
+                time1.value = configObj.programs[0].start_time;
             valve11 = document.getElementById("valve11");
             if (!valve11.changed)
-                valve11.value = configObj.programs["first"].valves_times['valve1']
+                valve11.value = configObj.programs[0].valves[0].time
             valve12 = document.getElementById("valve12");
             if (!valve12.changed)
-                valve12.value = configObj.programs["first"].valves_times['valve2']
+                valve12.value = configObj.programs[0].valves[1].time
             prog1enabled = document.getElementById("prog1enabled");
             if (!prog1enabled.changed)
-                prog1enabled.checked = configObj.programs["first"].enabled;
+                prog1enabled.checked = configObj.programs[0].enabled;
 
             time1 = document.getElementById("time2");
             if (!time1.changed)
-                time1.value = configObj.programs["second"].start_time;
+                time1.value = configObj.programs[1].start_time;
             valve21 = document.getElementById("valve21");
             if (!valve21.changed)
-                valve21.value = configObj.programs["second"].valves_times['valve1']
+                valve21.value = configObj.programs[1].valves[0].time
             valve22 = document.getElementById("valve22");
             if (!valve22.changed)
-                valve22.value = configObj.programs["second"].valves_times['valve2']
+                valve22.value = configObj.programs[1].valves[1].time
             prog2enabled = document.getElementById("prog2enabled");
             if (!prog2enabled.changed)
-                prog2enabled.checked = configObj.programs["second"].enabled;
+                prog2enabled.checked = configObj.programs[1].enabled;
 
             if (first_time) { // Get this value from the closure (parameter in update function)
+                // Set names of programs and valves
+                document.getElementById('program1trigger').textContent = configObj.programs[0].name;
+                document.getElementById('program2trigger').textContent = configObj.programs[1].name;
+                document.getElementById('valve1trigger').textContent = configObj.programs[0].valves[0].name;
+                document.getElementById('valve2trigger').textContent = configObj.programs[0].valves[1].name;
+
                 saveCurrentValues();
                 refreshSaveButton();
             }
         }
     });
 }
 
@@ -236,28 +250,37 @@
 
 function stopWaterflow(button) {
     socket.emit('stop');
     button.disabled = true;
 }
 
 function save(button) {
-    socket.emit('save', {
-        'prog1': {
-            'time': document.getElementById("time1").value,
-            'valve1': parseInt(document.getElementById("valve11").value),
-            'valve2': parseInt(document.getElementById("valve12").value),
-            'enabled': document.getElementById("prog1enabled").value
-        },
-        'prog2': {
-            'time': document.getElementById("time2").value,
-            'valve1': parseInt(document.getElementById("valve21").value),
-            'valve2': parseInt(document.getElementById("valve12").value),
-            'enabled': document.getElementById("prog2enabled").value
-        }
-    }, function ack(result) {
+    socket.emit('save', [{
+        'name': getProgramName(0),
+        'time': document.getElementById("time1").value,
+        'valves': [{
+            'name': getValveName(0),
+            'time': parseInt(document.getElementById("valve11").value)
+        }, {
+            'name': getValveName(1),
+            'time': parseInt(document.getElementById("valve12").value)
+        }, ],
+        'enabled': document.getElementById("prog1enabled").checked
+    }, {
+        'name': getProgramName(1),
+        'time': document.getElementById("time2").value,
+        'valves': [{
+            'name': getValveName(0),
+            'time': parseInt(document.getElementById("valve21").value)
+        }, {
+            'name': getValveName(1),
+            'time': parseInt(document.getElementById("valve22").value)
+        }, ],
+        'enabled': document.getElementById("prog2enabled").checked
+    }], function ack(result) {
         if (result) {
             saveCurrentValues();
             refreshSaveButton();
             button.disabled = true;
         }
     });
 }
```

### Comparing `piwwwaterflow-0.1.6/piwwwaterflow/templates/form.html` & `piwwwaterflow-0.1.7/piwwwaterflow/templates/form.html`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.6/piwwwaterflow/webservice.py` & `piwwwaterflow-0.1.7/piwwwaterflow/webservice.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,19 +58,19 @@
         except PackageNotFoundError:
             ver = '?.?.?'
 
         responsedict = {'log': self.waterflow.get_log(),
                         'forced': self.waterflow.get_forced_info(),
                         'stop': self.waterflow.stop_requested(),
                         'config': self._get_public_config(),
-                        'lastlooptime': self.waterflow.last_loop_time().strftime('%Y-%m-%dT%H:%M:%S.000Z'),
+                        'lastlooptime': self.waterflow.last_loop_time().strftime('%Y-%m-%dT%H:%M:%S'),
                         'version': ver
                         }
         # Change to string so that javascript can manage with it
-        for program in responsedict['config']['programs'].values():
+        for program in responsedict['config']['programs']:
             program['start_time'] = program['start_time'].strftime('%H:%M')
         return responsedict
 
     def on_force(self, data: dict):
         """ On force action request
         Args:
             data (dict): 'type': Must be 'valve' or 'program'
@@ -90,26 +90,26 @@
         """ Event to save the changes in the watering system schedulling
         Args:
             data (dict): Information about the required schedulling
         Returns:
             bool: If everything went ok
         """
         parsed_config = self.waterflow.config.get_dict_copy()
-        self._change_program(parsed_config['programs']['first'], data['prog1'])
-        self._change_program(parsed_config['programs']['second'], data['prog2'])
+        for program, update in zip(parsed_config['programs'], data):
+            self._change_program(program, update)
 
         self.waterflow.update_config(programs=parsed_config['programs'])
         return True
 
     def _get_public_config(self):
         config = self.waterflow.config.get_dict_copy()
         del config['influxdbconn']
         return config
 
     def _change_program(self, program, new_program):
         inputbox_text = new_program['time']
         time1 = datetime.strptime(inputbox_text, '%H:%M')
         new_datetime = program['start_time'].replace(hour=time1.hour, minute=time1.minute)
         program['start_time'] = new_datetime
-        program['valves_times']['valve1'] = new_program['valve1']
-        program['valves_times']['valve2'] = new_program['valve2']
-        program['enabled'] = new_program['enabled'] is not None
+        program['valves'][0] = new_program['valves'][0]
+        program['valves'][1] = new_program['valves'][1]
+        program['enabled'] = new_program['enabled']
```

### Comparing `piwwwaterflow-0.1.6/piwwwaterflow/wsgi.py` & `piwwwaterflow-0.1.7/piwwwaterflow/wsgi.py`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.6/piwwwaterflow.egg-info/PKG-INFO` & `piwwwaterflow-0.1.7/piwwwaterflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwwwaterflow
-Version: 0.1.6
+Version: 0.1.7
 Summary: Raspberry Pi Waterflow resilient system
 Home-page: https://github.com/Phornee/piwwwaterflow
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # piwwwaterflow
         Flask/Gunicorn Webservice for piwaterflow system
```

### Comparing `piwwwaterflow-0.1.6/piwwwaterflow.egg-info/SOURCES.txt` & `piwwwaterflow-0.1.7/piwwwaterflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.6/setup.py` & `piwwwaterflow-0.1.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="piwwwaterflow",
-    version="0.1.6",
+    version="0.1.7",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Raspberry Pi Waterflow resilient system",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/piwwwaterflow",
     packages=setuptools.find_packages(),
@@ -23,13 +23,13 @@
     ],
     install_requires=[
         'Flask>=1.1.2',
         'flask-compress>=1.9.0',
         'importlib-metadata>=4.5.0',
         'python-socketio>=5.8.0',
         'flask-socketio>=5.3.3',
-        'eventlet>=0.33.3',
-        'piwaterflow>=0.5.4',
+        'eventlet>=0.30.2',
+        'piwaterflow>=0.5.9',
         'revproxy_auth>=0.1.6'
     ],
     python_requires='>=3.6',
 )
```

