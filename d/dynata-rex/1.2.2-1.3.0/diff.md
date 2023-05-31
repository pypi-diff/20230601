# Comparing `tmp/dynata_rex-1.2.2.tar.gz` & `tmp/dynata_rex-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dynata_rex-1.2.2.tar", last modified: Fri Nov  4 14:29:29 2022, max compression
+gzip compressed data, was "dynata_rex-1.3.0.tar", last modified: Wed May 31 23:09:17 2023, max compression
```

## Comparing `dynata_rex-1.2.2.tar` & `dynata_rex-1.3.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)        0 2022-11-04 14:29:29.423381 dynata_rex-1.2.2/
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)    11376 2022-11-04 14:29:29.424017 dynata_rex-1.2.2/PKG-INFO
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)     8129 2022-11-04 14:28:45.000000 dynata_rex-1.2.2/README.md
-drwxr-xr-x   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)        0 2022-11-04 14:29:29.149702 dynata_rex-1.2.2/dynata_rex/
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)      661 2022-01-31 14:38:11.000000 dynata_rex-1.2.2/dynata_rex/__init__.py
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)      732 2022-01-31 14:38:11.000000 dynata_rex-1.2.2/dynata_rex/exceptions.py
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)     2029 2022-02-02 17:44:59.000000 dynata_rex-1.2.2/dynata_rex/helpers.py
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)      378 2022-01-31 14:38:11.000000 dynata_rex-1.2.2/dynata_rex/logs.py
-drwxr-xr-x   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)        0 2022-11-04 14:29:29.236243 dynata_rex-1.2.2/dynata_rex/models/
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)      809 2022-01-31 14:38:11.000000 dynata_rex-1.2.2/dynata_rex/models/__init__.py
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)     1126 2022-01-31 14:38:11.000000 dynata_rex-1.2.2/dynata_rex/models/base.py
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)     3373 2022-04-11 13:24:36.000000 dynata_rex-1.2.2/dynata_rex/models/opportunity_registry.py
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)     1503 2022-01-31 14:38:11.000000 dynata_rex-1.2.2/dynata_rex/models/respondent_gateway.py
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)     6197 2022-07-15 17:20:35.000000 dynata_rex-1.2.2/dynata_rex/opportunity_registry.py
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)    10513 2022-11-04 14:25:15.000000 dynata_rex-1.2.2/dynata_rex/respondent_gateway.py
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)     8715 2022-02-01 17:06:48.000000 dynata_rex-1.2.2/dynata_rex/signer.py
-drwxr-xr-x   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)        0 2022-11-04 14:29:29.199143 dynata_rex-1.2.2/dynata_rex.egg-info/
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)    11376 2022-11-04 14:29:28.000000 dynata_rex-1.2.2/dynata_rex.egg-info/PKG-INFO
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)     1776 2022-11-04 14:29:28.000000 dynata_rex-1.2.2/dynata_rex.egg-info/SOURCES.txt
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)        1 2022-11-04 14:29:28.000000 dynata_rex-1.2.2/dynata_rex.egg-info/dependency_links.txt
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)      174 2022-11-04 14:29:28.000000 dynata_rex-1.2.2/dynata_rex.egg-info/requires.txt
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)       20 2022-11-04 14:29:28.000000 dynata_rex-1.2.2/dynata_rex.egg-info/top_level.txt
-drwxr-xr-x   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)        0 2022-11-04 14:29:29.240109 dynata_rex-1.2.2/examples/
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)        0 2022-02-01 18:19:06.000000 dynata_rex-1.2.2/examples/__init__.py
-drwxr-xr-x   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)        0 2022-11-04 14:29:29.293584 dynata_rex-1.2.2/examples/opportunity_registry/
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)      111 2022-02-01 18:19:06.000000 dynata_rex-1.2.2/examples/opportunity_registry/01_instantiate_client.py
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)      280 2022-07-15 17:20:35.000000 dynata_rex-1.2.2/examples/opportunity_registry/02_receive_notifications.py
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)      267 2022-02-01 18:19:06.000000 dynata_rex-1.2.2/examples/opportunity_registry/03_convert_opportunity_json.py
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)      275 2022-07-15 17:20:35.000000 dynata_rex-1.2.2/examples/opportunity_registry/04_acknowledge_multiple_notifications.py
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)      236 2022-07-15 17:20:35.000000 dynata_rex-1.2.2/examples/opportunity_registry/05_acknowledge_single_notification.py
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)      329 2022-02-01 18:19:06.000000 dynata_rex-1.2.2/examples/opportunity_registry/06_list_corresponding_opportunities_by_project.py
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)      190 2022-02-01 18:19:06.000000 dynata_rex-1.2.2/examples/opportunity_registry/07_download_collection_type_cell.py
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)        0 2022-02-01 18:19:06.000000 dynata_rex-1.2.2/examples/opportunity_registry/__init__.py
-drwxr-xr-x   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)        0 2022-11-04 14:29:29.421607 dynata_rex-1.2.2/examples/respondent_gateway/
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)      106 2022-02-01 18:19:06.000000 dynata_rex-1.2.2/examples/respondent_gateway/01_instantiate_client.py
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)      392 2022-02-01 18:19:06.000000 dynata_rex-1.2.2/examples/respondent_gateway/02_create_signed_link.py
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)      447 2022-02-01 18:19:06.000000 dynata_rex-1.2.2/examples/respondent_gateway/03_create_quoted_signed_link.py
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)      948 2022-02-01 18:19:06.000000 dynata_rex-1.2.2/examples/respondent_gateway/04_create_survey_link_for_panelist.py
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)     1219 2022-02-01 18:19:06.000000 dynata_rex-1.2.2/examples/respondent_gateway/05_create_survey_link_for_panelist_with_custom_parameters.py
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)     1316 2022-02-01 18:19:06.000000 dynata_rex-1.2.2/examples/respondent_gateway/06_verify_signed_url.py
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)     1360 2022-02-01 18:19:06.000000 dynata_rex-1.2.2/examples/respondent_gateway/07_get_end_link_disposition.py
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)      353 2022-02-01 18:19:06.000000 dynata_rex-1.2.2/examples/respondent_gateway/08_create_context.py
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)      384 2022-02-01 18:19:06.000000 dynata_rex-1.2.2/examples/respondent_gateway/09_retrieve_context.py
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)      432 2022-02-01 18:19:06.000000 dynata_rex-1.2.2/examples/respondent_gateway/10_expire_context.py
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)      424 2022-07-15 17:20:35.000000 dynata_rex-1.2.2/examples/respondent_gateway/11_list_attributes.py
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)     1437 2022-05-02 15:14:12.000000 dynata_rex-1.2.2/examples/respondent_gateway/12_get_attribute_info.py
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)        0 2022-02-01 18:19:06.000000 dynata_rex-1.2.2/examples/respondent_gateway/__init__.py
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)       32 2022-07-15 17:20:35.000000 dynata_rex-1.2.2/requirements.txt
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)       79 2022-11-04 14:29:29.430174 dynata_rex-1.2.2/setup.cfg
--rw-r--r--   0 gino.trombetti (1418429374) DYNATACORP\Domain Users (1669268961)     1473 2022-11-04 14:26:05.000000 dynata_rex-1.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 23:09:17.701019 dynata_rex-1.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     9699 2023-05-31 23:09:17.702019 dynata_rex-1.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8929 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 23:09:17.694019 dynata_rex-1.3.0/dynata_rex/
+-rw-r--r--   0 root         (0) root         (0)      661 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/dynata_rex/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      732 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/dynata_rex/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2029 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/dynata_rex/helpers.py
+-rw-r--r--   0 root         (0) root         (0)      378 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/dynata_rex/logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 23:09:17.696019 dynata_rex-1.3.0/dynata_rex/models/
+-rw-r--r--   0 root         (0) root         (0)      989 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/dynata_rex/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/dynata_rex/models/base.py
+-rw-r--r--   0 root         (0) root         (0)     3526 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/dynata_rex/models/opportunity_registry.py
+-rw-r--r--   0 root         (0) root         (0)     3561 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/dynata_rex/models/respondent_gateway.py
+-rw-r--r--   0 root         (0) root         (0)     7668 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/dynata_rex/opportunity_registry.py
+-rw-r--r--   0 root         (0) root         (0)    11434 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/dynata_rex/respondent_gateway.py
+-rw-r--r--   0 root         (0) root         (0)     8715 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/dynata_rex/signer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 23:09:17.695019 dynata_rex-1.3.0/dynata_rex.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9699 2023-05-31 23:09:17.000000 dynata_rex-1.3.0/dynata_rex.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1767 2023-05-31 23:09:17.000000 dynata_rex-1.3.0/dynata_rex.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 23:09:17.000000 dynata_rex-1.3.0/dynata_rex.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      174 2023-05-31 23:09:17.000000 dynata_rex-1.3.0/dynata_rex.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-31 23:09:17.000000 dynata_rex-1.3.0/dynata_rex.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 23:09:17.697019 dynata_rex-1.3.0/examples/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 23:09:17.698019 dynata_rex-1.3.0/examples/opportunity_registry/
+-rw-r--r--   0 root         (0) root         (0)      111 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/opportunity_registry/01_instantiate_client.py
+-rw-r--r--   0 root         (0) root         (0)      280 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/opportunity_registry/02_receive_notifications.py
+-rw-r--r--   0 root         (0) root         (0)      267 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/opportunity_registry/03_convert_opportunity_json.py
+-rw-r--r--   0 root         (0) root         (0)      275 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/opportunity_registry/04_acknowledge_multiple_notifications.py
+-rw-r--r--   0 root         (0) root         (0)      236 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/opportunity_registry/05_acknowledge_single_notification.py
+-rw-r--r--   0 root         (0) root         (0)      329 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/opportunity_registry/06_list_corresponding_opportunities_by_project.py
+-rw-r--r--   0 root         (0) root         (0)      190 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/opportunity_registry/07_download_collection_type_cell.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/opportunity_registry/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 23:09:17.701019 dynata_rex-1.3.0/examples/respondent_gateway/
+-rw-r--r--   0 root         (0) root         (0)      106 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/respondent_gateway/01_instantiate_client.py
+-rw-r--r--   0 root         (0) root         (0)      392 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/respondent_gateway/02_create_signed_link.py
+-rw-r--r--   0 root         (0) root         (0)      447 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/respondent_gateway/03_create_quoted_signed_link.py
+-rw-r--r--   0 root         (0) root         (0)      948 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/respondent_gateway/04_create_survey_link_for_panelist.py
+-rw-r--r--   0 root         (0) root         (0)     1219 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/respondent_gateway/05_create_survey_link_for_panelist_with_custom_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     1316 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/respondent_gateway/06_verify_signed_url.py
+-rw-r--r--   0 root         (0) root         (0)     1360 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/respondent_gateway/07_get_end_link_disposition.py
+-rw-r--r--   0 root         (0) root         (0)      353 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/respondent_gateway/08_create_context.py
+-rw-r--r--   0 root         (0) root         (0)      384 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/respondent_gateway/09_retrieve_context.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/respondent_gateway/10_expire_context.py
+-rw-r--r--   0 root         (0) root         (0)      424 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/respondent_gateway/11_list_attributes.py
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/respondent_gateway/12_get_attribute_info.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/respondent_gateway/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       79 2023-05-31 23:09:17.703019 dynata_rex-1.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1473 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/setup.py
```

### Comparing `dynata_rex-1.2.2/README.md` & `dynata_rex-1.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -13,80 +13,80 @@
 #### Instantiate a Registry Client
 
 ```py
 from dynata_rex import OpportunityRegistry
 registry = OpportunityRegistry('rex_access_key', 'rex_secret_key')
 ```
 
