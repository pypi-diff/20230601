# Comparing `tmp/yeref-0.1.71.tar.gz` & `tmp/yeref-0.1.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.71.tar", last modified: Tue May 30 14:43:03 2023, max compression
+gzip compressed data, was "yeref-0.1.72.tar", last modified: Thu Jun  1 11:57:39 2023, max compression
```

## Comparing `yeref-0.1.71.tar` & `yeref-0.1.72.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-30 14:43:03.920371 yeref-0.1.71/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-30 14:43:03.920611 yeref-0.1.71/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-30 14:43:03.921854 yeref-0.1.71/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1392 2023-05-30 14:42:44.000000 yeref-0.1.71/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-30 14:43:03.913062 yeref-0.1.71/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.71/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   489716 2023-05-30 14:42:24.000000 yeref-0.1.71/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   206005 2023-05-30 13:53:38.000000 yeref-0.1.71/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-30 14:43:03.919047 yeref-0.1.71/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-30 14:43:03.000000 yeref-0.1.71/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-30 14:43:03.000000 yeref-0.1.71/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-30 14:43:03.000000 yeref-0.1.71/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-30 14:43:03.000000 yeref-0.1.71/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-01 11:57:39.092430 yeref-0.1.72/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-01 11:57:39.092668 yeref-0.1.72/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-01 11:57:39.093507 yeref-0.1.72/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-01 11:57:12.000000 yeref-0.1.72/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-01 11:57:39.089486 yeref-0.1.72/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.72/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   489747 2023-05-30 14:52:13.000000 yeref-0.1.72/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   207128 2023-06-01 11:53:54.000000 yeref-0.1.72/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-01 11:57:39.092039 yeref-0.1.72/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-01 11:57:39.000000 yeref-0.1.72/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-01 11:57:39.000000 yeref-0.1.72/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-01 11:57:39.000000 yeref-0.1.72/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-01 11:57:39.000000 yeref-0.1.72/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.71/setup.py` & `yeref-0.1.72/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.71',
+      version='0.1.72',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -41,15 +41,14 @@
 
 # python -m build
 
 # twine upload dist/*
 # freey.sitner.ya
 # cejwez-nosgin-vaVfe7
 
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.66-py3-none-any.whl
-
 # python3 -m pip install --upgrade yeref
 
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.71-py3-none-any.whl
 # pip install --force-reinstall -v "yeref==0.1.30"
 # pip install https://github.com/aiogram/aiogram/archive/refs/heads/dev-3.x.zip
 # pip show aiogram
 # ARCHFLAGS="-arch x86_64" pip install pycurl
```

### Comparing `yeref-0.1.71/yeref/l_.py` & `yeref-0.1.72/yeref/l_.py`

 * *Files 0% similar despite different names*

```diff
@@ -597,15 +597,15 @@
     'en': "🗝️ <b>Newsletter</b> ..{0}%",
     'es': "🗝️ <b>Boletín</b> ..{0}%",
     'fr': "🗝️ <b>Newsletter</b> ..{0}%",
     'zh': "🗝️<b>时事通讯</b>..{0}%",
     'ar': "🗝️ <b>النشرة الإخبارية</b> .. {0}٪",
 }
 l_broadcast_finish = {
-    'ru': "🏁 <b>Рассылка</b> завершена\n\n📧 Число пользователей, получивших сообщение: <u>{0}</u>",
+    'ru': "🏁 <b>Рассылка</b> завершена\n\n📧 <b>Количество</b> пользователей, получивших сообщение: <u>{0}</u>",
     'en': "🏁 <b>Newsletter</b> ended\n\n🗝️ Number of users who received the message: <u>{0}</u>",
     'es': "🏁 <b>Boletín</b> finalizado\n\n🗝️ Número de usuarios que recibieron el mensaje: <u>{0}</u>",
     'fr': "🏁 <b>Newsletter</b> terminée\n\n🗝️ Nombre d&#x27;utilisateurs ayant reçu le message : <u>{0}</u>",
     'zh': "🏁<b>通讯</b>结束\n\n🗝️ 收到消息的用户数： <u>{0}</u>",
     'ar': "🏁 انتهت <b>الرسالة الإخبارية</b>\n\n🗝️ عدد المستخدمين الذين تلقوا الرسالة: <u>{0}</u>",
 }
 
