# Comparing `tmp/oking_oz-3.2.32.tar.gz` & `tmp/oking_oz-3.2.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oking_oz-3.2.32.tar", last modified: Fri May 12 18:45:02 2023, max compression
+gzip compressed data, was "oking_oz-3.2.33.tar", last modified: Thu Jun  1 17:54:02 2023, max compression
```

## Comparing `oking_oz-3.2.32.tar` & `oking_oz-3.2.33.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 18:45:02.614814 oking_oz-3.2.32/
--rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.32/LICENSE
--rw-rw-rw-   0        0        0       29 2022-06-03 11:48:57.000000 oking_oz-3.2.32/MANIFEST.in
--rw-rw-rw-   0        0        0      935 2023-05-12 18:45:02.614814 oking_oz-3.2.32/PKG-INFO
--rw-rw-rw-   0        0        0     1187 2022-06-03 12:55:44.000000 oking_oz-3.2.32/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 18:45:02.567535 oking_oz-3.2.32/oking_oz.egg-info/
--rw-rw-rw-   0        0        0      935 2023-05-12 18:45:02.000000 oking_oz-3.2.32/oking_oz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1551 2023-05-12 18:45:02.000000 oking_oz-3.2.32/oking_oz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 18:45:02.000000 oking_oz-3.2.32/oking_oz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-12 18:45:02.000000 oking_oz-3.2.32/oking_oz.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       96 2023-05-12 18:45:02.000000 oking_oz-3.2.32/oking_oz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-12 18:45:02.000000 oking_oz-3.2.32/oking_oz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-06-03 11:48:57.000000 oking_oz-3.2.32/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-12 18:45:02.614814 oking_oz-3.2.32/setup.cfg
--rw-rw-rw-   0        0        0     1833 2023-05-12 18:44:55.000000 oking_oz-3.2.32/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-12 18:45:02.567535 oking_oz-3.2.32/src/
--rw-rw-rw-   0        0        0     2979 2022-08-23 11:22:25.000000 oking_oz-3.2.32/src/__init__.py
--rw-rw-rw-   0        0        0    25475 2023-04-10 18:55:42.000000 oking_oz-3.2.32/src/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 18:45:02.567535 oking_oz-3.2.32/src/api/
--rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.32/src/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 18:45:02.567535 oking_oz-3.2.32/src/api/entities/
--rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.32/src/api/entities/__init__.py
--rw-rw-rw-   0        0        0     5097 2022-12-16 19:21:16.000000 oking_oz-3.2.32/src/api/entities/cliente.py
--rw-rw-rw-   0        0        0     4496 2022-12-23 14:47:52.000000 oking_oz-3.2.32/src/api/entities/cliente_aprovado.py
--rw-rw-rw-   0        0        0      249 2022-12-19 18:06:20.000000 oking_oz-3.2.32/src/api/entities/cliente_erp_code.py
--rw-rw-rw-   0        0        0      932 2022-10-03 17:41:50.000000 oking_oz-3.2.32/src/api/entities/imposto_produto.py
--rw-rw-rw-   0        0        0     1171 2022-10-03 17:41:50.000000 oking_oz-3.2.32/src/api/entities/lista_preco.py
--rw-rw-rw-   0        0        0      390 2022-12-16 19:21:16.000000 oking_oz-3.2.32/src/api/entities/plano_pagamento_cliente.py
--rw-rw-rw-   0        0        0      934 2022-12-16 19:21:16.000000 oking_oz-3.2.32/src/api/entities/representante.py
--rw-rw-rw-   0        0        0      739 2022-06-03 11:48:57.000000 oking_oz-3.2.32/src/api/oking.py
--rw-rw-rw-   0        0        0    20636 2023-04-10 18:55:42.000000 oking_oz-3.2.32/src/api/okvendas.py
--rw-rw-rw-   0        0        0      886 2022-06-03 11:48:57.000000 oking_oz-3.2.32/src/api/slack.py
-drwxrwxrwx   0        0        0        0 2023-05-12 18:45:02.583169 oking_oz-3.2.32/src/database/
--rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.32/src/database/__init__.py
--rw-rw-rw-   0        0        0     2488 2022-08-23 11:22:25.000000 oking_oz-3.2.32/src/database/connection.py
-drwxrwxrwx   0        0        0        0 2023-05-12 18:45:02.583169 oking_oz-3.2.32/src/database/entities/
--rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.32/src/database/entities/__init__.py
--rw-rw-rw-   0        0        0     1616 2022-12-16 19:21:16.000000 oking_oz-3.2.32/src/database/entities/client.py
--rw-rw-rw-   0        0        0      253 2022-12-16 19:21:16.000000 oking_oz-3.2.32/src/database/entities/client_payment_plan.py
--rw-rw-rw-   0        0        0     1077 2022-10-03 17:41:50.000000 oking_oz-3.2.32/src/database/entities/price_list.py
--rw-rw-rw-   0        0        0      801 2023-04-10 18:55:42.000000 oking_oz-3.2.32/src/database/entities/product_tax.py
--rw-rw-rw-   0        0        0      639 2022-12-16 19:21:16.000000 oking_oz-3.2.32/src/database/entities/representative.py
--rw-rw-rw-   0        0        0    49121 2023-05-12 18:30:53.000000 oking_oz-3.2.32/src/database/queries.py
--rw-rw-rw-   0        0        0      327 2022-07-04 16:40:47.000000 oking_oz-3.2.32/src/database/sqlserver_db.py
--rw-rw-rw-   0        0        0     1106 2022-07-04 16:40:47.000000 oking_oz-3.2.32/src/database/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-12 18:45:02.601304 oking_oz-3.2.32/src/entities/
--rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.32/src/entities/__init__.py
--rw-rw-rw-   0        0        0      628 2022-07-29 17:49:42.000000 oking_oz-3.2.32/src/entities/invoice.py
--rw-rw-rw-   0        0        0      288 2022-06-03 11:48:57.000000 oking_oz-3.2.32/src/entities/log.py
--rw-rw-rw-   0        0        0     6846 2023-05-12 18:44:49.000000 oking_oz-3.2.32/src/entities/order.py
--rw-rw-rw-   0        0        0    16869 2023-04-10 18:55:42.000000 oking_oz-3.2.32/src/entities/orderb2b.py
--rw-rw-rw-   0        0        0     6823 2023-05-12 18:30:53.000000 oking_oz-3.2.32/src/entities/orderb2c.py
--rw-rw-rw-   0        0        0     3014 2022-06-03 11:48:57.000000 oking_oz-3.2.32/src/entities/pagamento.py
--rw-rw-rw-   0        0        0      351 2022-06-03 11:48:57.000000 oking_oz-3.2.32/src/entities/photos_sku.py
--rw-rw-rw-   0        0        0      407 2022-06-03 11:48:57.000000 oking_oz-3.2.32/src/entities/price.py
--rw-rw-rw-   0        0        0    10790 2023-04-10 18:55:42.000000 oking_oz-3.2.32/src/entities/product.py
--rw-rw-rw-   0        0        0     1959 2022-12-16 19:21:16.000000 oking_oz-3.2.32/src/entities/response.py
--rw-rw-rw-   0        0        0      940 2022-06-03 11:48:57.000000 oking_oz-3.2.32/src/entities/tracking.py
-drwxrwxrwx   0        0        0        0 2023-05-12 18:45:02.614814 oking_oz-3.2.32/src/jobs/
--rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.32/src/jobs/__init__.py
--rw-rw-rw-   0        0        0    18254 2023-04-10 18:55:42.000000 oking_oz-3.2.32/src/jobs/client_jobs.py
--rw-rw-rw-   0        0        0     8965 2023-04-10 18:55:42.000000 oking_oz-3.2.32/src/jobs/client_payment_plan_jobs.py
--rw-rw-rw-   0        0        0     2937 2023-04-10 18:55:42.000000 oking_oz-3.2.32/src/jobs/client_payment_plan_semaphore_jobs.py
--rw-rw-rw-   0        0        0    83964 2023-05-12 18:30:53.000000 oking_oz-3.2.32/src/jobs/order_jobs.py
--rw-rw-rw-   0        0        0    19666 2023-04-10 18:55:42.000000 oking_oz-3.2.32/src/jobs/price_jobs.py
--rw-rw-rw-   0        0        0    25107 2023-04-10 18:55:42.000000 oking_oz-3.2.32/src/jobs/products_jobs.py
--rw-rw-rw-   0        0        0     6841 2023-04-10 18:55:42.000000 oking_oz-3.2.32/src/jobs/representative_jobs.py
--rw-rw-rw-   0        0        0    12784 2023-04-10 18:55:42.000000 oking_oz-3.2.32/src/jobs/stock_jobs.py
--rw-rw-rw-   0        0        0     2003 2023-04-10 18:55:42.000000 oking_oz-3.2.32/src/jobs/system_jobs.py
+drwxrwxrwx   0        0        0        0 2023-06-01 17:54:02.755423 oking_oz-3.2.33/
+-rw-rw-rw-   0        0        0        0 2023-01-26 18:55:11.000000 oking_oz-3.2.33/LICENSE
+-rw-rw-rw-   0        0        0       29 2023-01-26 18:55:11.000000 oking_oz-3.2.33/MANIFEST.in
+-rw-rw-rw-   0        0        0      876 2023-06-01 17:54:02.750436 oking_oz-3.2.33/PKG-INFO
+-rw-rw-rw-   0        0        0     1187 2023-01-26 18:55:11.000000 oking_oz-3.2.33/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 17:54:02.301634 oking_oz-3.2.33/oking_oz.egg-info/
+-rw-rw-rw-   0        0        0      876 2023-06-01 17:54:02.000000 oking_oz-3.2.33/oking_oz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1551 2023-06-01 17:54:02.000000 oking_oz-3.2.33/oking_oz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 17:54:02.000000 oking_oz-3.2.33/oking_oz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-01 17:54:02.000000 oking_oz-3.2.33/oking_oz.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       96 2023-06-01 17:54:02.000000 oking_oz-3.2.33/oking_oz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-01 17:54:02.000000 oking_oz-3.2.33/oking_oz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-01-26 18:55:11.000000 oking_oz-3.2.33/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-01 17:54:02.756421 oking_oz-3.2.33/setup.cfg
+-rw-rw-rw-   0        0        0     1833 2023-06-01 17:49:44.000000 oking_oz-3.2.33/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 17:54:02.317591 oking_oz-3.2.33/src/
+-rw-rw-rw-   0        0        0     2979 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/__init__.py
+-rw-rw-rw-   0        0        0    25475 2023-04-24 14:39:17.000000 oking_oz-3.2.33/src/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 17:54:02.359479 oking_oz-3.2.33/src/api/
+-rw-rw-rw-   0        0        0        0 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 17:54:02.434281 oking_oz-3.2.33/src/api/entities/
+-rw-rw-rw-   0        0        0        0 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/api/entities/__init__.py
+-rw-rw-rw-   0        0        0     5097 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/api/entities/cliente.py
+-rw-rw-rw-   0        0        0     4496 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/api/entities/cliente_aprovado.py
+-rw-rw-rw-   0        0        0      249 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/api/entities/cliente_erp_code.py
+-rw-rw-rw-   0        0        0      932 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/api/entities/imposto_produto.py
+-rw-rw-rw-   0        0        0     1171 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/api/entities/lista_preco.py
+-rw-rw-rw-   0        0        0      390 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/api/entities/plano_pagamento_cliente.py
+-rw-rw-rw-   0        0        0      934 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/api/entities/representante.py
+-rw-rw-rw-   0        0        0      739 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/api/oking.py
+-rw-rw-rw-   0        0        0    20636 2023-04-12 12:17:25.000000 oking_oz-3.2.33/src/api/okvendas.py
+-rw-rw-rw-   0        0        0      886 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/api/slack.py
+drwxrwxrwx   0        0        0        0 2023-06-01 17:54:02.475170 oking_oz-3.2.33/src/database/
+-rw-rw-rw-   0        0        0        0 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/database/__init__.py
+-rw-rw-rw-   0        0        0     2488 2023-01-30 16:28:22.000000 oking_oz-3.2.33/src/database/connection.py
+drwxrwxrwx   0        0        0        0 2023-06-01 17:54:02.532020 oking_oz-3.2.33/src/database/entities/
+-rw-rw-rw-   0        0        0        0 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/database/entities/__init__.py
+-rw-rw-rw-   0        0        0     1616 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/database/entities/client.py
+-rw-rw-rw-   0        0        0      253 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/database/entities/client_payment_plan.py
+-rw-rw-rw-   0        0        0     1077 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/database/entities/price_list.py
+-rw-rw-rw-   0        0        0      801 2023-04-12 12:17:25.000000 oking_oz-3.2.33/src/database/entities/product_tax.py
+-rw-rw-rw-   0        0        0      639 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/database/entities/representative.py
+-rw-rw-rw-   0        0        0    50196 2023-06-01 16:36:53.000000 oking_oz-3.2.33/src/database/queries.py
+-rw-rw-rw-   0        0        0      327 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/database/sqlserver_db.py
+-rw-rw-rw-   0        0        0     1106 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/database/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-01 17:54:02.638734 oking_oz-3.2.33/src/entities/
+-rw-rw-rw-   0        0        0        0 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/entities/__init__.py
+-rw-rw-rw-   0        0        0      628 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/entities/invoice.py
+-rw-rw-rw-   0        0        0      288 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/entities/log.py
+-rw-rw-rw-   0        0        0     6846 2023-05-12 18:44:31.000000 oking_oz-3.2.33/src/entities/order.py
+-rw-rw-rw-   0        0        0    16869 2023-02-23 22:27:38.000000 oking_oz-3.2.33/src/entities/orderb2b.py
+-rw-rw-rw-   0        0        0     6823 2023-05-12 18:23:12.000000 oking_oz-3.2.33/src/entities/orderb2c.py
+-rw-rw-rw-   0        0        0     3014 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/entities/pagamento.py
+-rw-rw-rw-   0        0        0      351 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/entities/photos_sku.py
+-rw-rw-rw-   0        0        0      407 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/entities/price.py
+-rw-rw-rw-   0        0        0    10790 2023-02-23 22:27:38.000000 oking_oz-3.2.33/src/entities/product.py
+-rw-rw-rw-   0        0        0     1959 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/entities/response.py
+-rw-rw-rw-   0        0        0      940 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/entities/tracking.py
+drwxrwxrwx   0        0        0        0 2023-06-01 17:54:02.734478 oking_oz-3.2.33/src/jobs/
+-rw-rw-rw-   0        0        0        0 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/jobs/__init__.py
+-rw-rw-rw-   0        0        0    18254 2023-04-12 12:17:25.000000 oking_oz-3.2.33/src/jobs/client_jobs.py
+-rw-rw-rw-   0        0        0     8965 2023-04-12 12:17:25.000000 oking_oz-3.2.33/src/jobs/client_payment_plan_jobs.py
+-rw-rw-rw-   0        0        0     2937 2023-04-12 12:17:25.000000 oking_oz-3.2.33/src/jobs/client_payment_plan_semaphore_jobs.py
+-rw-rw-rw-   0        0        0    85575 2023-06-01 16:50:56.000000 oking_oz-3.2.33/src/jobs/order_jobs.py
+-rw-rw-rw-   0        0        0    19666 2023-03-20 16:46:08.000000 oking_oz-3.2.33/src/jobs/price_jobs.py
+-rw-rw-rw-   0        0        0    25107 2023-04-12 12:17:25.000000 oking_oz-3.2.33/src/jobs/products_jobs.py
+-rw-rw-rw-   0        0        0     6841 2023-03-20 16:47:52.000000 oking_oz-3.2.33/src/jobs/representative_jobs.py
+-rw-rw-rw-   0        0        0    12784 2023-03-20 16:49:42.000000 oking_oz-3.2.33/src/jobs/stock_jobs.py
+-rw-rw-rw-   0        0        0     2003 2023-03-20 16:50:03.000000 oking_oz-3.2.33/src/jobs/system_jobs.py
```

### Comparing `oking_oz-3.2.32/PKG-INFO` & `oking_oz-3.2.33/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 Metadata-Version: 2.1
 Name: oking_oz