-### List opportunity notifications from the registry
+#### List opportunity notifications from the registry
 
 ```py
 opportunities = registry.receive_notifications()
 
 
 # [Opportunity(id=1,...), Opportunity(id=2,...), Opportunity(id=1,...)]
 ```
 
-### Convert an opportunity to JSON
+#### Convert an opportunity to JSON
 
 ```py
 opportunity_json = Opportunity.json()
 ```
 
-### Acknowledge a list of notifications from the registry
+#### Acknowledge a list of notifications from the registry
 
 ```py
 registry.ack_notifications([opportunity_1.id, ..., opportunity_N.id])
 ```
-### Acknowledge a single notification from the registry
+#### Acknowledge a single notification from the registry
 ```
 registry.ack_notification(opportunity.id)
 ```
 
-### Get a list of corresponding opportunities from a project_id
+#### Get a list of corresponding opportunities from a project_id
 
 ```py
 corresponding = registry.list_project_opportunities(opportunity.project_id)
 
 # [12345, 45678, 78901]
 ```
 
-### Download a collection from a collection-type targeting cell
+#### Download a collection from a collection-type targeting cell
 
 ```py
 data = registry.download_collection(cell.collection_id)
 ```
 
 ---
 
 ### _**Respondent Gateway**_
 
-### Instantiate a RespondentGateway Client
+#### Instantiate a RespondentGateway Client
 
 ```py
 from dynata_rex import RespondentGateway
 gateway = RespondentGateway('rex_access_key', 'rex_secret_key')
 ```
 
