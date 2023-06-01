# Comparing `tmp/netbox-contract-2.0.0.tar.gz` & `tmp/netbox-contract-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-contract-2.0.0.tar", last modified: Thu May 25 20:33:15 2023, max compression
+gzip compressed data, was "netbox-contract-2.0.1.tar", last modified: Thu Jun  1 20:35:33 2023, max compression
```

## Comparing `netbox-contract-2.0.0.tar` & `netbox-contract-2.0.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-25 20:33:15.427488 netbox-contract-2.0.0/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1056 2023-01-03 17:10:18.000000 netbox-contract-2.0.0/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-03-12 14:44:04.000000 netbox-contract-2.0.0/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2299 2023-05-25 20:33:15.427488 netbox-contract-2.0.0/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1759 2023-03-12 15:14:54.000000 netbox-contract-2.0.0/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)      774 2023-05-25 20:27:44.000000 netbox-contract-2.0.0/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-05-25 20:33:15.427488 netbox-contract-2.0.0/setup.cfg
--rw-rw-r--   0 vscode    (1000) vscode    (1000)       52 2023-01-03 18:27:10.000000 netbox-contract-2.0.0/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-25 20:33:15.391487 netbox-contract-2.0.0/src/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-25 20:33:15.399487 netbox-contract-2.0.0/src/netbox_contract/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      469 2023-05-25 20:31:35.000000 netbox-contract-2.0.0/src/netbox_contract/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-25 20:33:15.407487 netbox-contract-2.0.0/src/netbox_contract/api/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/api/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4016 2023-05-25 20:01:58.000000 netbox-contract-2.0.0/src/netbox_contract/api/serializers.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      387 2023-05-23 17:57:34.000000 netbox-contract-2.0.0/src/netbox_contract/api/urls.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      955 2023-05-22 22:26:02.000000 netbox-contract-2.0.0/src/netbox_contract/api/views.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1369 2023-05-10 21:06:50.000000 netbox-contract-2.0.0/src/netbox_contract/filtersets.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5629 2023-05-16 21:07:49.000000 netbox-contract-2.0.0/src/netbox_contract/forms.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-25 20:33:15.419488 netbox-contract-2.0.0/src/netbox_contract/migrations/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4598 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/migrations/0001_initial.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      764 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/migrations/0002_alter_contract_circuit_and_more.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1579 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/migrations/0003_alter_contract_custom_field_data_and_more.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      601 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/migrations/0004_contract_currency_invoice_currency.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      584 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/migrations/0005_contract_accounting_dimensions_and_more.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      563 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/migrations/0006_alter_contract_circuit.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      403 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/migrations/0007_invoice_date.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      386 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/migrations/0008_invoice_comments.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      428 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/migrations/0009_contract_external_reference.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      494 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/migrations/0010_invoice_contracts.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/migrations/0011_auto_20230122_2112.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      339 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/migrations/0012_remove_invoice_contract.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      549 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      422 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/migrations/0014_contract_end_date.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2104 2023-05-13 17:53:07.000000 netbox-contract-2.0.0/src/netbox_contract/migrations/0015_contractassignement.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/migrations/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5517 2023-05-24 18:15:36.000000 netbox-contract-2.0.0/src/netbox_contract/models.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1644 2023-03-12 18:00:52.000000 netbox-contract-2.0.0/src/netbox_contract/navigation.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/search.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2700 2023-05-24 18:08:42.000000 netbox-contract-2.0.0/src/netbox_contract/tables.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1325 2023-05-23 21:14:03.000000 netbox-contract-2.0.0/src/netbox_contract/template_content.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-25 20:33:15.419488 netbox-contract-2.0.0/src/netbox_contract/templates/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      775 2023-05-23 19:02:53.000000 netbox-contract-2.0.0/src/netbox_contract/templates/contract_assignements_bottom.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)      305 2023-05-24 18:09:51.000000 netbox-contract-2.0.0/src/netbox_contract/templates/contract_list_bottom.html
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-25 20:33:15.423488 netbox-contract-2.0.0/src/netbox_contract/templates/netbox_contract/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4257 2023-05-23 21:01:17.000000 netbox-contract-2.0.0/src/netbox_contract/templates/netbox_contract/contract.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)      810 2023-05-22 21:27:25.000000 netbox-contract-2.0.0/src/netbox_contract/templates/netbox_contract/contract_assignement.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2284 2023-03-12 17:52:54.000000 netbox-contract-2.0.0/src/netbox_contract/templates/netbox_contract/invoice.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1128 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/templates/netbox_contract/serviceprovider.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3751 2023-05-23 19:01:13.000000 netbox-contract-2.0.0/src/netbox_contract/urls.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8384 2023-05-23 18:08:26.000000 netbox-contract-2.0.0/src/netbox_contract/views.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-25 20:33:15.403487 netbox-contract-2.0.0/src/netbox_contract.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2299 2023-05-25 20:33:15.000000 netbox-contract-2.0.0/src/netbox_contract.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2145 2023-05-25 20:33:15.000000 netbox-contract-2.0.0/src/netbox_contract.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-25 20:33:15.000000 netbox-contract-2.0.0/src/netbox_contract.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-02-19 10:47:00.000000 netbox-contract-2.0.0/src/netbox_contract.egg-info/not-zip-safe
--rw-r--r--   0 vscode    (1000) vscode    (1000)       16 2023-05-25 20:33:15.000000 netbox-contract-2.0.0/src/netbox_contract.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       16 2023-05-25 20:33:15.000000 netbox-contract-2.0.0/src/netbox_contract.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-01 20:35:33.739246 netbox-contract-2.0.1/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1056 2023-01-03 17:10:18.000000 netbox-contract-2.0.1/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-03-12 14:44:04.000000 netbox-contract-2.0.1/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2641 2023-06-01 20:35:33.739246 netbox-contract-2.0.1/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2102 2023-05-25 21:05:55.000000 netbox-contract-2.0.1/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      774 2023-06-01 20:33:56.000000 netbox-contract-2.0.1/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-06-01 20:35:33.739246 netbox-contract-2.0.1/setup.cfg
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)       52 2023-01-03 18:27:10.000000 netbox-contract-2.0.1/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-01 20:35:33.663245 netbox-contract-2.0.1/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-01 20:35:33.687245 netbox-contract-2.0.1/src/netbox_contract/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      469 2023-06-01 20:34:32.000000 netbox-contract-2.0.1/src/netbox_contract/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-01 20:35:33.707245 netbox-contract-2.0.1/src/netbox_contract/api/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/api/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4016 2023-05-25 20:01:58.000000 netbox-contract-2.0.1/src/netbox_contract/api/serializers.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      387 2023-05-23 17:57:34.000000 netbox-contract-2.0.1/src/netbox_contract/api/urls.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      955 2023-05-22 22:26:02.000000 netbox-contract-2.0.1/src/netbox_contract/api/views.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1369 2023-05-10 21:06:50.000000 netbox-contract-2.0.1/src/netbox_contract/filtersets.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5629 2023-05-16 21:07:49.000000 netbox-contract-2.0.1/src/netbox_contract/forms.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-01 20:35:33.727246 netbox-contract-2.0.1/src/netbox_contract/migrations/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4598 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/migrations/0001_initial.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      764 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/migrations/0002_alter_contract_circuit_and_more.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1579 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/migrations/0003_alter_contract_custom_field_data_and_more.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      601 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/migrations/0004_contract_currency_invoice_currency.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      584 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/migrations/0005_contract_accounting_dimensions_and_more.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      563 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/migrations/0006_alter_contract_circuit.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      403 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/migrations/0007_invoice_date.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      386 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/migrations/0008_invoice_comments.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      428 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/migrations/0009_contract_external_reference.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      494 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/migrations/0010_invoice_contracts.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/migrations/0011_auto_20230122_2112.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      339 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/migrations/0012_remove_invoice_contract.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      549 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      422 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/migrations/0014_contract_end_date.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2104 2023-05-13 17:53:07.000000 netbox-contract-2.0.1/src/netbox_contract/migrations/0015_contractassignement.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/migrations/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5517 2023-05-24 18:15:36.000000 netbox-contract-2.0.1/src/netbox_contract/models.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1644 2023-03-12 18:00:52.000000 netbox-contract-2.0.1/src/netbox_contract/navigation.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/search.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3712 2023-05-30 21:11:00.000000 netbox-contract-2.0.1/src/netbox_contract/tables.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2027 2023-06-01 20:32:56.000000 netbox-contract-2.0.1/src/netbox_contract/template_content.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-01 20:35:33.731246 netbox-contract-2.0.1/src/netbox_contract/templates/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      775 2023-05-23 19:02:53.000000 netbox-contract-2.0.1/src/netbox_contract/templates/contract_assignements_bottom.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      305 2023-05-24 18:09:51.000000 netbox-contract-2.0.1/src/netbox_contract/templates/contract_list_bottom.html
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-01 20:35:33.739246 netbox-contract-2.0.1/src/netbox_contract/templates/netbox_contract/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4257 2023-05-23 21:01:17.000000 netbox-contract-2.0.1/src/netbox_contract/templates/netbox_contract/contract.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      810 2023-05-22 21:27:25.000000 netbox-contract-2.0.1/src/netbox_contract/templates/netbox_contract/contract_assignement.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2284 2023-03-12 17:52:54.000000 netbox-contract-2.0.1/src/netbox_contract/templates/netbox_contract/invoice.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1128 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/templates/netbox_contract/serviceprovider.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3751 2023-05-23 19:01:13.000000 netbox-contract-2.0.1/src/netbox_contract/urls.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8388 2023-05-30 21:08:13.000000 netbox-contract-2.0.1/src/netbox_contract/views.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-01 20:35:33.699245 netbox-contract-2.0.1/src/netbox_contract.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2641 2023-06-01 20:35:33.000000 netbox-contract-2.0.1/src/netbox_contract.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2145 2023-06-01 20:35:33.000000 netbox-contract-2.0.1/src/netbox_contract.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-01 20:35:33.000000 netbox-contract-2.0.1/src/netbox_contract.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-02-19 10:47:00.000000 netbox-contract-2.0.1/src/netbox_contract.egg-info/not-zip-safe
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       16 2023-06-01 20:35:33.000000 netbox-contract-2.0.1/src/netbox_contract.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       16 2023-06-01 20:35:33.000000 netbox-contract-2.0.1/src/netbox_contract.egg-info/top_level.txt
```

### Comparing `netbox-contract-2.0.0/LICENSE` & `netbox-contract-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.0/PKG-INFO` & `netbox-contract-2.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-contract
-Version: 2.0.0
+Version: 2.0.1
 Summary: Contract management plugin for Netbox
 Author-email: Marc Lebreuil <marc@famillelebreuil.net>
 Project-URL: Homepage, https://github.com/mlebreuil/netbox-contract
 Project-URL: Bug Tracker, https://github.com/mlebreuil/netbox-contract/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -74,7 +74,13 @@
 
 ### Run database migrations
 
 ```bash
 (venv) $ cd /opt/netbox/netbox/
 (venv) $ python3 manage.py migrate
 ```
