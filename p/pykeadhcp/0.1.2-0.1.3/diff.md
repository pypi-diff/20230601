# Comparing `tmp/pykeadhcp-0.1.2.tar.gz` & `tmp/pykeadhcp-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykeadhcp-0.1.2.tar", max compression
+gzip compressed data, was "pykeadhcp-0.1.3.tar", max compression
```

## Comparing `pykeadhcp-0.1.2.tar` & `pykeadhcp-0.1.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    11356 2023-06-01 12:19:38.579915 pykeadhcp-0.1.2/LICENSE
--rw-r--r--   0        0        0     5301 2023-06-01 12:19:38.579915 pykeadhcp-0.1.2/README.md
--rw-r--r--   0        0        0       30 2023-06-01 12:19:38.579915 pykeadhcp-0.1.2/pykeadhcp/__init__.py
--rw-r--r--   0        0        0      174 2023-06-01 12:19:38.579915 pykeadhcp-0.1.2/pykeadhcp/daemons/__init__.py
--rw-r--r--   0        0        0     4508 2023-06-01 12:19:38.579915 pykeadhcp-0.1.2/pykeadhcp/daemons/ctrlagent.py
--rw-r--r--   0        0        0     4526 2023-06-01 12:19:38.579915 pykeadhcp-0.1.2/pykeadhcp/daemons/ddns.py
--rw-r--r--   0        0        0    25295 2023-06-01 12:19:38.579915 pykeadhcp-0.1.2/pykeadhcp/daemons/dhcp4.py
--rw-r--r--   0        0        0    21553 2023-06-01 12:19:38.579915 pykeadhcp-0.1.2/pykeadhcp/daemons/dhcp6.py
--rw-r--r--   0        0        0     2718 2023-06-01 12:19:38.579915 pykeadhcp-0.1.2/pykeadhcp/exceptions.py
--rw-r--r--   0        0        0     7453 2023-06-01 12:19:38.579915 pykeadhcp-0.1.2/pykeadhcp/kea.py
--rw-r--r--   0        0        0        0 2023-06-01 12:19:38.579915 pykeadhcp-0.1.2/pykeadhcp/models/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 12:19:38.583915 pykeadhcp-0.1.2/pykeadhcp/models/ctrlagent/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 12:19:38.583915 pykeadhcp-0.1.2/pykeadhcp/models/dhcp4/__init__.py
--rw-r--r--   0        0        0      207 2023-06-01 12:19:38.583915 pykeadhcp-0.1.2/pykeadhcp/models/dhcp4/lease.py
--rw-r--r--   0        0        0      303 2023-06-01 12:19:38.583915 pykeadhcp-0.1.2/pykeadhcp/models/dhcp4/reservation.py
--rw-r--r--   0        0        0      448 2023-06-01 12:19:38.583915 pykeadhcp-0.1.2/pykeadhcp/models/dhcp4/shared_network.py
--rw-r--r--   0        0        0      472 2023-06-01 12:19:38.583915 pykeadhcp-0.1.2/pykeadhcp/models/dhcp4/subnet.py
--rw-r--r--   0        0        0        0 2023-06-01 12:19:38.583915 pykeadhcp-0.1.2/pykeadhcp/models/dhcp6/__init__.py
--rw-r--r--   0        0        0      341 2023-06-01 12:19:38.583915 pykeadhcp-0.1.2/pykeadhcp/models/dhcp6/lease.py
--rw-r--r--   0        0        0      542 2023-06-01 12:19:38.583915 pykeadhcp-0.1.2/pykeadhcp/models/dhcp6/pd_pool.py
--rw-r--r--   0        0        0      202 2023-06-01 12:19:38.583915 pykeadhcp-0.1.2/pykeadhcp/models/dhcp6/reservation.py
--rw-r--r--   0        0        0      375 2023-06-01 12:19:38.583915 pykeadhcp-0.1.2/pykeadhcp/models/dhcp6/shared_network.py
--rw-r--r--   0        0        0      491 2023-06-01 12:19:38.583915 pykeadhcp-0.1.2/pykeadhcp/models/dhcp6/subnet.py
--rw-r--r--   0        0        0      495 2023-06-01 12:19:38.583915 pykeadhcp-0.1.2/pykeadhcp/models/enums.py
--rw-r--r--   0        0        0      169 2023-06-01 12:19:38.583915 pykeadhcp-0.1.2/pykeadhcp/models/generic/__init__.py
--rw-r--r--   0        0        0      181 2023-06-01 12:19:38.583915 pykeadhcp-0.1.2/pykeadhcp/models/generic/api_response.py
--rw-r--r--   0        0        0      247 2023-06-01 12:19:38.583915 pykeadhcp-0.1.2/pykeadhcp/models/generic/base.py
--rw-r--r--   0        0        0     1589 2023-06-01 12:19:38.583915 pykeadhcp-0.1.2/pykeadhcp/models/generic/dhcp_common.py
--rw-r--r--   0        0        0      156 2023-06-01 12:19:38.583915 pykeadhcp-0.1.2/pykeadhcp/models/generic/hook.py
--rw-r--r--   0        0        0      403 2023-06-01 12:19:38.583915 pykeadhcp-0.1.2/pykeadhcp/models/generic/lease.py
--rw-r--r--   0        0        0      364 2023-06-01 12:19:38.583915 pykeadhcp-0.1.2/pykeadhcp/models/generic/option_data.py
--rw-r--r--   0        0        0      412 2023-06-01 12:19:38.583915 pykeadhcp-0.1.2/pykeadhcp/models/generic/pool.py
--rw-r--r--   0        0        0      488 2023-06-01 12:19:38.583915 pykeadhcp-0.1.2/pykeadhcp/models/generic/reservation.py
--rw-r--r--   0        0        0      175 2023-06-01 12:19:38.583915 pykeadhcp-0.1.2/pykeadhcp/models/generic/shared_network.py
--rw-r--r--   0        0        0      244 2023-06-01 12:19:38.583915 pykeadhcp-0.1.2/pykeadhcp/models/generic/sockets.py
--rw-r--r--   0        0        0      472 2023-06-01 12:19:38.583915 pykeadhcp-0.1.2/pykeadhcp/models/generic/status.py
--rw-r--r--   0        0        0      390 2023-06-01 12:19:38.583915 pykeadhcp-0.1.2/pykeadhcp/models/generic/subnet.py
--rw-r--r--   0        0        0      447 2023-06-01 12:19:38.583915 pykeadhcp-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5906 1970-01-01 00:00:00.000000 pykeadhcp-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/LICENSE
+-rw-r--r--   0        0        0     5301 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/README.md
+-rw-r--r--   0        0        0       30 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/__init__.py
+-rw-r--r--   0        0        0      174 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/daemons/__init__.py
+-rw-r--r--   0        0        0     4508 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/daemons/ctrlagent.py
+-rw-r--r--   0        0        0     4526 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/daemons/ddns.py
+-rw-r--r--   0        0        0    25295 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/daemons/dhcp4.py
+-rw-r--r--   0        0        0    21553 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/daemons/dhcp6.py
+-rw-r--r--   0        0        0     2718 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/exceptions.py
+-rw-r--r--   0        0        0     7453 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/kea.py
+-rw-r--r--   0        0        0        0 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/ctrlagent/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/dhcp4/__init__.py
+-rw-r--r--   0        0        0      207 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/dhcp4/lease.py
+-rw-r--r--   0        0        0      303 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/dhcp4/reservation.py
+-rw-r--r--   0        0        0      448 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/dhcp4/shared_network.py
+-rw-r--r--   0        0        0      472 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/dhcp4/subnet.py
+-rw-r--r--   0        0        0        0 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/dhcp6/__init__.py
+-rw-r--r--   0        0        0      341 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/dhcp6/lease.py
+-rw-r--r--   0        0        0      542 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/dhcp6/pd_pool.py
+-rw-r--r--   0        0        0      202 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/dhcp6/reservation.py
+-rw-r--r--   0        0        0      375 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/dhcp6/shared_network.py
+-rw-r--r--   0        0        0      491 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/dhcp6/subnet.py
+-rw-r--r--   0        0        0      495 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/enums.py
+-rw-r--r--   0        0        0      169 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/generic/__init__.py
+-rw-r--r--   0        0        0      181 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/generic/api_response.py
+-rw-r--r--   0        0        0      247 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/generic/base.py
+-rw-r--r--   0        0        0     1589 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/generic/dhcp_common.py
+-rw-r--r--   0        0        0      156 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/generic/hook.py
+-rw-r--r--   0        0        0      403 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/generic/lease.py
+-rw-r--r--   0        0        0      364 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/generic/option_data.py
+-rw-r--r--   0        0        0      406 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/generic/pool.py
+-rw-r--r--   0        0        0      488 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/generic/reservation.py
+-rw-r--r--   0        0        0      175 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/generic/shared_network.py
+-rw-r--r--   0        0        0      244 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/generic/sockets.py
+-rw-r--r--   0        0        0      472 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/generic/status.py
+-rw-r--r--   0        0        0      385 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/generic/subnet.py
+-rw-r--r--   0        0        0      447 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5906 1970-01-01 00:00:00.000000 pykeadhcp-0.1.3/PKG-INFO
```

### Comparing `pykeadhcp-0.1.2/LICENSE` & `pykeadhcp-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.1.2/README.md` & `pykeadhcp-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.1.2/pykeadhcp/daemons/ctrlagent.py` & `pykeadhcp-0.1.3/pykeadhcp/daemons/ctrlagent.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.1.2/pykeadhcp/daemons/ddns.py` & `pykeadhcp-0.1.3/pykeadhcp/daemons/ddns.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.1.2/pykeadhcp/daemons/dhcp4.py` & `pykeadhcp-0.1.3/pykeadhcp/daemons/dhcp4.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.1.2/pykeadhcp/daemons/dhcp6.py` & `pykeadhcp-0.1.3/pykeadhcp/daemons/dhcp6.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.1.2/pykeadhcp/exceptions.py` & `pykeadhcp-0.1.3/pykeadhcp/exceptions.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.1.2/pykeadhcp/kea.py` & `pykeadhcp-0.1.3/pykeadhcp/kea.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.1.2/pykeadhcp/models/dhcp6/pd_pool.py` & `pykeadhcp-0.1.3/pykeadhcp/models/dhcp6/pd_pool.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.1.2/pykeadhcp/models/generic/dhcp_common.py` & `pykeadhcp-0.1.3/pykeadhcp/models/generic/dhcp_common.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.1.2/PKG-INFO` & `pykeadhcp-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykeadhcp
-Version: 0.1.2
+Version: 0.1.3
 Summary: Wrapper around requests module to query ISC Kea DHCP API Daemons (ctrlagent, dhcp4, dhcp6, ddns)
 License: Apache 2.0
 Author: Brandon Spendlove
 Author-email: brandon-spendlove@hotmail.co.uk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

