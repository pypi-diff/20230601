# Comparing `tmp/XPVI-0.0.3.tar.gz` & `tmp/XPVI-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\XPVI-0.0.3.tar", last modified: Thu Jun  1 03:21:42 2023, max compression
+gzip compressed data, was "dist\XPVI-0.0.4.tar", last modified: Thu Jun  1 03:28:06 2023, max compression
```

## Comparing `XPVI-0.0.3.tar` & `XPVI-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 03:21:42.755573 XPVI-0.0.3/
--rw-rw-rw-   0        0        0     3263 2023-06-01 03:21:42.754576 XPVI-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1806 2023-06-01 03:21:34.000000 XPVI-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 03:21:42.753580 XPVI-0.0.3/XPVI.egg-info/
--rw-rw-rw-   0        0        0     3263 2023-06-01 03:21:42.000000 XPVI-0.0.3/XPVI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      130 2023-06-01 03:21:42.000000 XPVI-0.0.3/XPVI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 03:21:42.000000 XPVI-0.0.3/XPVI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 03:21:42.000000 XPVI-0.0.3/XPVI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 03:21:42.755573 XPVI-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0    10220 2023-06-01 03:21:42.000000 XPVI-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 03:28:06.796168 XPVI-0.0.4/
+-rw-rw-rw-   0        0        0     3263 2023-06-01 03:28:06.795168 XPVI-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1806 2023-06-01 03:25:46.000000 XPVI-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 03:28:06.794169 XPVI-0.0.4/XPVI.egg-info/
+-rw-rw-rw-   0        0        0     3263 2023-06-01 03:28:06.000000 XPVI-0.0.4/XPVI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      130 2023-06-01 03:28:06.000000 XPVI-0.0.4/XPVI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 03:28:06.000000 XPVI-0.0.4/XPVI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 03:28:06.000000 XPVI-0.0.4/XPVI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 03:28:06.796168 XPVI-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0    10945 2023-06-01 03:28:06.000000 XPVI-0.0.4/setup.py
```

### Comparing `XPVI-0.0.3/PKG-INFO` & `XPVI-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: XPVI
-Version: 0.0.3
+Version: 0.0.4
 Summary: Get and save custom variables "to" a usb video device
 Home-page: UNKNOWN
 Author: Karrson Heumann
 Author-email: <mail@example.com>
 License: UNKNOWN
 Description: 
-        # XPVI (0.0.3)
+        # XPVI (0.0.4)
         
          Cross Platform Video Info
         
         Get and save custom system-wide variables "to" a usb video device or filepath.
         
         Also works with audio devices, very useful for saving calibration data.
```

### Comparing `XPVI-0.0.3/README.md` & `XPVI-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# XPVI (0.0.3)
+# XPVI (0.0.4)
 
  Cross Platform Video Info
 
 Get and save custom system-wide variables "to" a usb video device or filepath.
 
 Also works with audio devices, very useful for saving calibration data.
```

### Comparing `XPVI-0.0.3/XPVI.egg-info/PKG-INFO` & `XPVI-0.0.4/XPVI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: XPVI
-Version: 0.0.3
+Version: 0.0.4
 Summary: Get and save custom variables "to" a usb video device
 Home-page: UNKNOWN
 Author: Karrson Heumann
 Author-email: <mail@example.com>
 License: UNKNOWN
 Description: 
-        # XPVI (0.0.3)
+        # XPVI (0.0.4)
         
          Cross Platform Video Info
         
         Get and save custom system-wide variables "to" a usb video device or filepath.
         
         Also works with audio devices, very useful for saving calibration data.
```

### Comparing `XPVI-0.0.3/setup.py` & `XPVI-0.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,22 +4,40 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Get and save custom variables "to" a usb video device'
 LONG_DESCRIPTION = 'Cross Platform Video Info, \n' + \
 'Get and save custom system-wide variables "to" a usb video device or filepath, \n' + \
 'Also works with audio devices, very useful for saving calibration data, \n' + \
 'Can also get a device index from it\'s name and vice-versa'
 
 def install_package():