-Version: 3.2.32
+Version: 3.2.33
 Summary: Pacote de integração de produtos, preço, estoque e pedidos com o sistema OkVendas da Openk
-Home-page: UNKNOWN
 Author: Openk Tecnologia
 Author-email: <suporte.b2c@openk.com.br>
-License: UNKNOWN
 Keywords: python,oking,openk,okvendas,ok
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
@@ -24,8 +21,7 @@
 - Estoque
 - Pedido
 - Produtos
 - Clientes
 
 ## Manual
 <https://doc.clickup.com/d/h/2zgwt-5063/8b4903a4de0ccbd>
-
```

### Comparing `oking_oz-3.2.32/README.md` & `oking_oz-3.2.33/README.md`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/oking_oz.egg-info/PKG-INFO` & `oking_oz-3.2.33/oking_oz.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 Metadata-Version: 2.1
 Name: oking-oz
-Version: 3.2.32
+Version: 3.2.33
 Summary: Pacote de integração de produtos, preço, estoque e pedidos com o sistema OkVendas da Openk
-Home-page: UNKNOWN
 Author: Openk Tecnologia
 Author-email: <suporte.b2c@openk.com.br>
-License: UNKNOWN
 Keywords: python,oking,openk,okvendas,ok
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
@@ -24,8 +21,7 @@
 - Estoque
 - Pedido
 - Produtos
 - Clientes
 
 ## Manual
 <https://doc.clickup.com/d/h/2zgwt-5063/8b4903a4de0ccbd>
-
```

