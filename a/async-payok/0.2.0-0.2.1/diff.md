# Comparing `tmp/async-payok-0.2.0.tar.gz` & `tmp/async-payok-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async-payok-0.2.0.tar", last modified: Thu Jun  1 02:09:36 2023, max compression
+gzip compressed data, was "async-payok-0.2.1.tar", last modified: Thu Jun  1 02:14:05 2023, max compression
```

## Comparing `async-payok-0.2.0.tar` & `async-payok-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 02:09:36.029625 async-payok-0.2.0/
--rw-rw-rw-   0        0        0     1585 2023-06-01 02:09:36.036732 async-payok-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1188 2023-06-01 02:09:09.000000 async-payok-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 02:09:36.016319 async-payok-0.2.0/async_payok/
--rw-rw-rw-   0        0        0      128 2023-05-27 05:54:41.000000 async-payok-0.2.0/async_payok/__init__.py
--rw-rw-rw-   0        0        0       25 2022-08-16 03:10:02.000000 async-payok-0.2.0/async_payok/__version__.py
--rw-rw-rw-   0        0        0     5874 2023-05-30 06:41:39.000000 async-payok-0.2.0/async_payok/asyncpayok.py
--rw-rw-rw-   0        0        0      138 2023-05-27 05:32:01.000000 async-payok-0.2.0/async_payok/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-01 02:09:36.028627 async-payok-0.2.0/async_payok/models/
--rw-rw-rw-   0        0        0      145 2023-05-27 05:54:41.000000 async-payok-0.2.0/async_payok/models/__init__.py
--rw-rw-rw-   0        0        0      162 2023-05-27 06:44:41.000000 async-payok-0.2.0/async_payok/models/balance.py
--rw-rw-rw-   0        0        0      469 2023-06-01 02:03:51.000000 async-payok-0.2.0/async_payok/models/enums.py
--rw-rw-rw-   0        0        0      496 2023-05-27 05:46:47.000000 async-payok-0.2.0/async_payok/models/invoice.py
--rw-rw-rw-   0        0        0      317 2023-05-27 06:55:47.000000 async-payok-0.2.0/async_payok/models/methods.py
-drwxrwxrwx   0        0        0        0 2023-06-01 02:09:36.021647 async-payok-0.2.0/async_payok.egg-info/
--rw-rw-rw-   0        0        0     1585 2023-06-01 02:09:35.000000 async-payok-0.2.0/async_payok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      488 2023-06-01 02:09:35.000000 async-payok-0.2.0/async_payok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 02:09:35.000000 async-payok-0.2.0/async_payok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-30 07:29:36.000000 async-payok-0.2.0/async_payok.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       70 2023-06-01 02:09:35.000000 async-payok-0.2.0/async_payok.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-01 02:09:35.000000 async-payok-0.2.0/async_payok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 02:09:36.037653 async-payok-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      929 2023-06-01 02:09:09.000000 async-payok-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 02:14:05.850005 async-payok-0.2.1/
+-rw-rw-rw-   0        0        0     1585 2023-06-01 02:14:05.850005 async-payok-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1188 2023-06-01 02:13:49.000000 async-payok-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 02:14:05.821358 async-payok-0.2.1/async_payok/
+-rw-rw-rw-   0        0        0      128 2023-05-27 05:54:41.000000 async-payok-0.2.1/async_payok/__init__.py
+-rw-rw-rw-   0        0        0       25 2022-08-16 03:10:02.000000 async-payok-0.2.1/async_payok/__version__.py
+-rw-rw-rw-   0        0        0     5874 2023-05-30 06:41:39.000000 async-payok-0.2.1/async_payok/asyncpayok.py
+-rw-rw-rw-   0        0        0      138 2023-05-27 05:32:01.000000 async-payok-0.2.1/async_payok/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-01 02:14:05.848001 async-payok-0.2.1/async_payok/models/
+-rw-rw-rw-   0        0        0      168 2023-06-01 02:13:49.000000 async-payok-0.2.1/async_payok/models/__init__.py
+-rw-rw-rw-   0        0        0      162 2023-05-27 06:44:41.000000 async-payok-0.2.1/async_payok/models/balance.py
+-rw-rw-rw-   0        0        0      469 2023-06-01 02:03:51.000000 async-payok-0.2.1/async_payok/models/enums.py
+-rw-rw-rw-   0        0        0      496 2023-05-27 05:46:47.000000 async-payok-0.2.1/async_payok/models/invoice.py
+-rw-rw-rw-   0        0        0      317 2023-05-27 06:55:47.000000 async-payok-0.2.1/async_payok/models/methods.py
+drwxrwxrwx   0        0        0        0 2023-06-01 02:14:05.839042 async-payok-0.2.1/async_payok.egg-info/
+-rw-rw-rw-   0        0        0     1585 2023-06-01 02:14:05.000000 async-payok-0.2.1/async_payok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      488 2023-06-01 02:14:05.000000 async-payok-0.2.1/async_payok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 02:14:05.000000 async-payok-0.2.1/async_payok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-01 02:14:05.000000 async-payok-0.2.1/async_payok.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       70 2023-06-01 02:14:05.000000 async-payok-0.2.1/async_payok.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-01 02:14:05.000000 async-payok-0.2.1/async_payok.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 02:14:05.851040 async-payok-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      929 2023-06-01 02:13:49.000000 async-payok-0.2.1/setup.py
```

### Comparing `async-payok-0.2.0/PKG-INFO` & `async-payok-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-payok
-Version: 0.2.0
+Version: 0.2.1
 Summary: Asynchronous module for working with the Payok API
 Author: VoXDoX
 Author-email: 1voxdox1@gmail.com
 Project-URL: TG Channel, https://t.me/AsyncModules
 Project-URL: Github, https://github.com/VoXDoX/async-payok
 Keywords: payok,payok api,asyncpayok,aiopayok
 Requires-Python: >=3.7
