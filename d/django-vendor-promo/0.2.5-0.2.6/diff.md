# Comparing `tmp/django-vendor-promo-0.2.5.tar.gz` & `tmp/django-vendor-promo-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-vendor-promo-0.2.5.tar", last modified: Wed May 31 02:21:56 2023, max compression
+gzip compressed data, was "django-vendor-promo-0.2.6.tar", last modified: Thu Jun  1 02:54:59 2023, max compression
```

## Comparing `django-vendor-promo-0.2.5.tar` & `django-vendor-promo-0.2.6.tar`

### file list

```diff
@@ -1,76 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:21:56.195092 django-vendor-promo-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/LICENSE.mit.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-31 02:21:56.195092 django-vendor-promo-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 02:21:56.199092 django-vendor-promo-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:21:56.187091 django-vendor-promo-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:21:56.187091 django-vendor-promo-0.2.5/src/django_vendor_promo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-31 02:21:56.000000 django-vendor-promo-0.2.5/src/django_vendor_promo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-31 02:21:56.000000 django-vendor-promo-0.2.5/src/django_vendor_promo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 02:21:56.000000 django-vendor-promo-0.2.5/src/django_vendor_promo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-31 02:21:56.000000 django-vendor-promo-0.2.5/src/django_vendor_promo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-31 02:21:56.000000 django-vendor-promo-0.2.5/src/django_vendor_promo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:21:56.191091 django-vendor-promo-0.2.5/src/vendorpromo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:21:56.191091 django-vendor-promo-0.2.5/src/vendorpromo/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:21:56.191091 django-vendor-promo-0.2.5/src/vendorpromo/api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/api/v1/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:21:56.191091 django-vendor-promo-0.2.5/src/vendorpromo/api/v1/vouchery/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/api/v1/vouchery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/api/v1/vouchery/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/api/v1/vouchery/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/integrations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:21:56.191091 django-vendor-promo-0.2.5/src/vendorpromo/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/migrations/0002_affiliate_couponcode_promotionalcampaign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/migrations/0003_auto_20230524_1701.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/migrations/0004_affiliate_name_type.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:21:56.195092 django-vendor-promo-0.2.5/src/vendorpromo/processors/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/processors/DummyProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/processors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/processors/stripe.py
--rw-r--r--   0 runner    (1001) docker     (123)    17456 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/processors/vouchery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:21:56.187091 django-vendor-promo-0.2.5/src/vendorpromo/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:21:56.195092 django-vendor-promo-0.2.5/src/vendorpromo/templates/vendorpromo/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/templates/vendorpromo/affiliate_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/templates/vendorpromo/affiliate_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/templates/vendorpromo/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/templates/vendorpromo/coupon_code_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/templates/vendorpromo/coupon_code_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:21:56.195092 django-vendor-promo-0.2.5/src/vendorpromo/templates/vendorpromo/includes/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/templates/vendorpromo/includes/promocode_apply.html
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/templates/vendorpromo/processor_site_config.html
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/templates/vendorpromo/processor_site_config_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/templates/vendorpromo/promo.html
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/templates/vendorpromo/promo_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/templates/vendorpromo/promocode_formset.html
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/templates/vendorpromo/promotional_campaign_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/templates/vendorpromo/promotional_campaign_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/templates/vendorpromo/vouchery_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/templates/vendorpromo/vouchery_integration.html
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/templates/vendorpromo/vouchery_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:21:56.195092 django-vendor-promo-0.2.5/src/vendorpromo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/tests/test_affiliate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/tests/test_coupon_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    21273 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/tests/test_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/tests/test_promo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/tests/test_promotional_campaign.py
--rw-r--r--   0 runner    (1001) docker     (123)    20938 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/tests/test_stripe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15017 2023-05-31 02:20:31.000000 django-vendor-promo-0.2.5/src/vendorpromo/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:54:59.883942 django-vendor-promo-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/LICENSE.mit.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-01 02:54:59.883942 django-vendor-promo-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 02:54:59.883942 django-vendor-promo-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:54:59.871942 django-vendor-promo-0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:54:59.871942 django-vendor-promo-0.2.6/src/django_vendor_promo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-01 02:54:59.000000 django-vendor-promo-0.2.6/src/django_vendor_promo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-01 02:54:59.000000 django-vendor-promo-0.2.6/src/django_vendor_promo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 02:54:59.000000 django-vendor-promo-0.2.6/src/django_vendor_promo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-01 02:54:59.000000 django-vendor-promo-0.2.6/src/django_vendor_promo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 02:54:59.000000 django-vendor-promo-0.2.6/src/django_vendor_promo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:54:59.875942 django-vendor-promo-0.2.6/src/vendorpromo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:54:59.875942 django-vendor-promo-0.2.6/src/vendorpromo/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:54:59.875942 django-vendor-promo-0.2.6/src/vendorpromo/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/api/v1/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:54:59.879942 django-vendor-promo-0.2.6/src/vendorpromo/api/v1/vouchery/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/api/v1/vouchery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/api/v1/vouchery/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/api/v1/vouchery/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/integrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:54:59.879942 django-vendor-promo-0.2.6/src/vendorpromo/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/migrations/0002_affiliate_couponcode_promotionalcampaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/migrations/0003_auto_20230524_1701.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/migrations/0004_affiliate_name_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/migrations/0005_alter_couponcode_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:54:59.879942 django-vendor-promo-0.2.6/src/vendorpromo/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/processors/DummyProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/processors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/processors/stripe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17456 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/processors/vouchery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:54:59.871942 django-vendor-promo-0.2.6/src/vendorpromo/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:54:59.883942 django-vendor-promo-0.2.6/src/vendorpromo/templates/vendorpromo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/templates/vendorpromo/affiliate_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/templates/vendorpromo/affiliate_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/templates/vendorpromo/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/templates/vendorpromo/coupon_code_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/templates/vendorpromo/coupon_code_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:54:59.883942 django-vendor-promo-0.2.6/src/vendorpromo/templates/vendorpromo/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/templates/vendorpromo/includes/promocode_apply.html
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/templates/vendorpromo/processor_site_config.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/templates/vendorpromo/processor_site_config_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/templates/vendorpromo/promo.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/templates/vendorpromo/promo_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/templates/vendorpromo/promocode_formset.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/templates/vendorpromo/promotional_campaign_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/templates/vendorpromo/promotional_campaign_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/templates/vendorpromo/vouchery_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/templates/vendorpromo/vouchery_integration.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/templates/vendorpromo/vouchery_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:54:59.883942 django-vendor-promo-0.2.6/src/vendorpromo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/tests/test_affiliate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/tests/test_coupon_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21273 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/tests/test_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/tests/test_promo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/tests/test_promotional_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20938 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/tests/test_stripe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15017 2023-06-01 02:53:45.000000 django-vendor-promo-0.2.6/src/vendorpromo/views.py
```

### Comparing `django-vendor-promo-0.2.5/PKG-INFO` & `django-vendor-promo-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vendor-promo
-Version: 0.2.5
+Version: 0.2.6
 Summary: Extension to Django Vendor to add Promo Code capabilities
 Author: Roberto Himmelbauer
 Author-email: Grant Viklund <renderbox@gmail.com>
 Project-URL: Homepage, https://github.com/renderbox/django-vendor-promo/
 Project-URL: Bug Tracker, https://github.com/renderbox/django-vendor-promo/issues
 Keywords: django,app
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `django-vendor-promo-0.2.5/pyproject.toml` & `django-vendor-promo-0.2.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 [project]
 name = "django-vendor-promo"
-version = "0.2.5"
+version = "0.2.6"
 
 authors = [
   { name="Grant Viklund", email="renderbox@gmail.com" },
   { name="Roberto Himmelbauer" }
 ]
 description = "Extension to Django Vendor to add Promo Code capabilities"
 readme = "README.md"
```

