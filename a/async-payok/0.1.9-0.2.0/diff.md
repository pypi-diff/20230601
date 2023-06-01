# Comparing `tmp/async-payok-0.1.9.tar.gz` & `tmp/async-payok-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async-payok-0.1.9.tar", last modified: Tue May 30 07:29:36 2023, max compression
+gzip compressed data, was "async-payok-0.2.0.tar", last modified: Thu Jun  1 02:09:36 2023, max compression
```

## Comparing `async-payok-0.1.9.tar` & `async-payok-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 07:29:36.703596 async-payok-0.1.9/
--rw-rw-rw-   0        0        0     1278 2023-05-30 07:29:36.703596 async-payok-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0      881 2023-05-30 07:27:27.000000 async-payok-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 07:29:36.656222 async-payok-0.1.9/async_payok/
--rw-rw-rw-   0        0        0      128 2023-05-27 05:54:41.000000 async-payok-0.1.9/async_payok/__init__.py
--rw-rw-rw-   0        0        0       25 2022-08-16 03:10:02.000000 async-payok-0.1.9/async_payok/__version__.py
--rw-rw-rw-   0        0        0     5874 2023-05-30 06:41:39.000000 async-payok-0.1.9/async_payok/asyncpayok.py
--rw-rw-rw-   0        0        0      138 2023-05-27 05:32:01.000000 async-payok-0.1.9/async_payok/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-30 07:29:36.702282 async-payok-0.1.9/async_payok/models/
--rw-rw-rw-   0        0        0      145 2023-05-27 05:54:41.000000 async-payok-0.1.9/async_payok/models/__init__.py
--rw-rw-rw-   0        0        0      162 2023-05-27 06:44:41.000000 async-payok-0.1.9/async_payok/models/balance.py
--rw-rw-rw-   0        0        0      199 2023-05-27 06:55:47.000000 async-payok-0.1.9/async_payok/models/enums.py
--rw-rw-rw-   0        0        0      496 2023-05-27 05:46:47.000000 async-payok-0.1.9/async_payok/models/invoice.py
--rw-rw-rw-   0        0        0      317 2023-05-27 06:55:47.000000 async-payok-0.1.9/async_payok/models/methods.py
-drwxrwxrwx   0        0        0        0 2023-05-30 07:29:36.695578 async-payok-0.1.9/async_payok.egg-info/
--rw-rw-rw-   0        0        0     1278 2023-05-30 07:29:36.000000 async-payok-0.1.9/async_payok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      488 2023-05-30 07:29:36.000000 async-payok-0.1.9/async_payok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 07:29:36.000000 async-payok-0.1.9/async_payok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-30 07:29:36.000000 async-payok-0.1.9/async_payok.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       70 2023-05-30 07:29:36.000000 async-payok-0.1.9/async_payok.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-30 07:29:36.000000 async-payok-0.1.9/async_payok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 07:29:36.704586 async-payok-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      929 2023-05-30 07:29:15.000000 async-payok-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 02:09:36.029625 async-payok-0.2.0/
+-rw-rw-rw-   0        0        0     1585 2023-06-01 02:09:36.036732 async-payok-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1188 2023-06-01 02:09:09.000000 async-payok-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 02:09:36.016319 async-payok-0.2.0/async_payok/
+-rw-rw-rw-   0        0        0      128 2023-05-27 05:54:41.000000 async-payok-0.2.0/async_payok/__init__.py
+-rw-rw-rw-   0        0        0       25 2022-08-16 03:10:02.000000 async-payok-0.2.0/async_payok/__version__.py
+-rw-rw-rw-   0        0        0     5874 2023-05-30 06:41:39.000000 async-payok-0.2.0/async_payok/asyncpayok.py
+-rw-rw-rw-   0        0        0      138 2023-05-27 05:32:01.000000 async-payok-0.2.0/async_payok/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-01 02:09:36.028627 async-payok-0.2.0/async_payok/models/
+-rw-rw-rw-   0        0        0      145 2023-05-27 05:54:41.000000 async-payok-0.2.0/async_payok/models/__init__.py
+-rw-rw-rw-   0        0        0      162 2023-05-27 06:44:41.000000 async-payok-0.2.0/async_payok/models/balance.py
+-rw-rw-rw-   0        0        0      469 2023-06-01 02:03:51.000000 async-payok-0.2.0/async_payok/models/enums.py
+-rw-rw-rw-   0        0        0      496 2023-05-27 05:46:47.000000 async-payok-0.2.0/async_payok/models/invoice.py
+-rw-rw-rw-   0        0        0      317 2023-05-27 06:55:47.000000 async-payok-0.2.0/async_payok/models/methods.py
+drwxrwxrwx   0        0        0        0 2023-06-01 02:09:36.021647 async-payok-0.2.0/async_payok.egg-info/
+-rw-rw-rw-   0        0        0     1585 2023-06-01 02:09:35.000000 async-payok-0.2.0/async_payok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      488 2023-06-01 02:09:35.000000 async-payok-0.2.0/async_payok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 02:09:35.000000 async-payok-0.2.0/async_payok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-30 07:29:36.000000 async-payok-0.2.0/async_payok.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       70 2023-06-01 02:09:35.000000 async-payok-0.2.0/async_payok.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-01 02:09:35.000000 async-payok-0.2.0/async_payok.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 02:09:36.037653 async-payok-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      929 2023-06-01 02:09:09.000000 async-payok-0.2.0/setup.py
```

### Comparing `async-payok-0.1.9/PKG-INFO` & `async-payok-0.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: async-payok
-Version: 0.1.9
-Summary: Asynchronous module for working with the Payok API
-Author: VoXDoX
-Author-email: 1voxdox1@gmail.com
-Project-URL: TG Channel, https://t.me/AsyncModules
-Project-URL: Github, https://github.com/VoXDoX/async-payok
-Keywords: payok,payok api,asyncpayok,aiopayok
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 # Installation | Установка
 
 ## Windows
 ```
 pip install async-payok
 ```
 