### Comparing `oking_oz-3.2.32/oking_oz.egg-info/SOURCES.txt` & `oking_oz-3.2.33/oking_oz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/setup.py` & `oking_oz-3.2.33/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #     f = open('version.txt', 'w')
 #     f.write(f'\tOking {v} - Openk Tecnologia')
 #     f.close()
 
 
 # Utilizar o padrão x.x.x.xxxx para caso precise subir versão de testes para o respositorio test-pypi
 # Utilizar o padrão x.x.x para subir em produção
-version = '3.2.32'
+version = '3.2.33'
 package_name = "oking_oz" if len([c for c in version if c == '.']) < 3 else 'okingtest'
 # save_version(version)
 setup(
     name=package_name,
     version=version,
     author="Openk Tecnologia",
     author_email="<suporte.b2c@openk.com.br>",
```

### Comparing `oking_oz-3.2.32/src/__init__.py` & `oking_oz-3.2.33/src/__init__.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/src/__main__.py` & `oking_oz-3.2.33/src/__main__.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/src/api/entities/cliente.py` & `oking_oz-3.2.33/src/api/entities/cliente.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/src/api/entities/cliente_aprovado.py` & `oking_oz-3.2.33/src/api/entities/cliente_aprovado.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/src/api/entities/imposto_produto.py` & `oking_oz-3.2.33/src/api/entities/imposto_produto.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/src/api/entities/lista_preco.py` & `oking_oz-3.2.33/src/api/entities/lista_preco.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/src/api/entities/representante.py` & `oking_oz-3.2.33/src/api/entities/representante.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/src/api/oking.py` & `oking_oz-3.2.33/src/api/oking.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/src/api/okvendas.py` & `oking_oz-3.2.33/src/api/okvendas.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/src/api/slack.py` & `oking_oz-3.2.33/src/api/slack.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/src/database/connection.py` & `oking_oz-3.2.33/src/database/connection.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/src/database/entities/client.py` & `oking_oz-3.2.33/src/database/entities/client.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/src/database/entities/price_list.py` & `oking_oz-3.2.33/src/database/entities/price_list.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/src/database/entities/product_tax.py` & `oking_oz-3.2.33/src/database/entities/product_tax.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/src/database/entities/representative.py` & `oking_oz-3.2.33/src/database/entities/representative.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/src/database/queries.py` & `oking_oz-3.2.33/src/database/queries.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,23 +278,41 @@
         return 'select id from openk_semaforo.cliente where cpf = %s'
     elif connection_type.lower() == 'oracle':
         return 'SELECT ID FROM OPENK_SEMAFORO.CLIENTE WHERE CPF = :cpf '
     elif connection_type.lower() == 'sql':
         return 'select id from openk_semaforo.cliente where cpf = ?'
 
 
+def get_query_client_integrado_cpf(connection_type: str):
+    if connection_type.lower() == 'mysql':
+        return 'select id, cliente_erp from openk_semaforo.cliente where cpf = %s and cliente_erp is not null'
+    elif connection_type.lower() == 'oracle':
+        return 'SELECT ID, cliente_erp FROM OPENK_SEMAFORO.CLIENTE WHERE CPF = :cpf and cliente_erp is not null'
+    elif connection_type.lower() == 'sql':
+        return 'select id, cliente_erp from openk_semaforo.cliente where cpf = ? and cliente_erp is not null'
+
+
 def get_query_client_cnpj(connection_type: str):
     if connection_type.lower() == 'mysql':
         return 'select id from openk_semaforo.cliente where cnpj = %s'
     elif connection_type.lower() == 'oracle':
         return 'SELECT ID FROM OPENK_SEMAFORO.CLIENTE WHERE CNPJ = :cnpj '
     elif connection_type.lower() == 'sql':
         return 'select id from openk_semaforo.cliente where cnpj = ?'
 
 
+def get_query_client_integrado_cnpj(connection_type: str):
+    if connection_type.lower() == 'mysql':
+        return 'select id, cliente_erp from openk_semaforo.cliente where cnpj = %s and cliente_erp is not null'
+    elif connection_type.lower() == 'oracle':
+        return 'SELECT ID, cliente_erp FROM OPENK_SEMAFORO.CLIENTE WHERE CNPJ = :cnpj and cliente_erp is not null'
+    elif connection_type.lower() == 'sql':
+        return 'select id, cliente_erp from openk_semaforo.cliente where cnpj = ? and cliente_erp is not null'
+
+
 def get_insert_out_clients(connection_type: str) -> str:
     if connection_type.lower() == 'mysql':
         return '''insert into openk_semaforo.cliente (cliente_erp, data_alteracao, data_sincronizacao)
 					values (%s, %s, %s) '''
     elif connection_type.lower() == 'oracle':
         return '''INSERT INTO OPENK_SEMAFORO.CLIENTE (CLIENTE_ERP, DATA_ALTERACAO, DATA_SINCRONIZACAO)
 					VALUES (:1, :2, :3)'''
```

### Comparing `oking_oz-3.2.32/src/database/utils.py` & `oking_oz-3.2.33/src/database/utils.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/src/entities/invoice.py` & `oking_oz-3.2.33/src/entities/invoice.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/src/entities/order.py` & `oking_oz-3.2.33/src/entities/order.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/src/entities/orderb2b.py` & `oking_oz-3.2.33/src/entities/orderb2b.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/src/entities/orderb2c.py` & `oking_oz-3.2.33/src/entities/orderb2c.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/src/entities/pagamento.py` & `oking_oz-3.2.33/src/entities/pagamento.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/src/entities/product.py` & `oking_oz-3.2.33/src/entities/product.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/src/entities/response.py` & `oking_oz-3.2.33/src/entities/response.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/src/entities/tracking.py` & `oking_oz-3.2.33/src/entities/tracking.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/src/jobs/client_jobs.py` & `oking_oz-3.2.33/src/jobs/client_jobs.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/src/jobs/client_payment_plan_jobs.py` & `oking_oz-3.2.33/src/jobs/client_payment_plan_jobs.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/src/jobs/client_payment_plan_semaphore_jobs.py` & `oking_oz-3.2.33/src/jobs/client_payment_plan_semaphore_jobs.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/src/jobs/order_jobs.py` & `oking_oz-3.2.33/src/jobs/order_jobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -507,23 +507,23 @@
             conn.commit()
             conn.close()
 
             client_erp_code = ClienteErpCode(
                 cpf_cnpj=order.user.cpf if order.user.cnpj is None or order.user.cnpj == '' else order.user.cnpj,
                 codigo_cliente=client_erp_id)
 
-            send_log(job_config.get('job_name'), job_config.get('enviar_logs'), False,
+            send_log(job_config.get('job_name'), job_config.get('enviar_logs'), True,
                      f'Protocolando cliente via api okvendas com codigo_referencia {client_erp_id}', 'info', 'PEDIDO')
             updated_client_code = api_okvendas.put_client_erp_code(client_erp_code)
             if updated_client_code:
                 send_log(job_config.get('job_name'), job_config.get('enviar_logs'), False,
                          f'Codigo Erp do cliente atualizado via api OkVendas', 'info', 'PEDIDO')
             else:
-                send_log(job_config.get('job_name'), job_config.get('enviar_logs'), False,
-                         f'Falha ao atualizar o Codigo Erp do cliente via api OkVendas', 'warning', 'PEDIDO')
+                send_log(job_config.get('job_name'), job_config.get('enviar_logs'), True,
+                         f'Falha ao atualizar o Codigo Erp do cliente {client_erp_id} via api OkVendas', 'warning', 'PEDIDO')
 
         send_log(job_config.get('job_name'), job_config.get('enviar_logs'), False,
                  f'Removendo pedido da fila pelo protocolo {queue_order.protocol}', 'info', 'PEDIDO')
         protocoled_order = api_okvendas.put_protocol_orders([queue_order.protocol])
         if protocoled_order:
             send_log(job_config.get('job_name'), job_config.get('enviar_logs'), False,
                      f'Pedido protocolado via api OkVendas', 'info', 'PEDIDO')
@@ -927,22 +927,41 @@
 def insert_temp_b2b_order(job_config: dict, order: OrderB2B, db_config: DatabaseConfig) -> bool:
     step = ''
     db = database.Connection(db_config)
     conn = db.get_conect()
     try:
         step = 'conexao'
         cursor = conn.cursor()
-
+        # verificando se o cliente existe pelo cliente erp
         existent_client = None
         if order.user.erp_code is not None and order.user.erp_code != '' and order.user.erp_code != '0':  # Por padrao o erp_code vem = '0' da api okvendas
+            send_log(job_config.get('job_name'), job_config.get('enviar_logs'), False,
+                     f'Consultando id do cliente no banco semaforo pelo cliente erp', 'info', 'PEDIDO')
             cursor.execute(queries.get_query_client_erp(db_config.db_type),
                            queries.get_command_parameter(db_config.db_type, [order.user.erp_code]))
             existent_client = cursor.fetchone()
 
-        if existent_client is None:
+        # verificando se o cliente existe pelo cpf
+        if existent_client is None and order.user.cpf is not None and order.user.cpf != '':
+            send_log(job_config.get('job_name'), job_config.get('enviar_logs'), False,
+                     f'Verificando id do cliente integrado no banco semaforo pelo cpf', 'info', 'PEDIDO')
+            cursor.execute(queries.get_query_client_integrado_cpf(db_config.db_type),
+                       queries.get_command_parameter(db_config.db_type, [order.user.cpf]))
+
+            existent_client, order.user.erp_code = cursor.fetchone()
+        # verificando se o cliente existe pelo cnpj
+        elif existent_client is None and order.user.cnpj is not None and order.user.cnpj != '':
+            send_log(job_config.get('job_name'), job_config.get('enviar_logs'), False,
+                     f'Consultando id do cliente no banco semaforo pelo cnpj', 'info', 'PEDIDO')
+            cursor.execute(queries.get_query_client_integrado_cnpj(db_config.db_type),
+                       queries.get_command_parameter(db_config.db_type, [order.user.cnpj]))
+
+            existent_client, order.user.erp_code = cursor.fetchone()
+
+        if existent_client is None: # cliente não existe
             # insere cliente
             step = 'insere cliente'
             logger.info(f'')
             send_log(job_config.get('job_name'), job_config.get('enviar_logs'), False,
                      f'\tPedido {order.order_id}: Inserindo cliente', 'info', 'PEDIDO')
 
             erp_code = order.user.erp_code if order.user.erp_code is not None and order.user.erp_code not in ['', '0'] else None
@@ -966,16 +985,15 @@
                                order.user.address.state,
                                order.user.address.reference,
                                'IN',
                                order.user.state_registry,
                                order.user.address.ibge_code,
                                erp_code,
                            ]))