+
+## release notes
+
+### version 2.0.0
+
+Add a new contract asignement model to allow the assignement of contract not only to Circuits. The support for the direct Contract to Circuit relation will be removed in version 2.1.0 . In Order to migrate existing relations contract_migration.py script is provided and can be run from the django shell.
```

### Comparing `netbox-contract-2.0.0/README.md` & `netbox-contract-2.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -59,8 +59,14 @@
 ```
 
 ### Run database migrations
 
 ```bash
 (venv) $ cd /opt/netbox/netbox/
 (venv) $ python3 manage.py migrate
-```
+```
+
+## release notes
+
+### version 2.0.0
+
+Add a new contract asignement model to allow the assignement of contract not only to Circuits. The support for the direct Contract to Circuit relation will be removed in version 2.1.0 . In Order to migrate existing relations contract_migration.py script is provided and can be run from the django shell.
```

### Comparing `netbox-contract-2.0.0/pyproject.toml` & `netbox-contract-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "netbox-contract"
-version = "2.0.0"
+version = "2.0.1"
 authors = [
   { name="Marc Lebreuil", email="marc@famillelebreuil.net" },
 ]
 description = "Contract management plugin for Netbox"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `netbox-contract-2.0.0/src/netbox_contract/api/serializers.py` & `netbox-contract-2.0.1/src/netbox_contract/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.0/src/netbox_contract/api/views.py` & `netbox-contract-2.0.1/src/netbox_contract/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.0/src/netbox_contract/filtersets.py` & `netbox-contract-2.0.1/src/netbox_contract/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.0/src/netbox_contract/forms.py` & `netbox-contract-2.0.1/src/netbox_contract/forms.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.0/src/netbox_contract/migrations/0001_initial.py` & `netbox-contract-2.0.1/src/netbox_contract/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.0/src/netbox_contract/migrations/0002_alter_contract_circuit_and_more.py` & `netbox-contract-2.0.1/src/netbox_contract/migrations/0002_alter_contract_circuit_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.0/src/netbox_contract/migrations/0003_alter_contract_custom_field_data_and_more.py` & `netbox-contract-2.0.1/src/netbox_contract/migrations/0003_alter_contract_custom_field_data_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.0/src/netbox_contract/migrations/0004_contract_currency_invoice_currency.py` & `netbox-contract-2.0.1/src/netbox_contract/migrations/0004_contract_currency_invoice_currency.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.0/src/netbox_contract/migrations/0005_contract_accounting_dimensions_and_more.py` & `netbox-contract-2.0.1/src/netbox_contract/migrations/0005_contract_accounting_dimensions_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.0/src/netbox_contract/migrations/0006_alter_contract_circuit.py` & `netbox-contract-2.0.1/src/netbox_contract/migrations/0006_alter_contract_circuit.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.0/src/netbox_contract/migrations/0011_auto_20230122_2112.py` & `netbox-contract-2.0.1/src/netbox_contract/migrations/0011_auto_20230122_2112.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.0/src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py` & `netbox-contract-2.0.1/src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.0/src/netbox_contract/migrations/0015_contractassignement.py` & `netbox-contract-2.0.1/src/netbox_contract/migrations/0015_contractassignement.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.0/src/netbox_contract/models.py` & `netbox-contract-2.0.1/src/netbox_contract/models.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.0/src/netbox_contract/navigation.py` & `netbox-contract-2.0.1/src/netbox_contract/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.0/src/netbox_contract/search.py` & `netbox-contract-2.0.1/src/netbox_contract/search.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.0/src/netbox_contract/tables.py` & `netbox-contract-2.0.1/src/netbox_contract/tables.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,16 +17,46 @@
     )
     actions = columns.ActionsColumn(
         actions=('edit', 'delete')
     )
 
     class Meta(NetBoxTable.Meta):
         model = ContractAssignement
-        fields = ('pk', 'content_type', 'content_object', 'contract', 'actions')
-        default_columns = ('pk', 'content_type', 'content_object', 'contract')
+        fields = ('pk', 'content_type', 'content_object', 'contract','contract__external_partie', 'actions')
+        default_columns = ('pk', 'content_type', 'content_object', 'contract','contract__external_partie')
+
+class ContractAssignementObjectTable(NetBoxTable):
+    contract = tables.Column(
+        linkify=True
+    )
+    actions = columns.ActionsColumn(
+        actions=('edit', 'delete')
+    )
+
+    class Meta(NetBoxTable.Meta):
+        model = ContractAssignement
+        fields = ('pk','contract','contract__external_partie','contract__status', 'actions')
+        default_columns = ('pk', 'contract','contract__external_partie','contract__status')
+
+class ContractAssignementContractTable(NetBoxTable):
+    content_type = columns.ContentTypeColumn(
+        verbose_name='Object Type'
+    )
+    content_object = tables.Column(
+        linkify=True,
+        orderable=False
+    )
+    actions = columns.ActionsColumn(
+        actions=('edit', 'delete')
+    )
+
+    class Meta(NetBoxTable.Meta):
+        model = ContractAssignement
+        fields = ('pk', 'content_type', 'content_object','actions')
+        default_columns = ('pk', 'content_type', 'content_object')
 
 class ContractListTable(NetBoxTable):
 
     name = tables.Column(
         linkify=True
     )
     external_partie = tables.Column(
```