-### Create a survey link for your respondent
+#### Create a survey link for your respondent
 
 ```py
 url = 'https://respondent.fake.rex.dynata.com/start?ctx=XXXX&language=en'
 
 signed_link = gateway.create_respondent_url(url,
                                             '1990-01-01',
                                             'male',
                                             '90210',
                                             'very-unique-respondent-id',
 
                                             ttl=60)
 # https://respondent.fake.rex.dynata.com/start?ctx=XXXX&language=en&birth_date=1990-01-01&gender=male&postal_code=90210&respondent_id=very-unique-respondent-id&access_key=rex_access_key&expiration=2021-11-29T15:35:12.993Z&signature=4353e8c4ca8f8fb75530214ac78139b55ca3f090438c639476b8584afe1396e6
 ```
 
-### Add additional query parameters to a link that will be present on return from survey
+#### Add additional query parameters to a link that will be present on return from survey
 
 ```py
 url = 'https://respondent.fake.rex.dynata.com/start?ctx=XXXX&language=en'
 
 custom_params = {
     'custom_parameter': 'custom_value',
     'another_custom_parameter': 'another_custom_value'
@@ -99,24 +99,24 @@
                                             'very-unique-respondent-id',
                                             additional_params=custom_params,
                                             ttl=60)
 
 # https://respondent.fake.rex.dynata.com/start?ctx=XXXX&language=en&custom_parameter=custom_value&another_custom_parameter=another_custom_value&birth_date=1990-01-01&gender=male&postal_code=90210&respondent_id=very-unique-respondent-id&access_key=rex_access_key&expiration=2021-12-02T13:48:55.759Z&signature=cf443326b73fb8af14c590e18d79a970fc3f73327c2d140c324ee1ce3020d064
 ```
 