@@ -21,16 +9,16 @@
 ```
 pip3 install async-payok
 ```
 ![изображение](https://imgur.com/OyxTv9W.jpg)
 
 
 # Information | Информация
-ENG: The current version of AsyncPayOk is 0.1.9
-RU: Актуальная версия AsyncPayOk 0.1.9
+ENG: The current version of AsyncPayOk is 0.2.0
+RU: Актуальная версия AsyncPayOk 0.2.0
 
 # Methods | Фyнкции
 ## ENG
 ```
 Asynchronous module for working with the Payok API
 
 What can?
@@ -46,7 +34,20 @@
 
 Что может?
 - Получение баланса
 - Получение реферального баланса
 - Создание формы оплаты
 - Получение актуальных транзакций
 ```
+
+# UPDATE 0.2.0 | ОБНОВЛЕНИЕ 0.2.0
+```
+END:
+Added new types:
+- Status (PAID, WAITING);
+- Webhook_status (DELIVERED, NOT_DELIVERED, DELIVERED_ERROR)
+
+RU:
+Добавлены новые типы:
+- Status (PAID, WAITING);
+- Webhook_status (DELIVERED, NOT_DELIVERED, DELIVERED_ERROR)
+```
```

### Comparing `async-payok-0.1.9/async_payok/asyncpayok.py` & `async-payok-0.2.0/async_payok/asyncpayok.py`

 * *Files identical despite different names*

### Comparing `async-payok-0.1.9/setup.py` & `async-payok-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 with open("README.md", "r", encoding="utf-8") as desc_long:
 	description_long = desc_long.read()
 
 
 setup(
 	name='async-payok',
-	version='0.1.9',
+	version='0.2.0',
 	description='Asynchronous module for working with the Payok API',
 	long_description=description_long,
 	packages=find_packages(),
 	long_description_content_type='text/markdown',
 	author='VoXDoX',
 	author_email='1voxdox1@gmail.com',
 	keywords=['payok', 'payok api', 'asyncpayok', 'aiopayok'],
```

