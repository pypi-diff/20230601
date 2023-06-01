# Comparing `tmp/PyHarshit-0.0.6.tar.gz` & `tmp/PyHarshit-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyHarshit-0.0.6.tar", last modified: Wed May 31 08:41:37 2023, max compression
+gzip compressed data, was "PyHarshit-0.0.7.tar", last modified: Thu Jun  1 15:13:59 2023, max compression
```

## Comparing `PyHarshit-0.0.6.tar` & `PyHarshit-0.0.7.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-05-31 08:41:37.174084 PyHarshit-0.0.6/
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      778 2023-05-31 08:41:37.174084 PyHarshit-0.0.6/PKG-INFO
-drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-05-31 08:41:37.170084 PyHarshit-0.0.6/PyHarshit/
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        1 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/PyHarshit/__init__.py
-drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-05-31 08:41:37.170084 PyHarshit-0.0.6/PyHarshit/tg/
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)    12360 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/PyHarshit/tg/FasterTg.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        1 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/PyHarshit/tg/__init__.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)     3009 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/PyHarshit/tg/extractor.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)     4125 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/PyHarshit/tg/tgControl.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)     1354 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/PyHarshit/tg/tgFunctions.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      478 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/PyHarshit/tg/tools.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)     2761 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/PyHarshit/tg/uploader.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      174 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/PyHarshit/tg/utils.py
-drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-05-31 08:41:37.174084 PyHarshit-0.0.6/PyHarshit/tools/
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        1 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/PyHarshit/tools/__init__.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      173 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/PyHarshit/tools/anim.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)       19 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/PyHarshit/tools/boolset.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      106 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/PyHarshit/tools/charset.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      313 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/PyHarshit/tools/maths.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      887 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/PyHarshit/tools/utils.py
-drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-05-31 08:41:37.170084 PyHarshit-0.0.6/PyHarshit.egg-info/
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      778 2023-05-31 08:41:37.000000 PyHarshit-0.0.6/PyHarshit.egg-info/PKG-INFO
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      559 2023-05-31 08:41:37.000000 PyHarshit-0.0.6/PyHarshit.egg-info/SOURCES.txt
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        1 2023-05-31 08:41:37.000000 PyHarshit-0.0.6/PyHarshit.egg-info/dependency_links.txt
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      103 2023-05-31 08:41:37.000000 PyHarshit-0.0.6/PyHarshit.egg-info/requires.txt
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)       10 2023-05-31 08:41:37.000000 PyHarshit-0.0.6/PyHarshit.egg-info/top_level.txt
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      564 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/README.md
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)       38 2023-05-31 08:41:37.174084 PyHarshit-0.0.6/setup.cfg
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      545 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/setup.py
+drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-06-01 15:13:59.108886 PyHarshit-0.0.7/
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      778 2023-06-01 15:13:59.108886 PyHarshit-0.0.7/PKG-INFO
+drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-06-01 15:13:59.104886 PyHarshit-0.0.7/PyHarshit/
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        1 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/PyHarshit/__init__.py
+drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-06-01 15:13:59.104886 PyHarshit-0.0.7/PyHarshit/tg/
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)     4125 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/PyHarshit/tg/Control.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)    12360 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/PyHarshit/tg/FasterTg.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)     1803 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/PyHarshit/tg/Functions.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        1 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/PyHarshit/tg/__init__.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)     3009 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/PyHarshit/tg/extractor.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      478 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/PyHarshit/tg/tools.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)     2761 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/PyHarshit/tg/uploader.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      174 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/PyHarshit/tg/utils.py
+drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-06-01 15:13:59.108886 PyHarshit-0.0.7/PyHarshit/tools/
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        1 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/PyHarshit/tools/__init__.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      173 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/PyHarshit/tools/anim.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)       19 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/PyHarshit/tools/boolset.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      106 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/PyHarshit/tools/charset.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)     1301 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/PyHarshit/tools/fiverr.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      313 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/PyHarshit/tools/maths.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      887 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/PyHarshit/tools/utils.py
+drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-06-01 15:13:59.104886 PyHarshit-0.0.7/PyHarshit.egg-info/
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      778 2023-06-01 15:13:59.000000 PyHarshit-0.0.7/PyHarshit.egg-info/PKG-INFO
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      581 2023-06-01 15:13:59.000000 PyHarshit-0.0.7/PyHarshit.egg-info/SOURCES.txt
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        1 2023-06-01 15:13:59.000000 PyHarshit-0.0.7/PyHarshit.egg-info/dependency_links.txt
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      119 2023-06-01 15:13:59.000000 PyHarshit-0.0.7/PyHarshit.egg-info/requires.txt
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)       10 2023-06-01 15:13:59.000000 PyHarshit-0.0.7/PyHarshit.egg-info/top_level.txt
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      564 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/README.md
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)       38 2023-06-01 15:13:59.108886 PyHarshit-0.0.7/setup.cfg
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      545 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/setup.py
```

### Comparing `PyHarshit-0.0.6/PKG-INFO` & `PyHarshit-0.0.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyHarshit
-Version: 0.0.6
+Version: 0.0.7
 Summary: Utlity file for my codes
 Author: Harshit Shrivastav
 Author-email: itsharshit@yandex.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # just a utility files for my codes