-### Sign an inbound /start link with your credentials
+#### Sign an inbound /start link with your credentials
 
 ```py
 url = 'https://respondent.fake.rex.dynata.com/start?ctx=XXXX&language=en'
 signed_url = gateway.sign_url(url)
 
 # "https://respondent.fake.rex.dynata.com/start?ctx=XXXX&language=en&access_key=rex_access_key&expiration=2021-11-24T16:12:06.070Z&signature=fa8b5cac82d34bcf8026904b353349db5b1b871f735e07a601389cb6da2d744d"
 ```
 
-### Generate a URL-quoted signed url
+#### Generate a URL-quoted signed url
 
 ```py
 signed_url = gateway.sign_url(url, url_quoting=True)
 
 # 'https://respondent.fake.rex.dynata.com/start?ctx=XXXX&language=en&access_key=rex_access_key&expiration=2021-11-24T16%3A12%3A35.991Z&signature=4219cf63406ae429d94dbe9c33027816c264c1e2bf1edbadd2510eb9bf2351c3'
 ```
 
@@ -205,15 +205,15 @@
 
 # 'super-unique-ctx-id'
 ```
 
 ##### Retrieve a context
 
 ```py
-gw.get_context('super-unique-ctx-id')
+gateway.get_context('super-unique-ctx-id')
 
 # {
 #    'id': 'super-unique-ctx-id',
 #    'items': {
 #        'ctx': 'parent-context-id',
 #        'gender': 'male',
 #        'birth_data': '1999-09-09',