### Comparing `django-vendor-promo-0.2.5/src/django_vendor_promo.egg-info/PKG-INFO` & `django-vendor-promo-0.2.6/src/django_vendor_promo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vendor-promo
-Version: 0.2.5
+Version: 0.2.6
 Summary: Extension to Django Vendor to add Promo Code capabilities
 Author: Roberto Himmelbauer
 Author-email: Grant Viklund <renderbox@gmail.com>
 Project-URL: Homepage, https://github.com/renderbox/django-vendor-promo/
 Project-URL: Bug Tracker, https://github.com/renderbox/django-vendor-promo/issues
 Keywords: django,app
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `django-vendor-promo-0.2.5/src/django_vendor_promo.egg-info/SOURCES.txt` & `django-vendor-promo-0.2.6/src/django_vendor_promo.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 src/vendorpromo/api/v1/vouchery/__init__.py
 src/vendorpromo/api/v1/vouchery/urls.py
 src/vendorpromo/api/v1/vouchery/views.py
 src/vendorpromo/migrations/0001_initial.py
 src/vendorpromo/migrations/0002_affiliate_couponcode_promotionalcampaign.py
 src/vendorpromo/migrations/0003_auto_20230524_1701.py
 src/vendorpromo/migrations/0004_affiliate_name_type.py
+src/vendorpromo/migrations/0005_alter_couponcode_code.py
 src/vendorpromo/migrations/__init__.py
 src/vendorpromo/processors/DummyProcessor.py
 src/vendorpromo/processors/__init__.py
 src/vendorpromo/processors/base.py
 src/vendorpromo/processors/stripe.py
 src/vendorpromo/processors/vouchery.py
 src/vendorpromo/templates/vendorpromo/affiliate_detail.html
```

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/admin.py` & `django-vendor-promo-0.2.6/src/vendorpromo/admin.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/api/v1/urls.py` & `django-vendor-promo-0.2.6/src/vendorpromo/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/api/v1/views.py` & `django-vendor-promo-0.2.6/src/vendorpromo/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/api/v1/vouchery/views.py` & `django-vendor-promo-0.2.6/src/vendorpromo/api/v1/vouchery/views.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/config.py` & `django-vendor-promo-0.2.6/src/vendorpromo/config.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/forms.py` & `django-vendor-promo-0.2.6/src/vendorpromo/forms.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from django import forms
 from django.contrib.sites.models import Site
 from django.db.models import TextChoices
 from django.forms import modelformset_factory