@@ -21,16 +21,16 @@
 ```
 pip3 install async-payok
 ```
 ![изображение](https://imgur.com/OyxTv9W.jpg)
 
 
 # Information | Информация
-ENG: The current version of AsyncPayOk is 0.2.0
-RU: Актуальная версия AsyncPayOk 0.2.0
+ENG: The current version of AsyncPayOk is 0.2.1
+RU: Актуальная версия AsyncPayOk 0.2.1
 
 # Methods | Фyнкции
 ## ENG
 ```
 Asynchronous module for working with the Payok API
 
 What can?
@@ -47,15 +47,15 @@
 Что может?
 - Получение баланса
 - Получение реферального баланса
 - Создание формы оплаты
 - Получение актуальных транзакций
 ```
 
-# UPDATE 0.2.0 | ОБНОВЛЕНИЕ 0.2.0
+# UPDATE 0.2.1 | ОБНОВЛЕНИЕ 0.2.1
 ```
 END:
 Added new types:
 - Status (PAID, WAITING);
 - Webhook_status (DELIVERED, NOT_DELIVERED, DELIVERED_ERROR)
 
 RU:
```

### Comparing `async-payok-0.2.0/README.md` & `async-payok-0.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 ```
 pip3 install async-payok
 ```
 ![изображение](https://imgur.com/OyxTv9W.jpg)
 
 
 # Information | Информация
-ENG: The current version of AsyncPayOk is 0.2.0
-RU: Актуальная версия AsyncPayOk 0.2.0
+ENG: The current version of AsyncPayOk is 0.2.1
+RU: Актуальная версия AsyncPayOk 0.2.1
 
 # Methods | Фyнкции
 ## ENG
 ```
 Asynchronous module for working with the Payok API
 
 What can?
@@ -35,15 +35,15 @@
 Что может?
 - Получение баланса
 - Получение реферального баланса
 - Создание формы оплаты
 - Получение актуальных транзакций
 ```
 
-# UPDATE 0.2.0 | ОБНОВЛЕНИЕ 0.2.0
+# UPDATE 0.2.1 | ОБНОВЛЕНИЕ 0.2.1
 ```
 END:
 Added new types:
 - Status (PAID, WAITING);
 - Webhook_status (DELIVERED, NOT_DELIVERED, DELIVERED_ERROR)
 
 RU:
```

### Comparing `async-payok-0.2.0/async_payok/asyncpayok.py` & `async-payok-0.2.1/async_payok/asyncpayok.py`

 * *Files identical despite different names*

### Comparing `async-payok-0.2.0/async_payok.egg-info/PKG-INFO` & `async-payok-0.2.1/async_payok.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-payok
-Version: 0.2.0
+Version: 0.2.1
 Summary: Asynchronous module for working with the Payok API
 Author: VoXDoX
 Author-email: 1voxdox1@gmail.com
 Project-URL: TG Channel, https://t.me/AsyncModules
 Project-URL: Github, https://github.com/VoXDoX/async-payok
 Keywords: payok,payok api,asyncpayok,aiopayok
 Requires-Python: >=3.7
@@ -21,16 +21,16 @@
 ```
 pip3 install async-payok
 ```
 ![изображение](https://imgur.com/OyxTv9W.jpg)
 
 
 # Information | Информация
-ENG: The current version of AsyncPayOk is 0.2.0
-RU: Актуальная версия AsyncPayOk 0.2.0
+ENG: The current version of AsyncPayOk is 0.2.1
+RU: Актуальная версия AsyncPayOk 0.2.1
 
 # Methods | Фyнкции
 ## ENG
 ```
 Asynchronous module for working with the Payok API
 
 What can?
@@ -47,15 +47,15 @@
 Что может?
 - Получение баланса
 - Получение реферального баланса
 - Создание формы оплаты
 - Получение актуальных транзакций
 ```
 
-# UPDATE 0.2.0 | ОБНОВЛЕНИЕ 0.2.0
+# UPDATE 0.2.1 | ОБНОВЛЕНИЕ 0.2.1
 ```
 END:
 Added new types:
 - Status (PAID, WAITING);
 - Webhook_status (DELIVERED, NOT_DELIVERED, DELIVERED_ERROR)
 
 RU:
```

### Comparing `async-payok-0.2.0/setup.py` & `async-payok-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 with open("README.md", "r", encoding="utf-8") as desc_long:
 	description_long = desc_long.read()
 
 
 setup(
 	name='async-payok',
-	version='0.2.0',
+	version='0.2.1',
 	description='Asynchronous module for working with the Payok API',
 	long_description=description_long,
 	packages=find_packages(),
 	long_description_content_type='text/markdown',
 	author='VoXDoX',
 	author_email='1voxdox1@gmail.com',
 	keywords=['payok', 'payok api', 'asyncpayok', 'aiopayok'],
```