@@ -221,15 +221,15 @@
 #     }
 # }
 ```
 
 ##### Expire a context
 
 ```py
-gw.expire_context('super-unique-ctx-id')
+gateway.expire_context('super-unique-ctx-id')
 
 # {
 #    'id': 'super-unique-ctx-id',
 #    'items': {
 #        'ctx': 'parent-context-id',
 #        'gender': 'male',
 #        'birth_data': '1999-09-09',
@@ -238,15 +238,15 @@
 #     'expiration': '2021-11-30T16:10:44Z'
 # }
 ```
 
 ##### List Attributes
 
 ```py
-gw.list_attributes('country', 'page_number', 'page_size')
+gateway.list_attributes('country', 'page_number', 'page_size')
 
 # {
 #    'data':
 #    [
 #       {
 #           'active': true,
 #           'parameter_id": 402
@@ -254,15 +254,15 @@
 #    ]
 # }
 ```
 
 ##### Get Attribute Info
 
 ```py
-gw.get_attribute_info('attribute-id')
+gateway.get_attribute_info('attribute-id')
 
 # {
 #   'id': 402,
 #   'name': "This Parameter",
 #   'description': "Details of what this is",
 #   'display_mode: "N" (Optional),
 #   'parent_dependencies':
@@ -305,7 +305,38 @@
 #                   'locale': "GB",
 #                   'text': "Other language"
 #           ]
 #       }
 #   ]
 # }
 ```
+
+#### put respondent
+
+```python
+from dynata_rex.models import PutRespondentRequest, Attribute
+
+respondent = PutRespondentRequest(
+    respondent_id="respondent_id",
+    gender="gender", # str | None
+    country="country",
+    language="language",
+    birth_date="birth_date", # str | None
+    attributes= [Attribute(attribute_id=111, answers=[111, 222, 333])],
+    postal_code="postal_code" # str | None
+)
+
+gateway.put_respondent(respondent)
+```
+
+#### put respondent answers
+
+```python
+from dynata_rex.models import PutRespondentAnswersRequest, Attribute
+
+respondent_answers = PutRespondentAnswersRequest(
+    respondent_id="respondent_id",
+    attributes= [Attribute(attribute_id=111, answers=[111, 222, 333])]
+)
+
+gateway.put_respondent_answers(respondent_answers)
+```
```

### Comparing `dynata_rex-1.2.2/dynata_rex/__init__.py` & `dynata_rex-1.3.0/dynata_rex/__init__.py`

 * *Files identical despite different names*

### Comparing `dynata_rex-1.2.2/dynata_rex/exceptions.py` & `dynata_rex-1.3.0/dynata_rex/exceptions.py`

 * *Files identical despite different names*

### Comparing `dynata_rex-1.2.2/dynata_rex/helpers.py` & `dynata_rex-1.3.0/dynata_rex/helpers.py`

 * *Files identical despite different names*

### Comparing `dynata_rex-1.2.2/dynata_rex/models/base.py` & `dynata_rex-1.3.0/dynata_rex/models/base.py`

 * *Files identical despite different names*

### Comparing `dynata_rex-1.2.2/dynata_rex/models/opportunity_registry.py` & `dynata_rex-1.3.0/dynata_rex/models/opportunity_registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -129,15 +129,14 @@
 
 class Filter(HashableModel):
     id: str
     cells: List[str]
 
 
 class Opportunity(HashableModel):
-
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         allow_mutation = False
 
     id: int
     status: StatusEnum