+from django.utils import timezone
 from django.utils.translation import gettext as _
 from integrations.models import Credential
 from vendor.models import CustomerProfile
 from vendor.models.base import get_product_model
 
 from vendorpromo.models import (Affiliate, CouponCode, Promo,
                                 PromotionalCampaign)
@@ -94,27 +95,33 @@
             self.fields['applies_to'].queryset = get_product_model().objects.filter(site=site)
 
         if self.instance.pk:
             self.fields['applies_to'].initial = self.instance.applies_to.products.all()
             self.fields['is_percent_off'].initial = (True, "Percent Off") if self.instance.is_percent_off else (False, "Fixed Amount")
             self.fields['discount_value'].initial = self.instance.applies_to.current_price()
 
-
     def clean_discount_value(self):
         discount_value = self.cleaned_data.get('discount_value', 0)
 
         if discount_value <= 0:
             raise forms.ValidationError(_("Number must be greater than 0"))
         
         if self.cleaned_data.get('is_percent_off'):
             if not (0 < discount_value < 100):
                 raise forms.ValidationError(_("Must be a number between 1 and 99"))
         
         return discount_value
+    
+    def clean_end_date(self):
+        end_date = self.cleaned_data['end_date']
+
+        if end_date and end_date < timezone.now():
+            raise forms.ValidationError(_("The End Date must be a future date"))
 
+        return end_date
 
 class StripePromotionalCampaignForm(PromotionalCampaignForm):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         if self.instance.pk:
```

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/integrations.py` & `django-vendor-promo-0.2.6/src/vendorpromo/integrations.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/migrations/0001_initial.py` & `django-vendor-promo-0.2.6/src/vendorpromo/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/migrations/0002_affiliate_couponcode_promotionalcampaign.py` & `django-vendor-promo-0.2.6/src/vendorpromo/migrations/0002_affiliate_couponcode_promotionalcampaign.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/migrations/0003_auto_20230524_1701.py` & `django-vendor-promo-0.2.6/src/vendorpromo/migrations/0003_auto_20230524_1701.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/migrations/0004_affiliate_name_type.py` & `django-vendor-promo-0.2.6/src/vendorpromo/migrations/0004_affiliate_name_type.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/models.py` & `django-vendor-promo-0.2.6/src/vendorpromo/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         verbose_name = "Promotional Campaign"
         verbose_name_plural = "Promotional Campaigns"
     
 
 class CouponCode(CreateUpdateModelBase):
     uuid = models.UUIDField(default=uuid.uuid4, editable=False, unique=True)
     active = models.BooleanField(_("Active"), default=True)
-    code = AutoSlugField(unique_with=('promo__site'), editable=True, blank=True, null=True, verbose_name=_("Affiliate Code"))
+    code = AutoSlugField(unique_with=('promo__site'), editable=True, blank=True, null=True, sep="copy", verbose_name=_("Affiliate Code"))
     max_redemptions = models.IntegerField(_("Max Redemptions"), blank=True, null=True)
     end_date = models.DateTimeField(_("End Date"), blank=True, null=True, help_text=_("When will the code be unavailable"))
     meta = models.JSONField(blank=True, null=True, default=dict)
     promo = models.ForeignKey(PromotionalCampaign, related_name=("coupon_code"), blank=False, null=False, on_delete=models.CASCADE)
     invoice = models.ManyToManyField(Invoice, related_name=("coupon_code"), blank=True)
 
     objects = models.Manager()
```

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/processors/base.py` & `django-vendor-promo-0.2.6/src/vendorpromo/processors/base.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/processors/stripe.py` & `django-vendor-promo-0.2.6/src/vendorpromo/processors/stripe.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/processors/vouchery.py` & `django-vendor-promo-0.2.6/src/vendorpromo/processors/vouchery.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/templates/vendorpromo/affiliate_detail.html` & `django-vendor-promo-0.2.6/src/vendorpromo/templates/vendorpromo/affiliate_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/templates/vendorpromo/affiliate_list.html` & `django-vendor-promo-0.2.6/src/vendorpromo/templates/vendorpromo/affiliate_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/templates/vendorpromo/coupon_code_detail.html` & `django-vendor-promo-0.2.6/src/vendorpromo/templates/vendorpromo/coupon_code_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/templates/vendorpromo/coupon_code_list.html` & `django-vendor-promo-0.2.6/src/vendorpromo/templates/vendorpromo/coupon_code_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/templates/vendorpromo/includes/promocode_apply.html` & `django-vendor-promo-0.2.6/src/vendorpromo/templates/vendorpromo/includes/promocode_apply.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/templates/vendorpromo/processor_site_config_list.html` & `django-vendor-promo-0.2.6/src/vendorpromo/templates/vendorpromo/processor_site_config_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/templates/vendorpromo/promo.html` & `django-vendor-promo-0.2.6/src/vendorpromo/templates/vendorpromo/promo.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/templates/vendorpromo/promo_list.html` & `django-vendor-promo-0.2.6/src/vendorpromo/templates/vendorpromo/promo_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/templates/vendorpromo/promocode_formset.html` & `django-vendor-promo-0.2.6/src/vendorpromo/templates/vendorpromo/promocode_formset.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/templates/vendorpromo/promotional_campaign_detail.html` & `django-vendor-promo-0.2.6/src/vendorpromo/templates/vendorpromo/promotional_campaign_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/templates/vendorpromo/promotional_campaign_list.html` & `django-vendor-promo-0.2.6/src/vendorpromo/templates/vendorpromo/promotional_campaign_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/templates/vendorpromo/vouchery_detail.html` & `django-vendor-promo-0.2.6/src/vendorpromo/templates/vendorpromo/vouchery_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/templates/vendorpromo/vouchery_integration.html` & `django-vendor-promo-0.2.6/src/vendorpromo/templates/vendorpromo/vouchery_integration.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/templates/vendorpromo/vouchery_list.html` & `django-vendor-promo-0.2.6/src/vendorpromo/templates/vendorpromo/vouchery_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/tests/test_affiliate.py` & `django-vendor-promo-0.2.6/src/vendorpromo/tests/test_affiliate.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/tests/test_api.py` & `django-vendor-promo-0.2.6/src/vendorpromo/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/tests/test_coupon_code.py` & `django-vendor-promo-0.2.6/src/vendorpromo/tests/test_coupon_code.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/tests/test_processor.py` & `django-vendor-promo-0.2.6/src/vendorpromo/tests/test_processor.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/tests/test_promo.py` & `django-vendor-promo-0.2.6/src/vendorpromo/tests/test_promo.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/tests/test_promotional_campaign.py` & `django-vendor-promo-0.2.6/src/vendorpromo/tests/test_promotional_campaign.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/tests/test_stripe.py` & `django-vendor-promo-0.2.6/src/vendorpromo/tests/test_stripe.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/urls.py` & `django-vendor-promo-0.2.6/src/vendorpromo/urls.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.5/src/vendorpromo/views.py` & `django-vendor-promo-0.2.6/src/vendorpromo/views.py`

 * *Files identical despite different names*