@@ -3259,23 +3259,23 @@
     'en': "🎥 Send this command as reply to message",
     'es': "🎥 Enviar este comando como respuesta al mensaje",
     'fr': "🎥 Envoyez cette commande en réponse au message",
     'zh': "🎥 將此命令作為對消息的回復發送",
     'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
 }
 l_ban_users_start = {
-    'ru': "👩🏽‍💻 <b>Очистка</b> запущена\nТекущее количество пользователей в базе: <u>{0}</u>",
+    'ru': "👩🏽‍💻 <b>Очистка</b> запущена\n<b>Текущее</b> количество пользователей в базе: <u>{0}</u>",
     'en': "🎥 Send this command as reply to message",
     'es': "🎥 Enviar este comando como respuesta al mensaje",
     'fr': "🎥 Envoyez cette commande en réponse au message",
     'zh': "🎥 將此命令作為對消息的回復發送",
     'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
 }
 l_ban_users_stop = {
-    'ru': "👩🏽‍💻 <b>Очистка</b> завершена\nТекущее количество пользователей в базе: <u>{0}</u> (-{1})",
+    'ru': "👩🏽‍💻 <b>Очистка</b> завершена\n<b>Текущее</b> количество пользователей в базе: <u>{0}</u> (-{1})",
     'en': "🎥 Send this command as reply to message",
     'es': "🎥 Enviar este comando como respuesta al mensaje",
     'fr': "🎥 Envoyez cette commande en réponse au message",
     'zh': "🎥 將此命令作為對消息的回復發送",
     'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
 }
 l_chn_ccheck_handler = {
```

### Comparing `yeref-0.1.71/yeref/yeref.py` & `yeref-0.1.72/yeref/yeref.py`

 * *Files 1% similar despite different names*

```diff
@@ -3165,14 +3165,44 @@
     for k, v in dicti_.items():
         if tmp == pos:
             return k, v
         tmp += 1
     return None, None
 
 
+async def del_extra_files(UNKNOWN_ERRORS_TXT, EXTRA_D):
+    try:
+        if os.path.exists(UNKNOWN_ERRORS_TXT): os.remove(UNKNOWN_ERRORS_TXT)
+
+        max_dt = datetime.datetime(2020, 1, 1)
+        arr = [it for it in os.listdir(EXTRA_D) if it.startswith('debug.') and it != 'debug.log']
+
+        for item in arr:
+            parts = item.split('.')
+            if len(parts) <= 2: continue
+            parts_dt = parts[1].split('_')
+            cur_dt = datetime.datetime.strptime(f"{parts_dt[0]}_{parts_dt[1]}", '%d-%m-%Y_%H-%M-%S')
+
+            if cur_dt > max_dt:
+                max_dt = cur_dt
+
+        for item in arr:
+            file_item = os.path.join(EXTRA_D, item)
+            parts = item.split('.')
+            if len(parts) <= 2: continue
+            parts_dt = parts[1].split('_')
+            cur_dt = datetime.datetime.strptime(f"{parts_dt[0]}_{parts_dt[1]}", '%d-%m-%Y_%H-%M-%S')
+
+            if cur_dt < max_dt and os.path.exists(file_item):
+                os.remove(file_item)
+    except Exception as e:
+        logger.info(log_ % str(e))
+        await asyncio.sleep(round(random.uniform(0, 1), 2))
+
+
 async def get_proxy(identifier, EXTRA_D, CONF_P, server=None):
     result = None
     try:
         if r_conf('proxy', CONF_P) == 0: return
 
         with open(os.path.join(EXTRA_D, "proxy.txt"), "r") as f:
             lines = f.readlines()
```