@@ -156,7 +155,16 @@
     project_exclusions: List[int]
     category_exclusions: List[CategoryEnum]
     category_ids: List[CategoryEnum]
     devices: List[DevicesEnum]
     filters: List[List[Filter]]
     cells: List[Union[RangeCell, ListCell, ValueCell, CollectionCell]]
     quotas: List[List[Quota]]
+
+
+class Invite(HashableModel):
+    id: int
+    collection_id: str
+    respondent_id: str
+    expiration: Optional[int]
+    modified: str
+    created: str
```

### Comparing `dynata_rex-1.2.2/dynata_rex/opportunity_registry.py` & `dynata_rex-1.3.0/dynata_rex/opportunity_registry.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 import dynata_rex.models as models
 from .signer import RexRequest
 from .logs import logger
 from .exceptions import InvalidShardException
 
 
 class OpportunityRegistry:
-
     _BASE_URL = 'https://registry.rex.dynata.com'
 
     def __init__(self,
                  access_key: str,
                  secret_key: str,
                  base_url: str = _BASE_URL,
                  default_ttl: int = 10,
@@ -86,14 +85,22 @@
             "shards": {
                 "count": self.shard_count,
                 "current": self.current_shard
             }
         }
         return self.make_request.post(endpoint, data)
 
+    def _receive_invites(self, limit: int = 10) -> list[dict]:
+        """Raw receive invites"""
+        endpoint = f"{self.base_url}/receive_invites"
+        data = {
+            "limit": limit
+        }
+        return self.make_request.post(endpoint, data)
+
     def list_opportunities(self, limit: int = 10) -> List[models.Opportunity]:
         """
         [Deprecated - please use receive_notifications()]
         Get opportunities from Opportunity Registry"""
         opportunities = self._list_opportunities(limit=limit)
         out = []
         for opp in opportunities:
@@ -167,7 +174,36 @@
 
     def download_collection(self, collection_id: str) -> list:
         """Download targeting from a collection cell"""
         endpoint = f"{self.base_url}/download-collection"
         data = {"id": str(collection_id)}
         res = self.make_request.post(endpoint, data)
         return str(res).split('\n')
+
+    def ack_invites(self, invites: list[int]) -> None:
+        """Acknowledge a list of invites"""
+        endpoint = f"{self.base_url}/ack-invites"
+        res = self.make_request.post(endpoint, invites)
+        return res
+
+    def receive_invites(self, limit: int = 10) -> List[models.Invite]:
+        """Receive invites from opportunity registry"""
+        invites = self._receive_invites(limit=limit)
+        out = []
+        for inv in invites:
+            try:
+                out.append(models.Invite(**inv))
+            except pydantic.error_wrappers.ValidationError:
+                invite_id = inv['id']
+                logger.warning(
+                    f"Unable to parse {invite_id}, excluding...")
+                logger.warning(json.dumps(inv, indent=4))
+                # Ack invites so we don't see it again
+                self.ack_invites(invite_id)
+        return out
+
+    def download_invite_collection(self, invite_id: str) -> list:
+        """Download invite collection from opportunity registry"""
+        endpoints = f"{self.base_url}/download-invite-collection"
+        data = {"id": invite_id}
+        res = self.make_request.post(endpoints, data)
+        return str(res).split('\n')
```

### Comparing `dynata_rex-1.2.2/dynata_rex/respondent_gateway.py` & `dynata_rex-1.3.0/dynata_rex/respondent_gateway.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 from urllib.parse import urlparse, parse_qsl, unquote, urlencode
 from typing import Union
 from copy import copy
 
 # Third Party Imports
 
 # Local Imports