### Comparing `netbox-contract-2.0.0/src/netbox_contract/template_content.py` & `netbox-contract-2.0.1/src/netbox_contract/template_content.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from django.contrib.contenttypes.models import ContentType
 from extras.plugins import PluginTemplateExtension
 from circuits.models import Circuit
+from dcim.models import Device
 from .models import ContractAssignement
 from . import tables
 
 class CircuitContracts(PluginTemplateExtension):
     model = 'circuits.circuit'
 
     def full_width_page(self):
@@ -19,15 +20,29 @@
 class CircuitContractAssignements(PluginTemplateExtension):
     model = 'circuits.circuit'
 
     def full_width_page(self):
         circuit = self.context['object']
         circuit_type = ContentType.objects.get_for_model(Circuit)
         contract_assignements = ContractAssignement.objects.filter(content_type__pk=circuit_type.id, object_id=circuit.id)
-        assignements_table = tables.ContractAssignementListTable(contract_assignements)
+        assignements_table = tables.ContractAssignementObjectTable(contract_assignements)
         assignements_table.configure(self.context['request'])
 
         return self.render('contract_assignements_bottom.html', extra_context={
             'assignements_table': assignements_table,
         })
 
-template_extensions = [ CircuitContracts, CircuitContractAssignements]
+class DeviceContractAssignements(PluginTemplateExtension):
+    model = 'dcim.device'
+
+    def full_width_page(self):
+        device = self.context['object']
+        device_type = ContentType.objects.get_for_model(Device)
+        contract_assignements = ContractAssignement.objects.filter(content_type__pk=device_type.id, object_id=device.id)
+        assignements_table = tables.ContractAssignementObjectTable(contract_assignements)
+        assignements_table.configure(self.context['request'])
+
+        return self.render('contract_assignements_bottom.html', extra_context={
+            'assignements_table': assignements_table,
+        })
+
+template_extensions = [ CircuitContracts, CircuitContractAssignements, DeviceContractAssignements]
```

### Comparing `netbox-contract-2.0.0/src/netbox_contract/templates/contract_assignements_bottom.html` & `netbox-contract-2.0.1/src/netbox_contract/templates/contract_assignements_bottom.html`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.0/src/netbox_contract/templates/netbox_contract/contract.html` & `netbox-contract-2.0.1/src/netbox_contract/templates/netbox_contract/contract.html`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.0/src/netbox_contract/templates/netbox_contract/contract_assignement.html` & `netbox-contract-2.0.1/src/netbox_contract/templates/netbox_contract/contract_assignement.html`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.0/src/netbox_contract/templates/netbox_contract/invoice.html` & `netbox-contract-2.0.1/src/netbox_contract/templates/netbox_contract/invoice.html`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.0/src/netbox_contract/templates/netbox_contract/serviceprovider.html` & `netbox-contract-2.0.1/src/netbox_contract/templates/netbox_contract/serviceprovider.html`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.0/src/netbox_contract/urls.py` & `netbox-contract-2.0.1/src/netbox_contract/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.0/src/netbox_contract/views.py` & `netbox-contract-2.0.1/src/netbox_contract/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     queryset = models.Contract.objects.all()
 
     def get_extra_context(self, request, instance):
         invoices_table = tables.InvoiceListTable(instance.invoices.all())
         invoices_table.configure(request)
         circuit_table = tables.ContractCircuitListTable(instance.circuit.all())
         circuit_table.configure(request)
-        assignements_table = tables.ContractAssignementListTable(instance.assignments.all())
+        assignements_table = tables.ContractAssignementContractTable(instance.assignments.all())
         assignements_table.configure(request)
 
         return {
             'invoices_table': invoices_table,
             'circuit_table': circuit_table,
             'assignements_table': assignements_table,
         }
```

### Comparing `netbox-contract-2.0.0/src/netbox_contract.egg-info/PKG-INFO` & `netbox-contract-2.0.1/src/netbox_contract.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-contract
-Version: 2.0.0
+Version: 2.0.1
 Summary: Contract management plugin for Netbox
 Author-email: Marc Lebreuil <marc@famillelebreuil.net>
 Project-URL: Homepage, https://github.com/mlebreuil/netbox-contract
 Project-URL: Bug Tracker, https://github.com/mlebreuil/netbox-contract/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -74,7 +74,13 @@
 
 ### Run database migrations
 
 ```bash
 (venv) $ cd /opt/netbox/netbox/
 (venv) $ python3 manage.py migrate
 ```
+
+## release notes
+
+### version 2.0.0
+
+Add a new contract asignement model to allow the assignement of contract not only to Circuits. The support for the direct Contract to Circuit relation will be removed in version 2.1.0 . In Order to migrate existing relations contract_migration.py script is provided and can be run from the django shell.
```

### Comparing `netbox-contract-2.0.0/src/netbox_contract.egg-info/SOURCES.txt` & `netbox-contract-2.0.1/src/netbox_contract.egg-info/SOURCES.txt`

 * *Files identical despite different names*