```

### Comparing `PyHarshit-0.0.6/PyHarshit/tg/FasterTg.py` & `PyHarshit-0.0.7/PyHarshit/tg/FasterTg.py`

 * *Files identical despite different names*

### Comparing `PyHarshit-0.0.6/PyHarshit/tg/extractor.py` & `PyHarshit-0.0.7/PyHarshit/tg/extractor.py`

 * *Files identical despite different names*

### Comparing `PyHarshit-0.0.6/PyHarshit/tg/tgControl.py` & `PyHarshit-0.0.7/PyHarshit/tg/Control.py`

 * *Files identical despite different names*

### Comparing `PyHarshit-0.0.6/PyHarshit/tg/tgFunctions.py` & `PyHarshit-0.0.7/PyHarshit/tg/Functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,23 @@
         msg  = await client.get_messages(chat, msg_id)
     except Exception as e:
         await message.reply(f'{str(e)}')
     if 't.me/c/' in msg_link:
         await message.reply(f'Sorry, but i can only give you message of public channel.', quote=True)
     else:
         chat =  msg_link.split("/")[-2]
+    if '?single' in link:
+        try:
+            await client.copy_media_group(int(sender), msg.chat.id, msg.id)
+        except FloodWait as f:
+            await message.reply(f'Bot is limited by telegram for {f.value + 2} seconds.\nPlease try again after {f.value + 2} seconds.', quote=True)
+            await asyncio.sleep(f.value)
+        except Exception as e: 
+            return await message.reply(f'Error: {str(e)}', quote=True)
+    else:
         try:
             await client.copy_message(int(sender), msg.chat.id, msg.id)
         except FloodWait as f:
             await message.reply(f'Bot is limited by telegram for {f.value + 2} seconds.\nPlease try again after {f.value + 2} seconds.', quote=True)
             await asyncio.sleep(f.value)
         except Exception as e: 
             return await message.reply(f'Error: {str(e)}', quote=True)
```

### Comparing `PyHarshit-0.0.6/PyHarshit/tg/uploader.py` & `PyHarshit-0.0.7/PyHarshit/tg/uploader.py`

 * *Files identical despite different names*

### Comparing `PyHarshit-0.0.6/PyHarshit/tools/utils.py` & `PyHarshit-0.0.7/PyHarshit/tools/utils.py`

 * *Files identical despite different names*

### Comparing `PyHarshit-0.0.6/PyHarshit.egg-info/PKG-INFO` & `PyHarshit-0.0.7/PyHarshit.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyHarshit
-Version: 0.0.6
+Version: 0.0.7
 Summary: Utlity file for my codes
 Author: Harshit Shrivastav
 Author-email: itsharshit@yandex.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # just a utility files for my codes
```

### Comparing `PyHarshit-0.0.6/PyHarshit.egg-info/SOURCES.txt` & `PyHarshit-0.0.7/PyHarshit.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 setup.py
 PyHarshit/__init__.py
 PyHarshit.egg-info/PKG-INFO
 PyHarshit.egg-info/SOURCES.txt
 PyHarshit.egg-info/dependency_links.txt
 PyHarshit.egg-info/requires.txt
 PyHarshit.egg-info/top_level.txt
+PyHarshit/tg/Control.py
 PyHarshit/tg/FasterTg.py
+PyHarshit/tg/Functions.py
 PyHarshit/tg/__init__.py
 PyHarshit/tg/extractor.py
-PyHarshit/tg/tgControl.py
-PyHarshit/tg/tgFunctions.py
 PyHarshit/tg/tools.py
 PyHarshit/tg/uploader.py
 PyHarshit/tg/utils.py
 PyHarshit/tools/__init__.py
 PyHarshit/tools/anim.py
 PyHarshit/tools/boolset.py
 PyHarshit/tools/charset.py
+PyHarshit/tools/fiverr.py
 PyHarshit/tools/maths.py
 PyHarshit/tools/utils.py
```

### Comparing `PyHarshit-0.0.6/README.md` & `PyHarshit-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `PyHarshit-0.0.6/setup.py` & `PyHarshit-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     page_description = f.read()
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="PyHarshit",
-    version="0.0.6",
+    version="0.0.7",
     author="Harshit Shrivastav",
     author_email="itsharshit@yandex.com",
     description="Utlity file for my codes",
     long_description=page_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=requirements,
```