-from dynata_rex.models import GatewayDispositionsEnum, GatewayStatusEnum
+from dynata_rex.models import GatewayDispositionsEnum, \
+    GatewayStatusEnum, \
+    PutRespondentRequest, \
+    PutRespondentAnswersRequest
 from .signer import Signer, RexRequest
 from .exceptions import SignatureExpiredException, SignatureInvalidException
 
 
 class RespondentGateway:
     """
     Respondent Gateway interactions
@@ -295,7 +298,31 @@
         endpoint = f"{self.base_url}/list-attributes"
         data = {
             "country": country,
             "page_number": page_number,
             "page_size": page_size
         }
         return self.make_request.post(endpoint, data)
+
+    def put_respondent(self,
+                       request: PutRespondentRequest
+                       ) -> Union[dict, str]:
+        """
+        Create a respondent from its models.
+
+        :param request: Respondent model
+        :type request: PutRespondentRequest
+        """
+        endpoint = f"{self.base_url}/put-respondent"
+        return self.make_request.post(endpoint, request.to_json())
+
+    def put_respondent_answers(self,
+                               request: PutRespondentAnswersRequest
+                               ) -> Union[dict, str]:
+        """
+        Add answers to respondent.
+
+        :param request: Respondent answers model
+        :type request: PutRespondentAnswersRequest
+        """
+        endpoint = f"{self.base_url}/put-respondent-answers"
+        return self.make_request.post(endpoint, request.to_json())
```

### Comparing `dynata_rex-1.2.2/dynata_rex/signer.py` & `dynata_rex-1.3.0/dynata_rex/signer.py`

 * *Files identical despite different names*

### Comparing `dynata_rex-1.2.2/dynata_rex.egg-info/SOURCES.txt` & `dynata_rex-1.3.0/dynata_rex.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+LICENSE
 README.md
-requirements.txt
 setup.cfg
 setup.py
 dynata_rex/__init__.py
 dynata_rex/exceptions.py
 dynata_rex/helpers.py
 dynata_rex/logs.py
 dynata_rex/opportunity_registry.py
```

### Comparing `dynata_rex-1.2.2/examples/respondent_gateway/04_create_survey_link_for_panelist.py` & `dynata_rex-1.3.0/examples/respondent_gateway/04_create_survey_link_for_panelist.py`

 * *Files identical despite different names*

### Comparing `dynata_rex-1.2.2/examples/respondent_gateway/05_create_survey_link_for_panelist_with_custom_parameters.py` & `dynata_rex-1.3.0/examples/respondent_gateway/05_create_survey_link_for_panelist_with_custom_parameters.py`

 * *Files identical despite different names*

### Comparing `dynata_rex-1.2.2/examples/respondent_gateway/06_verify_signed_url.py` & `dynata_rex-1.3.0/examples/respondent_gateway/06_verify_signed_url.py`

 * *Files identical despite different names*

### Comparing `dynata_rex-1.2.2/examples/respondent_gateway/07_get_end_link_disposition.py` & `dynata_rex-1.3.0/examples/respondent_gateway/07_get_end_link_disposition.py`

 * *Files identical despite different names*

### Comparing `dynata_rex-1.2.2/examples/respondent_gateway/12_get_attribute_info.py` & `dynata_rex-1.3.0/examples/respondent_gateway/12_get_attribute_info.py`

 * *Files identical despite different names*

### Comparing `dynata_rex-1.2.2/setup.py` & `dynata_rex-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 
 setuptools.setup(
     name="dynata_rex",
-    version="1.2.2",
+    version="1.3.0",
     author="REX Maintainers",
     author_email="tech.supply@Dynata.com",
     description=("Package for building and interacting with the "
                  "Dynata Respondent Exchange (REX)"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dynata/rex-sdk-python",
@@ -21,19 +21,19 @@
     platforms=['Any'],
     install_requires=requirements,
     setup_requires=['pytest-runner'],
     extras_require={
         # pip install -e ".[testing]"
         "testing": ['pytest'],
         ':python_version == "3.6"': [
-            "typing-extensions==4.4.0",
+            "typing-extensions==4.6.2",
             'dataclasses==0.8'
         ],
         ':python_version == "3.7"': [
-            "typing-extensions==4.4.0"
+            "typing-extensions==4.6.2"
         ]
     },
     tests_require=['pytest'],
     keywords='respondent exchange rex smor dynata python',
     classifiers=[
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
```

