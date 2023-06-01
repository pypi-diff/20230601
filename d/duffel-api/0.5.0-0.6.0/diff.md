# Comparing `tmp/duffel-api-0.5.0.tar.gz` & `tmp/duffel-api-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duffel-api-0.5.0.tar", last modified: Wed Feb 15 14:41:09 2023, max compression
+gzip compressed data, was "duffel-api-0.6.0.tar", last modified: Thu Jun  1 08:12:10 2023, max compression
```

## Comparing `duffel-api-0.5.0.tar` & `duffel-api-0.6.0.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:41:09.556866 duffel-api-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-02-15 14:41:01.000000 duffel-api-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-02-15 14:41:09.556866 duffel-api-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-02-15 14:41:01.000000 duffel-api-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:41:09.548866 duffel-api-0.5.0/duffel_api/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:41:09.548866 duffel-api-0.5.0/duffel_api/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:41:09.548866 duffel-api-0.5.0/duffel_api/api/booking/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/api/booking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/api/booking/offer_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/api/booking/offers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/api/booking/order_cancellations.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/api/booking/order_change_offers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/api/booking/order_change_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/api/booking/order_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/api/booking/orders.py
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/api/booking/partial_offer_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/api/booking/payments.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/api/booking/seat_maps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:41:09.548866 duffel-api-0.5.0/duffel_api/api/duffel_payments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/api/duffel_payments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/api/duffel_payments/payment_intents.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:41:09.548866 duffel-api-0.5.0/duffel_api/api/links/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/api/links/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/api/links/sessions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:41:09.548866 duffel-api-0.5.0/duffel_api/api/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/api/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/api/notifications/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:41:09.548866 duffel-api-0.5.0/duffel_api/api/supporting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/api/supporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/api/supporting/aircraft.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/api/supporting/airlines.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/api/supporting/airports.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:41:09.552866 duffel-api-0.5.0/duffel_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/models/aircraft.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/models/airline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/models/airport.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/models/loyalty_programme_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    17335 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/models/offer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/models/offer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    19113 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/models/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/models/order_cancellation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/models/order_change.py
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/models/order_change_offer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/models/order_change_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/models/payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/models/payment_intent.py
--rw-r--r--   0 runner    (1001) docker     (123)     6725 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/models/seat_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/models/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/models/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-02-15 14:41:01.000000 duffel-api-0.5.0/duffel_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:41:09.548866 duffel-api-0.5.0/duffel_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-02-15 14:41:09.000000 duffel-api-0.5.0/duffel_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-02-15 14:41:09.000000 duffel-api-0.5.0/duffel_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 14:41:09.000000 duffel-api-0.5.0/duffel_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-15 14:41:09.000000 duffel-api-0.5.0/duffel_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-15 14:41:09.000000 duffel-api-0.5.0/duffel_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-02-15 14:41:01.000000 duffel-api-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 14:41:09.556866 duffel-api-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-02-15 14:41:01.000000 duffel-api-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:41:09.556866 duffel-api-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_aircraft.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_aircrafts.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_airline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_airlines.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_airport.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_airports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_links_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_loyalty_programme_account.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_offer.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_offer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_offer_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_offers.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_order_cancellation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_order_cancellations.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_order_change.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_order_change_offer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_order_change_offers.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_order_change_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_order_change_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_order_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_orders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_partial_offer_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_payment.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_payment_intent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_payment_intents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_payments.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_refund.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_seat_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_seat_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-02-15 14:41:01.000000 duffel-api-0.5.0/tests/test_webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:12:10.287767 duffel-api-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-01 08:12:01.000000 duffel-api-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-06-01 08:12:10.287767 duffel-api-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-01 08:12:01.000000 duffel-api-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:12:10.275767 duffel-api-0.6.0/duffel_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:12:10.275767 duffel-api-0.6.0/duffel_api/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:12:10.275767 duffel-api-0.6.0/duffel_api/api/booking/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/api/booking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/api/booking/offer_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/api/booking/offers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/api/booking/order_cancellations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/api/booking/order_change_offers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/api/booking/order_change_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/api/booking/order_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/api/booking/orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/api/booking/partial_offer_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/api/booking/payments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/api/booking/seat_maps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:12:10.275767 duffel-api-0.6.0/duffel_api/api/duffel_payments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/api/duffel_payments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/api/duffel_payments/payment_intents.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:12:10.279767 duffel-api-0.6.0/duffel_api/api/links/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/api/links/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/api/links/sessions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:12:10.279767 duffel-api-0.6.0/duffel_api/api/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/api/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/api/notifications/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:12:10.279767 duffel-api-0.6.0/duffel_api/api/supporting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/api/supporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/api/supporting/aircraft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/api/supporting/airlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/api/supporting/airports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:12:10.279767 duffel-api-0.6.0/duffel_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/models/aircraft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/models/airline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/models/airport.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/models/loyalty_programme_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17152 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/models/offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/models/offer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/models/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/models/order_cancellation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/models/order_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/models/order_change_offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/models/order_change_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/models/payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/models/payment_intent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6725 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/models/seat_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/models/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/models/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-01 08:12:01.000000 duffel-api-0.6.0/duffel_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:12:10.275767 duffel-api-0.6.0/duffel_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-06-01 08:12:10.000000 duffel-api-0.6.0/duffel_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-01 08:12:10.000000 duffel-api-0.6.0/duffel_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 08:12:10.000000 duffel-api-0.6.0/duffel_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-01 08:12:10.000000 duffel-api-0.6.0/duffel_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-01 08:12:10.000000 duffel-api-0.6.0/duffel_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-01 08:12:01.000000 duffel-api-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 08:12:10.287767 duffel-api-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-01 08:12:01.000000 duffel-api-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:12:10.287767 duffel-api-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_aircraft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_aircrafts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_airline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_airlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_airport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_airports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_links_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_loyalty_programme_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_offer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_offer_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_offers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_order_cancellation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_order_cancellations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_order_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_order_change_offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_order_change_offers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_order_change_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_order_change_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_order_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_partial_offer_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_payment_intent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_payment_intents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_payments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_refund.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_seat_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_seat_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-01 08:12:01.000000 duffel-api-0.6.0/tests/test_webhooks.py
```

### Comparing `duffel-api-0.5.0/LICENSE` & `duffel-api-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/PKG-INFO` & `duffel-api-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: duffel-api
-Version: 0.5.0
+Version: 0.6.0
 Summary: Client library for the Duffel API
 Home-page: https://github.com/duffelhq/duffel-api-python
 Author: Duffel Engineering
 Author-email: client-libraries@duffel.com
 License: MIT
 Keywords: duffel api flights airports airlines aircraft
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI](https://img.shields.io/pypi/v/duffel-api?style=flat-square)](https://pypi.org/project/duffel-api/)
 [![Supported Python
 versions](https://img.shields.io/pypi/pyversions/duffel-api.svg)](https://pypi.org/project/duffel-api/)
 [![Build Status](https://github.com/duffelhq/duffel-api-python/actions/workflows/main.yaml/badge.svg)](https://github.com/duffelhq/duffel-api-python/actions/workflows/main.yaml)
@@ -24,15 +24,15 @@
 
 # duffel-api
 
 Python client library for the [Duffel API](https://duffel.com/docs/api).
 
 ## Requirements
 
-- Python 3.7+
+- Python 3.8+
 
 ## Getting started
 
 ```shell
 pip install duffel-api
 ```
```

### Comparing `duffel-api-0.5.0/README.md` & `duffel-api-0.6.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # duffel-api
 
 Python client library for the [Duffel API](https://duffel.com/docs/api).
 
 ## Requirements
 
-- Python 3.7+
+- Python 3.8+
 
 ## Getting started
 
 ```shell
 pip install duffel-api
 ```
```

### Comparing `duffel-api-0.5.0/duffel_api/api/__init__.py` & `duffel-api-0.6.0/duffel_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/duffel_api/api/booking/offer_requests.py` & `duffel-api-0.6.0/duffel_api/api/booking/offer_requests.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/duffel_api/api/booking/offers.py` & `duffel-api-0.6.0/duffel_api/api/booking/offers.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/duffel_api/api/booking/order_cancellations.py` & `duffel-api-0.6.0/duffel_api/api/booking/order_cancellations.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/duffel_api/api/booking/order_change_offers.py` & `duffel-api-0.6.0/duffel_api/api/booking/order_change_offers.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/duffel_api/api/booking/order_change_requests.py` & `duffel-api-0.6.0/duffel_api/api/booking/order_change_requests.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/duffel_api/api/booking/order_changes.py` & `duffel-api-0.6.0/duffel_api/api/booking/order_changes.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/duffel_api/api/booking/orders.py` & `duffel-api-0.6.0/duffel_api/api/booking/orders.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/duffel_api/api/booking/partial_offer_requests.py` & `duffel-api-0.6.0/duffel_api/api/booking/partial_offer_requests.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/duffel_api/api/booking/payments.py` & `duffel-api-0.6.0/duffel_api/api/booking/payments.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/duffel_api/api/duffel_payments/payment_intents.py` & `duffel-api-0.6.0/duffel_api/api/duffel_payments/payment_intents.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/duffel_api/api/links/sessions.py` & `duffel-api-0.6.0/duffel_api/api/links/sessions.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/duffel_api/api/notifications/webhooks.py` & `duffel-api-0.6.0/duffel_api/api/notifications/webhooks.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/duffel_api/api/supporting/aircraft.py` & `duffel-api-0.6.0/duffel_api/api/supporting/aircraft.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/duffel_api/api/supporting/airlines.py` & `duffel-api-0.6.0/duffel_api/api/supporting/airlines.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/duffel_api/api/supporting/airports.py` & `duffel-api-0.6.0/duffel_api/api/supporting/airports.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/duffel_api/client.py` & `duffel-api-0.6.0/duffel_api/client.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/duffel_api/http_client.py` & `duffel-api-0.6.0/duffel_api/http_client.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/duffel_api/models/__init__.py` & `duffel-api-0.6.0/duffel_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/duffel_api/models/airport.py` & `duffel-api-0.6.0/duffel_api/models/airport.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Optional, Sequence
 
-from duffel_api.utils import get_and_transform
+from duffel_api.utils import get_and_transform, parse_datetime
 
 
 @dataclass
 class City:
     """The metropolitan area where the airport is located.
     Only present for airports which are registered with IATA as
     belonging to a metropolitan area.
@@ -140,10 +140,10 @@
             amount=json["amount"],
             currency=json["currency"],
             net_amount=json.get("net_amount"),
             net_currency=json.get("net_currency"),
             status=json["status"],
             destination=json["destination"],
             arrival=json["arrival"],
-            created_at=datetime.strptime(json["created_at"], "%Y-%m-%dT%H:%M:%S.%fZ"),
-            updated_at=datetime.strptime(json["created_at"], "%Y-%m-%dT%H:%M:%S.%fZ"),
+            created_at=parse_datetime(json["created_at"]),
+            updated_at=parse_datetime(json["updated_at"]),
         )
```

### Comparing `duffel-api-0.5.0/duffel_api/models/offer.py` & `duffel-api-0.6.0/duffel_api/models/offer.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,17 +95,15 @@
     def from_json(cls, json: dict):
         """Construct a class instance from a JSON response."""
         return cls(
             payment_required_by=get_and_transform(
                 json, "payment_required_by", parse_datetime
             ),
             price_guarantee_expires_at=get_and_transform(
-                json,
-                "price_guarantee_expires_at",
-                lambda value: datetime.strptime(value, "%Y-%m-%dT%H:%M:%SZ"),
+                json, "price_guarantee_expires_at", parse_datetime
             ),
             requires_instant_payment=json["requires_instant_payment"],
         )
 
 
 @dataclass
 class ServiceMetadata:
@@ -247,16 +245,16 @@
 
     @classmethod
     def from_json(cls, json: dict):
         """Construct a class instance from a JSON response."""
         return cls(
             id=json["id"],
             aircraft=get_and_transform(json, "aircraft", Aircraft.from_json),
-            arriving_at=datetime.strptime(json["arriving_at"], "%Y-%m-%dT%H:%M:%S"),
-            departing_at=datetime.strptime(json["departing_at"], "%Y-%m-%dT%H:%M:%S"),
+            arriving_at=parse_datetime(json["arriving_at"]),
+            departing_at=parse_datetime(json["departing_at"]),
             destination=Airport.from_json(json["destination"]),
             destination_terminal=json.get("destination_terminal"),
             origin=Airport.from_json(json["origin"]),
             origin_terminal=json.get("origin_terminal"),
             distance=json.get("distance"),
             duration=json.get("duration"),
             marketing_carrier=Airline.from_json(json["marketing_carrier"]),
@@ -462,16 +460,16 @@
                 "available_services",
                 lambda value: [Service.from_json(passenger) for passenger in value],
                 [],
             ),
             base_amount=json["base_amount"],
             base_currency=json["base_currency"],
             conditions=OfferConditions.from_json(json["conditions"]),
-            created_at=datetime.strptime(json["created_at"], "%Y-%m-%dT%H:%M:%S.%fZ"),
-            updated_at=datetime.strptime(json["updated_at"], "%Y-%m-%dT%H:%M:%S.%fZ"),
+            created_at=parse_datetime(json["created_at"]),
+            updated_at=parse_datetime(json["updated_at"]),
             expires_at=parse_datetime(json["expires_at"]),
             owner=Airline.from_json(json["owner"]),
             partial=json["partial"],
             passenger_identity_documents_required=json[
                 "passenger_identity_documents_required"
             ],
             passengers=get_and_transform(
```

### Comparing `duffel-api-0.5.0/duffel_api/models/offer_request.py` & `duffel-api-0.6.0/duffel_api/models/offer_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import dataclass
 from datetime import date, datetime
 from typing import Optional, Sequence, Union
 
 from duffel_api.models import Airport, City, LoyaltyProgrammeAccount, Offer
-from duffel_api.utils import get_and_transform
+from duffel_api.utils import get_and_transform, parse_datetime
 
 
 @dataclass
 class OfferRequestSlice:
     """One-way journeys can be expressed using one slice, whereas return trips will need
     two.
     """
@@ -116,9 +116,9 @@
                 json,
                 "passengers",
                 lambda value: [
                     OfferRequestPassenger.from_json(passenger) for passenger in value
                 ],
                 [],
             ),
-            created_at=datetime.strptime(json["created_at"], "%Y-%m-%dT%H:%M:%S.%fZ"),
+            created_at=parse_datetime(json["created_at"]),
         )
```

### Comparing `duffel-api-0.5.0/duffel_api/models/order.py` & `duffel-api-0.6.0/duffel_api/models/order.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Optional, Sequence, Union
 
 from duffel_api.models import Aircraft, Airline, Airport, LoyaltyProgrammeAccount, Place
-from duffel_api.utils import get_and_transform
+from duffel_api.utils import get_and_transform, parse_datetime
 
 
 @dataclass
 class OrderConditionChangeBeforeDeparture:
     """Whether the whole order can be changed before the departure of the first slice.
 
     If all of the slices on the order can be changed then
@@ -196,16 +196,16 @@
 
     @classmethod
     def from_json(cls, json: dict):
         """Construct a class instance from a JSON response."""
         return cls(
             id=json["id"],
             aircraft=get_and_transform(json, "aircraft", Aircraft.from_json),
-            arriving_at=datetime.strptime(json["arriving_at"], "%Y-%m-%dT%H:%M:%S"),
-            departing_at=datetime.strptime(json["departing_at"], "%Y-%m-%dT%H:%M:%S"),
+            arriving_at=parse_datetime(json["arriving_at"]),
+            departing_at=parse_datetime(json["departing_at"]),
             destination=Airport.from_json(json["destination"]),
             destination_terminal=json.get("destination_terminal"),
             origin=Airport.from_json(json["origin"]),
             origin_terminal=json.get("origin_terminal"),
             distance=json.get("distance"),
             duration=json.get("duration"),
             marketing_carrier=Airline.from_json(json["marketing_carrier"]),
@@ -416,20 +416,20 @@
     def from_json(cls, json: dict):
         """Construct a class instance from a JSON response."""
         return cls(
             awaiting_payment=json["awaiting_payment"],
             payment_required_by=get_and_transform(
                 json,
                 "payment_required_by",
-                lambda value: datetime.strptime(value, "%Y-%m-%dT%H:%M:%SZ"),
+                parse_datetime,
             ),
             price_guarantee_expires_at=get_and_transform(
                 json,
                 "price_guarantee_expires_at",
-                lambda value: datetime.strptime(value, "%Y-%m-%dT%H:%M:%SZ"),
+                parse_datetime,
             ),
         )
 
 
 @dataclass
 class OrderPassenger:
     """A passenger who is travelling"""
@@ -525,22 +525,22 @@
             live_mode=json["live_mode"],
             base_amount=json.get("base_amount"),
             base_currency=json.get("base_currency"),
             booking_reference=json["booking_reference"],
             cancelled_at=get_and_transform(
                 json,
                 "cancelled_at",
-                lambda value: datetime.strptime(value, "%Y-%m-%dT%H:%M:%S.%fZ"),
+                parse_datetime,
             ),
             content=json["content"],
-            created_at=datetime.strptime(json["created_at"], "%Y-%m-%dT%H:%M:%S.%fZ"),
+            created_at=parse_datetime(json["created_at"]),
             synced_at=get_and_transform(
                 json,
                 "synced_at",
-                lambda value: datetime.strptime(value, "%Y-%m-%dT%H:%M:%SZ"),
+                parse_datetime,
             ),
             documents=get_and_transform(
                 json,
                 "documents",
                 lambda value: [OrderDocument.from_json(document) for document in value],
                 [],
             ),
```

### Comparing `duffel-api-0.5.0/duffel_api/models/order_cancellation.py` & `duffel-api-0.6.0/duffel_api/models/order_cancellation.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/duffel_api/models/order_change.py` & `duffel-api-0.6.0/duffel_api/models/order_change.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/duffel_api/models/order_change_offer.py` & `duffel-api-0.6.0/duffel_api/models/order_change_offer.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/duffel_api/models/order_change_request.py` & `duffel-api-0.6.0/duffel_api/models/order_change_request.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/duffel_api/models/payment.py` & `duffel-api-0.6.0/duffel_api/models/payment.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Optional
 
+from duffel_api.utils import parse_datetime
+
 
 @dataclass
 class Payment:
     """To pay for an unpaid order you've previously created, you'll need to create a
     payment for it.
 
     The payment details you provide will be charged and, if successful, your order will
@@ -36,9 +38,9 @@
         """Construct a class instance from a JSON response."""
         return cls(
             id=json["id"],
             type=json["type"],
             live_mode=json["live_mode"],
             amount=json["amount"],
             currency=json.get("currency"),
-            created_at=datetime.strptime(json["created_at"], "%Y-%m-%dT%H:%M:%S.%fZ"),
+            created_at=parse_datetime(json["created_at"]),
         )
```

### Comparing `duffel-api-0.5.0/duffel_api/models/payment_intent.py` & `duffel-api-0.6.0/duffel_api/models/payment_intent.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/duffel_api/models/seat_map.py` & `duffel-api-0.6.0/duffel_api/models/seat_map.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/duffel_api/models/session.py` & `duffel-api-0.6.0/duffel_api/models/session.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/duffel_api/models/webhook.py` & `duffel-api-0.6.0/duffel_api/models/webhook.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/duffel_api.egg-info/PKG-INFO` & `duffel-api-0.6.0/duffel_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: duffel-api
-Version: 0.5.0
+Version: 0.6.0
 Summary: Client library for the Duffel API
 Home-page: https://github.com/duffelhq/duffel-api-python
 Author: Duffel Engineering
 Author-email: client-libraries@duffel.com
 License: MIT
 Keywords: duffel api flights airports airlines aircraft
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI](https://img.shields.io/pypi/v/duffel-api?style=flat-square)](https://pypi.org/project/duffel-api/)
 [![Supported Python
 versions](https://img.shields.io/pypi/pyversions/duffel-api.svg)](https://pypi.org/project/duffel-api/)
 [![Build Status](https://github.com/duffelhq/duffel-api-python/actions/workflows/main.yaml/badge.svg)](https://github.com/duffelhq/duffel-api-python/actions/workflows/main.yaml)
@@ -24,15 +24,15 @@
 
 # duffel-api
 
 Python client library for the [Duffel API](https://duffel.com/docs/api).
 
 ## Requirements
 
-- Python 3.7+
+- Python 3.8+
 
 ## Getting started
 
 ```shell
 pip install duffel-api
 ```
```

### Comparing `duffel-api-0.5.0/duffel_api.egg-info/SOURCES.txt` & `duffel-api-0.6.0/duffel_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/pyproject.toml` & `duffel-api-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/setup.py` & `duffel-api-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="duffel-api",
-    version="0.5.0",
+    version="0.6.0",
     author="Duffel Engineering",
     author_email="client-libraries@duffel.com",
     description="Client library for the Duffel API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/duffelhq/duffel-api-python",
     packages=find_packages(),
@@ -17,10 +17,10 @@
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
     ],
     keywords="duffel api flights airports airlines aircraft",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=["requests>=2.25"],
 )
```

### Comparing `duffel-api-0.5.0/tests/fixtures.py` & `duffel-api-0.6.0/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/tests/test_aircrafts.py` & `duffel-api-0.6.0/tests/test_aircrafts.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/tests/test_airlines.py` & `duffel-api-0.6.0/tests/test_airlines.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/tests/test_airports.py` & `duffel-api-0.6.0/tests/test_airports.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/tests/test_http_client.py` & `duffel-api-0.6.0/tests/test_http_client.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/tests/test_links_sessions.py` & `duffel-api-0.6.0/tests/test_links_sessions.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/tests/test_offer_requests.py` & `duffel-api-0.6.0/tests/test_offer_requests.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/tests/test_offers.py` & `duffel-api-0.6.0/tests/test_offers.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/tests/test_order_cancellations.py` & `duffel-api-0.6.0/tests/test_order_cancellations.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/tests/test_order_change_offers.py` & `duffel-api-0.6.0/tests/test_order_change_offers.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/tests/test_order_change_requests.py` & `duffel-api-0.6.0/tests/test_order_change_requests.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/tests/test_order_changes.py` & `duffel-api-0.6.0/tests/test_order_changes.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/tests/test_orders.py` & `duffel-api-0.6.0/tests/test_orders.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/tests/test_partial_offer_requests.py` & `duffel-api-0.6.0/tests/test_partial_offer_requests.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/tests/test_payment_intents.py` & `duffel-api-0.6.0/tests/test_payment_intents.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/tests/test_payments.py` & `duffel-api-0.6.0/tests/test_payments.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/tests/test_seat_maps.py` & `duffel-api-0.6.0/tests/test_seat_maps.py`

 * *Files identical despite different names*

### Comparing `duffel-api-0.5.0/tests/test_webhooks.py` & `duffel-api-0.6.0/tests/test_webhooks.py`

 * *Files identical despite different names*