+    if os.path.exists(os.path.join(
+        os.path.abspath(os.path.join(sys.executable, os.pardir)
+    ), 'XPVI.py')):
+        os.remove(os.path.join(
+        os.path.abspath(os.path.join(sys.executable, os.pardir)
+    ), 'XPVI.py'))
+    if os.path.exists(os.path.join(
+        os.path.abspath(os.path.join(sys.executable, os.pardir)
+    ), 'XPVI.bat')):
+        os.remove(os.path.join(
+        os.path.abspath(os.path.join(sys.executable, os.pardir)
+    ), 'XPVI.bat'))
+    if os.path.exists(os.path.join(
+        os.path.abspath(os.path.join(sys.executable, os.pardir)
+    ), 'XPVI.sh')):
+        os.remove(os.path.join(
+        os.path.abspath(os.path.join(sys.executable, os.pardir)
+    ), 'XPVI.sh'))
     with open(os.path.join(
         os.path.abspath(os.path.join(sys.executable, os.pardir)
     ), 'XPVI.py'), 'w') as fp:
         fp.write('import os\nimport sys\nimport re\nfrom subprocess import Popen, PIPE, STDOUT\ntry:\n    from subprocess import CREATE_NO_WINDOW\nexcept:\n    CREATE_NO_WINDOW = None\n\nscripts_dir = os.path.dirname(\n    os.path.realpath(\n        sys.executable\n    )\n)\n\ndef __raw_video_device_data():\n    has_ffmpeg = True\n    try:\n        proc = Popen([\'ffmpeg\', \'-version\'],\n                     creationflags=CREATE_NO_WINDOW, stderr=STDOUT,\n                     stdout=PIPE)\n    except:\n        try:\n            proc = Popen([\'ffmpeg\', \'-version\'],\n                         stderr=STDOUT, stdout=PIPE)\n        except:\n            has_ffmpeg = False\n    if not has_ffmpeg:\n        raise RuntimeError(\'ffmpeg not found\')\n    formats = [\n        \'alsa\',\n        \'android_camera\',\n        \'avfoundation\',\n        \'bktr\',\n        \'decklink\',\n        \'dshow\',\n        \'fbdev\',\n        \'gdigrab\',\n        \'iec61883\',\n        \'jack\',\n        \'kmsgrab\',\n        \'lavfi\',\n        \'libcdio\',\n        \'libdc1394\',\n        \'openal\',\n        \'oss\',\n        \'pulse\',\n        \'sndio\',\n        \'video4linux2\',\n        \'v4l2\',\n        \'vfwcap\',\n        \'x11grab\',\n    ]\n    raw_video_device_data = \'\'\n    for fmt in formats:\n        try:\n            raw_video_device_data += Popen(\n                [\n                    \'ffmpeg\',\n                    \'-f\',\n                    fmt,\n                    \'-list_devices\',\n                    \'true\',\n                    \'-i\',\n                    \'x\'\n                ],\n                creationflags=CREATE_NO_WINDOW,\n                stderr=STDOUT, stdout=PIPE\n            ).communicate()[0].decode(\'utf-8\') + \'\\n\'\n        except:\n            raw_video_device_data += Popen(\n                [\n                    \'ffmpeg\',\n                    \'-f\',\n                    fmt,\n                    \'-list_devices\',\n                    \'true\',\n                    \'-i\',\n                    \'x\'\n                ],\n                stderr=STDOUT, stdout=PIPE\n            ).communicate()[0].decode(\'utf-8\') + \'\\n\'\n    return raw_video_device_data\n\ndef __find_devices(kind):\n    matches = re.findall(r\'"(.+)"\\s+\\(\' + kind + \'\\)\', __raw_video_device_data())\n    return matches\n\ndef get_all_video_devices():\n    return list(enumerate(__find_devices(\'video\')))\n\ndef get_all_audio_devices():\n    return list(enumerate(__find_devices(\'audio\')))\n\ndef get_id_from_video_device(name):\n    ID = -1\n    for device in get_all_video_devices():\n        if device[1] == name:\n            ID = device[0]\n            break\n    return ID\n\ndef get_id_from_audio_device(name):\n    ID = -1\n    for device in get_all_audio_devices():\n        if device[1] == name:\n            ID = device[0]\n            break\n    return ID\n\ndef get_video_device_from_id(ID):\n    name = ""\n    for device in get_all_video_devices():\n        if device[0] == ID:\n            name = device[1]\n            break\n    return name\n\ndef get_audio_device_from_id(ID):\n    name = ""\n    for device in get_all_audio_devices():\n        if device[0] == ID:\n            name = device[1]\n            break\n    return name\n\nglobal env\nenv = {}\n\ndef save_env():\n    global env\n    if os.path.exists(os.path.join(scripts_dir, \'XPVI.env\')):\n        os.remove(os.path.join(scripts_dir, \'XPVI.env\'))\n    with open(os.path.join(scripts_dir, \'XPVI.env\'), \'w\') as fp:\n        fp.write(str(env))\n\ndef load_env():\n    global env\n    if not os.path.exists(os.path.join(scripts_dir, \'XPVI.env\')):\n        save_env()\n    with open(os.path.join(scripts_dir, \'XPVI.env\'), \'r\') as fp:\n        env = eval(fp.read())\n\nload_env()\n\nif __name__ == \'__main__\':\n    __raw_video_device_data()\n    if len(sys.argv) == 2 and sys.argv[1] == \'v*\':\n        print(get_all_video_devices())\n    elif len(sys.argv) == 2 and sys.argv[1] == \'a*\':\n        print(get_all_audio_devices())\n    elif len(sys.argv) == 3 and sys.argv[1] == \'v2i\':\n        if os.path.exists(sys.argv[2]):\n            print(sys.argv[2])\n        else:\n            print(str(get_id_from_video_device(sys.argv[2])))\n    elif len(sys.argv) == 3 and sys.argv[1] == \'a2i\':\n        if os.path.exists(sys.argv[2]):\n            print(sys.argv[2])\n        else:\n            print(str(get_id_from_audio_device(sys.argv[2])))\n    elif len(sys.argv) == 3 and sys.argv[1] == \'i2v\':\n        if os.path.exists(sys.argv[2]):\n            print(sys.argv[2])\n        else:\n            try:\n                print(get_video_device_from_id(int(sys.argv[2])))\n            except:\n                pass\n    elif len(sys.argv) == 3 and sys.argv[1] == \'i2a\':\n        if os.path.exists(sys.argv[2]):\n            print(sys.argv[2])\n        else:\n            try:\n                print(get_audio_device_from_id(int(sys.argv[2])))\n            except:\n                pass\n    elif len(sys.argv) == 5 and sys.argv[1] == \'set\':\n        ID = str(get_id_from_video_device(sys.argv[2]))\n        if os.path.exists(sys.argv[2]):\n            ID = sys.argv[2]\n        if ID == \'-1\':\n            ID = str(get_id_from_audio_device(sys.argv[2]))\n        if ID == \'-1\':\n            print(\'Error@DeviceName\')\n        elif sys.argv[3] is None or len(sys.argv[3]) == 0:\n            print(\'Error@Key\')\n        elif str(sys.argv[4]) == \'NULL\':\n            env.pop(sys.argv[2] + \'\\\\\' + sys.argv[3])\n            save_env()\n        else:\n            env[sys.argv[2] + \'\\\\\' + sys.argv[3]] = str(sys.argv[4])\n            save_env()\n    elif len(sys.argv) == 4 and sys.argv[1] == \'get\':\n        ID = str(get_id_from_video_device(sys.argv[2]))\n        if os.path.exists(sys.argv[2]):\n            ID = sys.argv[2]\n        if ID == \'-1\':\n            ID = str(get_id_from_audio_device(sys.argv[2]))\n        if ID == \'-1\':\n            print(\'Error@DeviceName\')\n        elif sys.argv[3] is None or len(sys.argv[3]) == 0:\n            print(\'Error@Key\')\n        else:\n            load_env()\n            if sys.argv[3] == \'ALL\':\n                tmp1 = [k for k in env if k.startswith(sys.argv[2] + \'\\\\\')]\n                tmp2 = {}\n                for tmp in tmp1:\n                    tmp2[tmp] = env[tmp]\n                print(str(tmp2))\n            else:\n                print(str(env[sys.argv[2] + \'\\\\\' + sys.argv[3]]))\n    else:\n        print(\'syntax:\')\n        print(\'v* (get_all_video_devices)\')\n        print(\'a* (get_all_audio_devices)\')\n        print(\'v2i name (get_id_from_video_device)\')\n        print(\'a2i name (get_id_from_audio_device)\')\n        print(\'i2v id (get_video_device_from_id)\')\n        print(\'i2a id (get_audio_device_from_id)\')\n        print(\'set name key value (set_value)\')\n        print(\'set name key "NULL" (delete_key)\')\n        print(\'get name key (get_value)\')\n        print(\'get name "ALL" (get_values)\')\nelse:\n    print("Error: Apps should use the XPVI cli")\n')
     with open(os.path.join(
         os.path.abspath(os.path.join(sys.executable, os.pardir)
     ), 'XPVI.bat'), 'w', newline='\r\n') as fp:
```