-        else:
-            # update no cliente existente
+        elif order.user.erp_code is not None and order.user.erp_code != '' and order.user.erp_code != '0': # cliente existe e verifica se o cliente erp esta preenchido
             step = 'update cliente'
             send_log(job_config.get('job_name'), job_config.get('enviar_logs'), False,
                      f'\tPedido {order.order_id}: Atualizando cliente existente', 'info', 'PEDIDO')
             cursor.execute(queries.get_update_b2b_client_sql(db_config.db_type),
                            queries.get_command_parameter(db_config.db_type, [
                                order.user.name,
                                order.user.company_name or order.user.name,
@@ -994,15 +1012,15 @@
                                order.user.address.state,
                                order.user.address.reference,
                                order.user.address.ibge_code,
                                order.user.state_registry,
                                order.user.erp_code
                            ]))
 
-        if cursor.rowcount > 0:
+        if cursor.rowcount > 0 or existent_client is not None:
             send_log(job_config.get('job_name'), job_config.get('enviar_logs'), False,
                      f'Cliente inserido/atualizado para o pedido {order.order_id}', 'info', 'PEDIDO')
             if order.user.erp_code is not None and order.user.erp_code not in ['', '0']:
                 send_log(job_config.get('job_name'), job_config.get('enviar_logs'), False,
                          f'Consultando id do cliente no banco semaforo pelo codigo erp', 'info', 'PEDIDO')
                 cursor.execute(queries.get_query_client_erp(db_config.db_type),
                                queries.get_command_parameter(db_config.db_type, [order.user.erp_code]))
```

### Comparing `oking_oz-3.2.32/src/jobs/price_jobs.py` & `oking_oz-3.2.33/src/jobs/price_jobs.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/src/jobs/products_jobs.py` & `oking_oz-3.2.33/src/jobs/products_jobs.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/src/jobs/representative_jobs.py` & `oking_oz-3.2.33/src/jobs/representative_jobs.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/src/jobs/stock_jobs.py` & `oking_oz-3.2.33/src/jobs/stock_jobs.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.32/src/jobs/system_jobs.py` & `oking_oz-3.2.33/src/jobs/system_jobs.py`

 * *Files identical despite different names*

