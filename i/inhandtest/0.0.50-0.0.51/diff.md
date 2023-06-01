# Comparing `tmp/inhandtest-0.0.50.tar.gz` & `tmp/inhandtest-0.0.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\inhandtest-0.0.50.tar", last modified: Wed May 31 02:53:07 2023, max compression
+gzip compressed data, was "dist\inhandtest-0.0.51.tar", last modified: Thu Jun  1 09:31:01 2023, max compression
```

## Comparing `inhandtest-0.0.50.tar` & `inhandtest-0.0.51.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 02:53:07.000000 inhandtest-0.0.50/
--rw-rw-rw-   0        0        0       81 2023-04-13 01:59:22.000000 inhandtest-0.0.50/MANIFEST.in
--rw-rw-rw-   0        0        0      593 2023-05-31 02:53:07.000000 inhandtest-0.0.50/PKG-INFO
--rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.50/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 02:53:07.000000 inhandtest-0.0.50/dm/
--rw-rw-rw-   0        0        0      134 2023-04-25 08:38:57.000000 inhandtest-0.0.50/dm/__init__.py
--rw-rw-rw-   0        0        0     1307 2023-04-26 07:13:22.000000 inhandtest-0.0.50/dm/mqtt.py
--rw-rw-rw-   0        0        0     3565 2023-04-28 07:00:23.000000 inhandtest-0.0.50/dm/register_v1.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:53:07.000000 inhandtest-0.0.50/inhandtest/
--rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.50/inhandtest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:53:07.000000 inhandtest-0.0.50/inhandtest/base_page/
--rw-rw-rw-   0        0        0      134 2023-03-15 06:05:35.000000 inhandtest-0.0.50/inhandtest/base_page/__init__.py
--rw-rw-rw-   0        0        0    39712 2023-05-16 03:23:36.000000 inhandtest-0.0.50/inhandtest/base_page/_ig_contents_locators.py
--rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.50/inhandtest/base_page/_ir3XX_contents_locators.py
--rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.50/inhandtest/base_page/_vg710_contents_locators.py
--rw-rw-rw-   0        0        0    56236 2023-05-29 08:18:45.000000 inhandtest-0.0.50/inhandtest/base_page/base_page.py
--rw-rw-rw-   0        0        0    22363 2023-05-29 08:30:51.000000 inhandtest-0.0.50/inhandtest/base_page/table_tr.py
--rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.50/inhandtest/exception.py
--rw-rw-rw-   0        0        0     3890 2023-03-30 10:08:49.000000 inhandtest-0.0.50/inhandtest/file.py
--rw-rw-rw-   0        0        0    11861 2023-05-06 01:56:01.000000 inhandtest-0.0.50/inhandtest/inmodbus.py
--rw-rw-rw-   0        0        0     4880 2023-04-27 01:05:22.000000 inhandtest-0.0.50/inhandtest/inmongodb.py
--rw-rw-rw-   0        0        0    22049 2023-03-30 10:08:49.000000 inhandtest-0.0.50/inhandtest/inmqtt.py
--rw-rw-rw-   0        0        0    51883 2023-05-16 09:03:39.000000 inhandtest-0.0.50/inhandtest/inrequest.py
--rw-rw-rw-   0        0        0     7583 2023-05-06 07:36:44.000000 inhandtest-0.0.50/inhandtest/inserial.py
--rw-rw-rw-   0        0        0    14352 2023-05-31 02:52:16.000000 inhandtest-0.0.50/inhandtest/insocket.py
--rw-rw-rw-   0        0        0     6847 2023-05-18 06:06:23.000000 inhandtest-0.0.50/inhandtest/inssh.py
--rw-rw-rw-   0        0        0     1569 2023-05-24 09:45:24.000000 inhandtest-0.0.50/inhandtest/ip.py
--rw-rw-rw-   0        0        0    11620 2023-05-08 10:30:07.000000 inhandtest-0.0.50/inhandtest/mail.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:53:07.000000 inhandtest-0.0.50/inhandtest/pages/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.50/inhandtest/pages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:53:07.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:53:07.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/edge_computing/
--rw-rw-rw-   0        0        0      134 2023-05-25 07:33:25.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/edge_computing/__init__.py
--rw-rw-rw-   0        0        0      670 2023-05-25 08:19:46.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/edge_computing/edge_computing.py
--rw-rw-rw-   0        0        0      345 2023-05-25 07:58:59.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
--rw-rw-rw-   0        0        0     5342 2023-05-29 08:19:20.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
--rw-rw-rw-   0        0        0     5007 2023-05-29 08:07:23.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/edge_computing/python_edge_computing_locators.py
--rw-rw-rw-   0        0        0     2365 2023-05-29 08:24:24.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/ingateway.py
--rw-rw-rw-   0        0        0     4051 2023-05-25 08:40:52.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/locale.yml
--rw-rw-rw-   0        0        0      767 2023-05-25 07:59:28.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/locators.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:53:07.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/__init__.py
--rw-rw-rw-   0        0        0     6939 2023-05-25 02:09:36.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/acl_locators.py
--rw-rw-rw-   0        0        0     3783 2023-05-24 10:28:05.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/bridge_locators.py
--rw-rw-rw-   0        0        0    15320 2023-05-24 10:28:05.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/cellular_locators.py
--rw-rw-rw-   0        0        0     3388 2023-05-24 10:28:05.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/dhcp_locators.py
--rw-rw-rw-   0        0        0     2457 2023-05-24 10:28:05.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/dns_locators.py
--rw-rw-rw-   0        0        0     5274 2023-05-24 10:28:05.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/ethernet_locators.py
--rw-rw-rw-   0        0        0     7476 2023-05-25 08:45:27.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/firewall.py
--rw-rw-rw-   0        0        0     8415 2023-05-24 10:28:05.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/gps_locators.py
--rw-rw-rw-   0        0        0      470 2023-05-23 03:37:38.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/host_list_locators.py
--rw-rw-rw-   0        0        0    11017 2023-05-25 06:05:46.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/l2tp_locators.py
--rw-rw-rw-   0        0        0     3667 2023-05-24 10:28:05.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/lan_locators.py
--rw-rw-rw-   0        0        0     2341 2023-05-24 10:28:05.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/loopback_locators.py
--rw-rw-rw-   0        0        0     5698 2023-05-25 02:19:26.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/nat_locators.py
--rw-rw-rw-   0        0        0     2628 2023-05-25 05:59:23.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/network.py
--rw-rw-rw-   0        0        0    32342 2023-05-25 08:09:35.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/network_interface.py
--rw-rw-rw-   0        0        0     1745 2023-05-25 03:11:00.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/network_locators.py
--rw-rw-rw-   0        0        0    13074 2023-05-25 08:09:35.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/network_services.py
--rw-rw-rw-   0        0        0     4371 2023-05-25 01:08:23.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/routing.py
--rw-rw-rw-   0        0        0     1305 2023-05-23 06:46:19.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/routing_status_locators.py
--rw-rw-rw-   0        0        0     2972 2023-05-24 10:28:05.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/static_routing_locators.py
--rw-rw-rw-   0        0        0     9910 2023-05-25 05:58:37.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/vpn.py
--rw-rw-rw-   0        0        0     5208 2023-05-24 10:28:05.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/wan_locators.py
--rw-rw-rw-   0        0        0    10254 2023-05-24 10:28:05.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/wlan_locators.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:53:07.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/overview/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/overview/__init__.py
--rw-rw-rw-   0        0        0     6971 2023-05-25 08:09:35.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/overview/overview.py
--rw-rw-rw-   0        0        0     6260 2023-05-18 07:02:23.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/overview/overview_locators.py
--rw-rw-rw-   0        0        0      303 2023-05-15 09:37:04.000000 inhandtest-0.0.50/inhandtest/pages/locale.py
--rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.50/inhandtest/pytest_email.html
--rw-rw-rw-   0        0        0    32773 2023-05-16 10:13:54.000000 inhandtest-0.0.50/inhandtest/telnet.py
--rw-rw-rw-   0        0        0    25490 2023-05-31 02:52:16.000000 inhandtest-0.0.50/inhandtest/tools.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:53:07.000000 inhandtest-0.0.50/inhandtest.egg-info/
--rw-rw-rw-   0        0        0      593 2023-05-31 02:53:07.000000 inhandtest-0.0.50/inhandtest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2784 2023-05-31 02:53:07.000000 inhandtest-0.0.50/inhandtest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 02:53:07.000000 inhandtest-0.0.50/inhandtest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2023-05-31 02:53:07.000000 inhandtest-0.0.50/inhandtest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-31 02:53:07.000000 inhandtest-0.0.50/inhandtest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      137 2023-05-15 07:42:26.000000 inhandtest-0.0.50/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 02:53:07.000000 inhandtest-0.0.50/setup.cfg
--rw-rw-rw-   0        0        0     1614 2023-05-31 02:52:54.000000 inhandtest-0.0.50/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:31:01.000000 inhandtest-0.0.51/
+-rw-rw-rw-   0        0        0       81 2023-04-13 01:59:22.000000 inhandtest-0.0.51/MANIFEST.in
+-rw-rw-rw-   0        0        0      593 2023-06-01 09:31:01.000000 inhandtest-0.0.51/PKG-INFO
+-rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.51/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 09:31:01.000000 inhandtest-0.0.51/dm/
+-rw-rw-rw-   0        0        0     1307 2023-04-26 07:13:22.000000 inhandtest-0.0.51/dm/mqtt.py
+-rw-rw-rw-   0        0        0     3565 2023-04-28 07:00:23.000000 inhandtest-0.0.51/dm/register_v1.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:31:01.000000 inhandtest-0.0.51/inhandtest/
+-rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.51/inhandtest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:31:01.000000 inhandtest-0.0.51/inhandtest/base_page/
+-rw-rw-rw-   0        0        0      330 2023-05-31 07:35:39.000000 inhandtest-0.0.51/inhandtest/base_page/__init__.py
+-rw-rw-rw-   0        0        0    39706 2023-05-31 08:51:14.000000 inhandtest-0.0.51/inhandtest/base_page/_ig_contents_locators.py
+-rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.51/inhandtest/base_page/_ir3XX_contents_locators.py
+-rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.51/inhandtest/base_page/_vg710_contents_locators.py
+-rw-rw-rw-   0        0        0    58057 2023-06-01 03:29:00.000000 inhandtest-0.0.51/inhandtest/base_page/base_page.py
+-rw-rw-rw-   0        0        0    23326 2023-06-01 01:06:15.000000 inhandtest-0.0.51/inhandtest/base_page/table_tr.py
+-rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.51/inhandtest/exception.py
+-rw-rw-rw-   0        0        0     3895 2023-06-01 09:18:53.000000 inhandtest-0.0.51/inhandtest/file.py
+-rw-rw-rw-   0        0        0    11861 2023-05-06 01:56:01.000000 inhandtest-0.0.51/inhandtest/inmodbus.py
+-rw-rw-rw-   0        0        0     4880 2023-04-27 01:05:22.000000 inhandtest-0.0.51/inhandtest/inmongodb.py
+-rw-rw-rw-   0        0        0    22057 2023-06-01 09:18:53.000000 inhandtest-0.0.51/inhandtest/inmqtt.py
+-rw-rw-rw-   0        0        0    51904 2023-06-01 09:15:20.000000 inhandtest-0.0.51/inhandtest/inrequest.py
+-rw-rw-rw-   0        0        0     7588 2023-06-01 09:15:20.000000 inhandtest-0.0.51/inhandtest/inserial.py
+-rw-rw-rw-   0        0        0    14360 2023-06-01 09:15:20.000000 inhandtest-0.0.51/inhandtest/insocket.py
+-rw-rw-rw-   0        0        0     6854 2023-06-01 09:15:20.000000 inhandtest-0.0.51/inhandtest/inssh.py
+-rw-rw-rw-   0        0        0     1569 2023-05-24 09:45:24.000000 inhandtest-0.0.51/inhandtest/ip.py
+-rw-rw-rw-   0        0        0    11625 2023-06-01 09:15:20.000000 inhandtest-0.0.51/inhandtest/mail.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:31:01.000000 inhandtest-0.0.51/inhandtest/pages/
+-rw-rw-rw-   0        0        0      230 2023-05-31 07:29:45.000000 inhandtest-0.0.51/inhandtest/pages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:31:01.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/
+-rw-rw-rw-   0        0        0      136 2023-05-31 07:30:00.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:31:01.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/edge_computing/
+-rw-rw-rw-   0        0        0      134 2023-05-25 07:33:25.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/edge_computing/__init__.py
+-rw-rw-rw-   0        0        0     6182 2023-06-01 03:29:35.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/edge_computing/docker_manager_locators.py
+-rw-rw-rw-   0        0        0      878 2023-06-01 03:02:00.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/edge_computing/edge_computing.py
+-rw-rw-rw-   0        0        0      469 2023-06-01 02:49:02.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
+-rw-rw-rw-   0        0        0    10706 2023-06-01 03:16:20.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
+-rw-rw-rw-   0        0        0     6112 2023-06-01 01:34:12.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/edge_computing/python_edge_computing_locators.py
+-rw-rw-rw-   0        0        0     2531 2023-06-01 09:19:48.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/ingateway.py
+-rw-rw-rw-   0        0        0     4165 2023-06-01 03:13:15.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/locale.yml
+-rw-rw-rw-   0        0        0      767 2023-05-25 07:59:28.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/locators.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:31:01.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/__init__.py
+-rw-rw-rw-   0        0        0     6939 2023-05-25 02:09:36.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/acl_locators.py
+-rw-rw-rw-   0        0        0     3783 2023-05-24 10:28:05.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/bridge_locators.py
+-rw-rw-rw-   0        0        0    15320 2023-05-24 10:28:05.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/cellular_locators.py
+-rw-rw-rw-   0        0        0     3388 2023-05-24 10:28:05.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/dhcp_locators.py
+-rw-rw-rw-   0        0        0     2457 2023-05-24 10:28:05.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/dns_locators.py
+-rw-rw-rw-   0        0        0     5274 2023-05-24 10:28:05.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/ethernet_locators.py
+-rw-rw-rw-   0        0        0     7476 2023-05-25 08:45:27.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/firewall.py
+-rw-rw-rw-   0        0        0     8415 2023-05-24 10:28:05.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/gps_locators.py
+-rw-rw-rw-   0        0        0      470 2023-05-23 03:37:38.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/host_list_locators.py
+-rw-rw-rw-   0        0        0    11017 2023-05-25 06:05:46.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/l2tp_locators.py
+-rw-rw-rw-   0        0        0     3667 2023-05-24 10:28:05.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/lan_locators.py
+-rw-rw-rw-   0        0        0     2341 2023-05-24 10:28:05.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/loopback_locators.py
+-rw-rw-rw-   0        0        0     5698 2023-05-25 02:19:26.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/nat_locators.py
+-rw-rw-rw-   0        0        0     2628 2023-05-25 05:59:23.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/network.py
+-rw-rw-rw-   0        0        0    32342 2023-05-25 08:09:35.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/network_interface.py
+-rw-rw-rw-   0        0        0     1745 2023-05-25 03:11:00.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/network_locators.py
+-rw-rw-rw-   0        0        0    13074 2023-05-25 08:09:35.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/network_services.py
+-rw-rw-rw-   0        0        0     4371 2023-05-25 01:08:23.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/routing.py
+-rw-rw-rw-   0        0        0     1305 2023-05-23 06:46:19.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/routing_status_locators.py
+-rw-rw-rw-   0        0        0     2972 2023-05-24 10:28:05.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/static_routing_locators.py
+-rw-rw-rw-   0        0        0     9910 2023-05-25 05:58:37.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/vpn.py
+-rw-rw-rw-   0        0        0     5208 2023-05-24 10:28:05.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/wan_locators.py
+-rw-rw-rw-   0        0        0    10254 2023-05-24 10:28:05.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/wlan_locators.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:31:01.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/overview/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/overview/__init__.py
+-rw-rw-rw-   0        0        0     6971 2023-05-25 08:09:35.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/overview/overview.py
+-rw-rw-rw-   0        0        0     6260 2023-05-18 07:02:23.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/overview/overview_locators.py
+-rw-rw-rw-   0        0        0      303 2023-05-15 09:37:04.000000 inhandtest-0.0.51/inhandtest/pages/locale.py
+-rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.51/inhandtest/pytest_email.html
+-rw-rw-rw-   0        0        0    33736 2023-06-01 08:56:40.000000 inhandtest-0.0.51/inhandtest/telnet.py
+-rw-rw-rw-   0        0        0    25747 2023-06-01 09:03:09.000000 inhandtest-0.0.51/inhandtest/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:31:01.000000 inhandtest-0.0.51/inhandtest.egg-info/
+-rw-rw-rw-   0        0        0      593 2023-06-01 09:31:01.000000 inhandtest-0.0.51/inhandtest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2838 2023-06-01 09:31:01.000000 inhandtest-0.0.51/inhandtest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 09:31:01.000000 inhandtest-0.0.51/inhandtest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2023-06-01 09:31:01.000000 inhandtest-0.0.51/inhandtest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-01 09:31:01.000000 inhandtest-0.0.51/inhandtest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      137 2023-05-15 07:42:26.000000 inhandtest-0.0.51/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 09:31:01.000000 inhandtest-0.0.51/setup.cfg
+-rw-rw-rw-   0        0        0     1614 2023-06-01 09:30:50.000000 inhandtest-0.0.51/setup.py
```

### Comparing `inhandtest-0.0.50/PKG-INFO` & `inhandtest-0.0.51/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: inhandtest
-Version: 0.0.50
+Version: 0.0.51
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 Maintainer: liwei
 Maintainer-email: liwei@inhand.com.cn
 License: UNKNOWN
```

### Comparing `inhandtest-0.0.50/README.md` & `inhandtest-0.0.51/README.md`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/dm/mqtt.py` & `inhandtest-0.0.51/dm/mqtt.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/dm/register_v1.py` & `inhandtest-0.0.51/dm/register_v1.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/inhandtest/base_page/_ig_contents_locators.py` & `inhandtest-0.0.51/inhandtest/base_page/_ig_contents_locators.py`

 * *Files 0% similar despite different names*

```diff
@@ -459,19 +459,19 @@
                 }
             },
             'edge_computing': {
                 'default': 'python_edge_computing',
                 'menu': self.edge_menu,
                 'visible_locator': [
                     self.page.locator('//span[@class="ant-breadcrumb-link"]/a[@href="/edge-computing"]').last],
-                'wait_locator': [self.content_target('python_edge').nth(1)],
+                'wait_locator': [self.content_target('python_edge').last],
                 'python_edge_computing': {
                     'menu': self.python_edge_menu,
-                    'visible_locator': [self.content_target('python_edge').nth(1)],
-                    'wait_locator': [self.content_target('python_edge').nth(1)]
+                    'visible_locator': [self.content_target('python_edge').last],
+                    'wait_locator': [self.content_target('python_edge').last]
                 },
                 'docker_manager': {
                     'menu': self.docker_manager_menu,
                     'visible_locator': [self.content_target('docker_manager').nth(1)],
                     'wait_locator': [self.content_target('docker_manager').nth(1)]
                 },
                 'cloud_edge_computing': {
```

### Comparing `inhandtest-0.0.50/inhandtest/base_page/_ir3XX_contents_locators.py` & `inhandtest-0.0.51/inhandtest/base_page/_ir3XX_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/inhandtest/base_page/_vg710_contents_locators.py` & `inhandtest-0.0.51/inhandtest/base_page/_vg710_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/inhandtest/base_page/base_page.py` & `inhandtest-0.0.51/inhandtest/base_page/base_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -540,15 +540,15 @@
         :return:
         """
         if file_path is not None:
             if os.path.isdir(file_path) and os.path.exists(file_path):
                 with self.page.expect_download() as download_info:
                     locator.click()
                 download = download_info.value
-                file_name = download.suggested_filename if file_name is not None else file_name
+                file_name = download.suggested_filename if file_name is None else file_name
                 download.save_as(path.join(file_path, file_name))
                 logging.info(
                     f'Device {self.host} download {download.suggested_filename} to path {file_path} successful')
             else:
                 logging.error(f'{file_path} Does Not Exist.')
 
     @allure.step("校验dialog message")
@@ -650,19 +650,21 @@
         """
         if self.model in ('IG902', 'IG502'):
             tr = IgTable(locators.get('columns'), locators.get('locator'), locators.get('param'), log_desc,
                          locators.get('action_confirm'), locators.get('pop_up_locator'))
             exist_tr = []
             if value:
                 for value_ in value:
-                    if value_[0] == 'add':
+                    if value_[0] in ('add', 'install'):
                         tr.add(self.agg_in, **value_[1])
+                        if value_[0] == 'install':  # app 的安装，安装完成页面要重新加载，需要固定等点时间
+                            self.page.wait_for_timeout(5000)
                     elif value_[0] == 'delete_all':
                         tr.delete_all()
-                    elif value_[0] in ('delete', 'clear_log', 'uninstall'):
+                    elif value_[0] in ('delete', 'uninstall'):
                         tr.delete(value_[1])
                     elif value_[0] == 'exist':
                         exist_tr.append(tr.exist(value_[1], self.locale))
                     elif value_[0] == 'edit':
                         tr.edit(self.agg_in, value_[1], **value_[2])
                     elif value_[0] == 'connect':
                         tr.connect(value_[1])
@@ -684,14 +686,16 @@
                         tr.start(value_[1])
                     elif value_[0] == 'stop':
                         tr.stop(value_[1])
                     elif value_[0] == 'restart':
                         tr.restart(value_[1])
                     elif value_[0] in ('check', 'enable'):
                         tr.check(self.check, value_[1], value_[2])
+                    elif value_[0] == 'clear_log':
+                        tr.clear_log(value_[1])
                 return exist_tr
         else:
             tr = Table(locators.get('columns'), locators.get('locator'),
                        locators.get('unique_columns'), locators.get('param'), log_desc)
             exist_tr = []
             if value:
                 for value_ in value:
@@ -724,16 +728,14 @@
                     "param":{$key, $value}: 参数转换，如大小写转换{"ab":"AB"} {"wan":"Wan"}等.
                 :param action_dict: 要做操作的参数名称与对应的值{$param1: $value1, $param2: $value2}
                 :return:
                 """
         relations = []
 
         def operation(param, param_locator, value):
-            if param_locator.get('wait_for'):
-                self.page.wait_for_timeout(param_locator.get('wait_for'))
             if param_locator.get('type') == 'text':
                 self.fill(param_locator.get('locator'), value, param)
             elif param_locator.get('type') == 'select':
                 if param_locator.get('param') and value in param_locator.get('param').keys():
                     value = param_locator.get('param').get(value)
                 self.select_option(param_locator.get('locator'), value, param)
             elif param_locator.get('type') == 'radio_select':
@@ -749,16 +751,24 @@
                     dialog_message, tip_messages, wait_for_time, tip_messages_timeout = None, None, None, 30
                     if isinstance(value, dict):
                         dialog_message = value.get('dialog_message')
                         tip_messages = value.get('tip_messages')
                         wait_for_time = value.get('wait_for_time')
                         tip_messages_timeout = value.get('tip_messages_timeout') if value.get(
                             'tip_messages_timeout') is not None else 30
-                    self.click(param_locator.get('locator'), param, dialog_message, tip_messages, wait_for_time,
-                               tip_messages_timeout)
+                    if isinstance(param_locator.get('locator'), Locator):
+                        self.click(param_locator.get('locator'), param, dialog_message, tip_messages, wait_for_time,
+                                   tip_messages_timeout)
+                    elif isinstance(param_locator.get('locator'), list) or isinstance(param_locator.get('locator'),
+                                                                                      tuple):  # 二次确认
+                        self.click(param_locator.get('locator')[0], param, dialog_message, tip_messages, wait_for_time,
+                                   tip_messages_timeout)
+                        self.click(param_locator.get('locator')[1], 'confirm', wait_for_time=1000)
+                    else:
+                        raise Exception(f'locator {param_locator.get("locator")} is not a Locator or list or tuple')
             elif param_locator.get('type') == 'check':
                 if value:
                     value_, tip_messages = value, None
                     if isinstance(value, dict):
                         value_ = value.get('value')
                         tip_messages = value.get('tip_messages')
                     self.check(param_locator.get('locator'), value_, param, tip_messages)
@@ -817,14 +827,24 @@
                     messages, timeout = value, 10
                     if isinstance(value, dict):
                         timeout = value.get('timeout') if value.get('timeout') else 10
                         messages = value.get('messages')
                     self.title_messages(messages, timeout)
             else:
                 raise Exception(f"not support this param type {param_locator.get('type')}")
+            if param_locator.get('wait_for'):
+                wait_for = [param_locator.get('wait_for')] if isinstance(param_locator.get('wait_for'),
+                                                                         dict) else param_locator.get('wait_for')
+                for wait_for_ in wait_for:
+                    if wait_for_.get('type') == 'timeout':
+                        self.page.wait_for_timeout(wait_for_.get('timeout'))
+                    elif wait_for_.get('type') == 'visible':
+                        wait_for_.get('locator').wait_for(state='visible', timeout=wait_for_.get('timeout'))
+                    elif wait_for_.get('type') == 'hidden':
+                        wait_for_.get('locator').wait_for(state='hidden', timeout=wait_for_.get('timeout'))
 
         if action_dict:
             for option in locators:
                 assert type(option) in (tuple, list) and len(option) == 2, "type of option is incorrect"
                 if option[0] in [key for key, value in action_dict.items() if value is not None]:
                     if option[1].get("relation") and option[1].get("relation") not in relations:
                         # 对关系项操作之前检查关系项
@@ -845,29 +865,31 @@
                         '"${value}".startswith("123")', '"${value}".endswith("23")', '"${value}" in a', '"${value}" not in b',
                         '"${value}".__contains__("234")', 'time.strptime("${value}}", "%Y-%m-%d %H:%M:%S")'）
                         ex: '${value}==8' 多个使用元组或者列表，注意期望值是字符串时需要带上引号， 如'${value}=="sim1"'
         :param locators: [($param1, {"locator": $locator1, "type": $type1, "relation": [($param2, $value2)], "param": {$key1: $value1}}),
                           ($param2, {"locator": $locator2, "type": $type2, "relation": [($param3, $value3),……], "param": {$key2: $value2}}),
                           ($param3, {"locator": $locator2, "type": 'table_tr', "relation": [($param3, $value3),……], "param": {$key2: $value2},
                                 "columns": list, 'unique_columns': list}),]
-                          type:  text, switch_button
+                          type:  text, switch_button, fill
 
         :return: 只返回True or False 不做断言
         """
         if expect_:
             for key in expect_.keys():
                 filter_key = list(filter(lambda x: x[0] == key, locators))
                 if len(filter_key) == 1:
                     option = filter_key[0]
                     locator = option[1].get('locator')
                     if option[1].get('type') == 'switch_button':
                         if 'ant-switch-checked' in locator.first.get_attribute('class'):
                             value = 'enable'
                         else:
                             value = 'disable'
+                    elif option[1].get('type') == 'fill':
+                        value = locator.first.input_value()
                     else:  # type is text
                         if isinstance(locator, Locator):
                             value = locator.first.inner_text() if locator.count() != 0 else 'None'
                         else:
                             value = str(locator)
                     try:
                         if '${value}' in expect_.get(key):
```

### Comparing `inhandtest-0.0.50/inhandtest/base_page/table_tr.py` & `inhandtest-0.0.51/inhandtest/base_page/table_tr.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 # @File    : table_tr.py
 """
 table_tr
 
 """
 import logging
 import re
+import time
 from typing import List
 from inhandtest.tools import replace_str
-from playwright.sync_api import Locator
+from playwright.sync_api import Locator, TimeoutError
 
 
 class Table:
 
     def __init__(self, columns: list, table_locator: Locator, unique_columns: list, locale: dict = None, log_desc=None):
         """
 
@@ -323,18 +324,21 @@
     def delete(self, value: str) -> None:
         """
         :param value str, 待删除列 及对应值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值 自己国际化
         :return:
         """
         value = replace_str(value, self.locale)
         exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
-        while exist_tr.count() > 0:
+        exist_tr_number = exist_tr.count()
+        for i in range(0, exist_tr_number):
             exist_tr.first.locator('//i[@class="anticon anticon-delete"]').click()
             if isinstance(self.action_confirm, Locator):
                 self.action_confirm.click()  # 二次确认
+            while exist_tr.count() + i + 1 != exist_tr_number:   # 等待删除完成,
+                self.table_locator.page.wait_for_timeout(500)
         logging.info(f'table resource {value} all delete')
 
     def associate_delete(self, value: str) -> None:
         """
         :param value str, 关联删除按钮，如VPN 中l2tp client表格中的删除按钮
         :return:
         """
@@ -351,27 +355,28 @@
         :param file_path: str, 下载文件存放路径
         :param file_name: str, 下载文件名
         :return:
         """
         value = replace_str(value, self.locale)
         exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
         if exist_tr.count() > 0:
-            action(exist_tr.first.locator('//i[@class="anticon.anticon-download"]').first, file_path, file_name=file_name)
+            action(exist_tr.first.locator('//i[@class="anticon anticon-download"]').first, file_path,
+                   file_name=file_name)
         logging.info(f'table resource {value} download success')
 
     def upload(self, action, value, file_path):
         """
         :param action: function, 导致该方法不能单独使用
         :param value str, 待上传列 及对应值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值 自己国际化
         :param file_path: str, 上传文件全路径
         :return:
         """
         exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
         if exist_tr.count() > 0:
-            exist_tr.first.locator('//i[@class="anticon.anticon-upload"]').click()
+            exist_tr.first.locator('//i[@class="anticon anticon-upload"]').click()
             action(self.pop_up_locator.locator('.anticon.anticon-upload').nth(0), file_path)
             self.pop_up_locator.locator('.ant-btn.ant-btn-primary').nth(0).click()
         logging.info(f'table resource {value}  click upload')
 
     def check(self, action, value, check_value):
         """
         :param action: function, 导致该方法不能单独使用
@@ -419,14 +424,27 @@
         exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
         if exist_tr.count() > 0:
             exist_tr.first.locator('//i[@class="anticon anticon-undo"]').first.click()
             if isinstance(self.action_confirm, Locator):
                 self.action_confirm.click()  # 二次确认
         logging.info(f'table resource {value} all restart')
 
+    def clear_log(self, value: str) -> None:
+        """
+        :param value str, 待开始列 及对应值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值 自己国际化
+        :return:
+        """
+        value = replace_str(value, self.locale)
+        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
+        if exist_tr.count() > 0:
+            exist_tr.first.locator('//i[@class="anticon anticon-delete"]').first.click()
+            if isinstance(self.action_confirm, Locator):
+                self.action_confirm.click()  # 二次确认
+        logging.info(f'table resource {value} all clear log')
+
     def connect(self, value: str) -> None:
         """
         :param value str, WLAN 页面connect连接，每列值可按顺序直接连接在一起传入，当然也可以传一列的值
         :return:
         """
         exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
         if exist_tr.count() > 0:
```

### Comparing `inhandtest-0.0.50/inhandtest/exception.py` & `inhandtest-0.0.51/inhandtest/exception.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/inhandtest/file.py` & `inhandtest-0.0.51/inhandtest/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,38 +24,38 @@
             if os.path.isdir(c_path):
                 del_file(c_path)
             else:
                 os.remove(c_path)
     elif os.path.isfile(file_path):
         os.remove(file_path)
     else:
-        logging.info(f"parameter file_path {file_path} is not exist")
+        logging.debug(f"parameter file_path {file_path} is not exist")
 
 
 def check_file(file_path_or_file_dir, create_dir=True) -> None:
     """校验文件夹以及文件是否存在, 如果文件夹不存在则创建，如果文件不存在则抛出异常
 
     :param file_path_or_file_dir: 文件夹路径或者文件路径
     :param create_dir: 当检测出文件夹不存在时就创建
     :return:  检查到文件不存在时就抛异常FileNotFoundError
     """
     if os.path.isdir(file_path_or_file_dir):
         if os.path.exists(file_path_or_file_dir):
-            logging.info(f"check dir {file_path_or_file_dir} ok")
+            logging.debug(f"check dir {file_path_or_file_dir} ok")
         else:
             if create_dir:
                 os.mkdir(file_path_or_file_dir)
-                logging.info(f"create dir {file_path_or_file_dir} ok")
+                logging.debug(f"create dir {file_path_or_file_dir} ok")
             else:
                 raise FileNotFoundError(f"this file {file_path_or_file_dir} not exist")
     else:
         if not os.path.isfile(file_path_or_file_dir):
             raise FileNotFoundError(f"this file {file_path_or_file_dir} not exist")
         else:
-            logging.info(f"check file {file_path_or_file_dir} ok")
+            logging.debug(f"check file {file_path_or_file_dir} ok")
 
 
 def generate_str_or_file(size: int or str = '48KB', file_path=None) -> str:
     """生成指定大小字符串或文件 1024KB=1MB  1024MB=1GB  1024GB=1TB
 
     :param size: int or str, int时单位为字节， str可带单位'KB'|'MB'|'GB', e.g: 49152|'48KB'...
     :param file_path: 文件全路径，ex: /$file_path/test.txt 将内容写道文件中
@@ -75,15 +75,15 @@
     else:
         raise Exception(f'param {size} type {type(size)} error, only can be str or int!')
     if size:  # 都已经转换为byte
         str_ = ''.join(random.choice(string.ascii_letters + string.digits) for _ in range(size))
         if os.path.isfile(file_path):  # 生成文件
             with open(file_path, 'w') as file:
                 file.write(str_)
-            logging.info(
+            logging.debug(
                 f"file {file_path} success create.Size is {os.path.getsize(file_path)}" + 'Byte')
     return str_
 
 
 def file_hash(file_path_or_msg, hash_type='md5') -> str:
     """
```

### Comparing `inhandtest-0.0.50/inhandtest/inmodbus.py` & `inhandtest-0.0.51/inhandtest/inmodbus.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/inhandtest/inmongodb.py` & `inhandtest-0.0.51/inhandtest/inmongodb.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/inhandtest/inmqtt.py` & `inhandtest-0.0.51/inhandtest/inmqtt.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,27 +63,27 @@
             logging.info(f"{client} Connection success, id: {self.client_id}")
             self.connect_time = int(time.time())
         else:
             logging.error(f'client {self.client_id} connect failed, code=%s' % rc)
 
     def __on_message(self, client, userdata, message):
         try:
-            logging.info(f"client {self.client_id} recv topic '{message.topic}', payload {json.loads(message.payload)}")
+            logging.debug(f"client {self.client_id} recv topic '{message.topic}', payload {json.loads(message.payload)}")
             self.recv_datas.append((message.topic, json.loads(message.payload), int(round(time.time() * 1000))))
         except Exception:
             logging.error(f'client {self.client_id} recv exception data: {message.payload}')
 
     def __on_subscribe(self, client, userdata, mid, granted_qos):
-        logging.info(f'On Subscribed: mid={mid}, qos={granted_qos}')
+        logging.debug(f'On Subscribed: mid={mid}, qos={granted_qos}')
 
     def __on_publish(self, client, userdata, mid):
-        logging.info(f'On onPublish: mid={mid}')
+        logging.debug(f'On onPublish: mid={mid}')
 
     def __on_log(self, client, userdata, level, buf):
-        logging.info(buf)
+        logging.debug(buf)
         if 'WinError 10054' in buf:
             self.disconnect()
 
     def __on_disconnect(self, client, userdata, rc):
         logging.info(f'client {self.client_id} On disconnected: rc={rc}')
         if not self.reconnect_on_failure:
             self.disconnect()
@@ -213,15 +213,15 @@
                                             expect_payload_ = dict_flatten(assert_payload)  # 平铺字典
                                             r_payload_ = dict_flatten(x[1])
                                             for expect_item_, expect_value_ in expect_payload_.items():
                                                 if expect_item_ not in ('number', 'exist', 'time_interval'):
                                                     value_ = r_payload_.get(expect_item_)
                                                     expect_value_ = str(expect_value_).replace('${value}', str(value_))
                                                     if not eval(expect_value_):
-                                                        logging.info(expect_value_)
+                                                        logging.debug(expect_value_)
                                                         raise AssertionError(
                                                             f'payload error parm {expect_item_} value is {expect_value_} is False')
 
                                     [payload_verify(data_) for data_ in self.recv_datas]
                             else:
                                 raise Exception('param expect_recv_rules topic value must be boolean or dict')
                 else:
@@ -264,16 +264,16 @@
             logging.info(f"mosquitto broker server already start")
             self.close()
         if clear_log:
             open(self.broker_log_file, 'w').close()
         log = open(self.broker_log_file, 'a')
         cnf_file = os.path.join(self.mosquitto_path, config)
         subprocess.Popen(f'"{self.mosquitto_exe}" -c "{cnf_file}" -p {self.port} -v', stdout=log, stderr=log)
-        logging.info(f"start mosquitto broker server success")
-        logging.info(f"mosquitto broker log is {self.broker_log_file}")
+        logging.debug(f"start mosquitto broker server success")
+        logging.debug(f"mosquitto broker log is {self.broker_log_file}")
 
     def broker_user(self, username, password, type_='add', filename='pwfile.example') -> None:
         """ 添加删除更新服务的用户
 
         :param username: 用户名
         :param password: 密码
         :param filename: 存储文件密码文件
@@ -325,15 +325,15 @@
         """
         if clear_log:
             open(self.sub_log_file, 'w').close()
         log = open(self.sub_log_file, 'a')
         param = param + ' -v' if '-v' not in param else param
         p = subprocess.Popen(f'"{self.mosquitto_sub}" {param}', stdout=log, stderr=log)
         logging.info(f"mosquitto sub {param} success")
-        logging.info(f"mosquitto sub log path is {log}")
+        logging.debug(f"mosquitto sub log path is {log}")
         return p.pid
 
     def pub(self, param: str) -> None:
         """ 发布Topic
 
         :param param: '-h 10.5.24.224 -p 1883 -t v1/VG7102022101801/# -u admin -P 123456 -m message'
         :return:
```

### Comparing `inhandtest-0.0.50/inhandtest/inrequest.py` & `inhandtest-0.0.51/inhandtest/inrequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         :return:
         """
         for i in range(0, timeout, interval):
             response = self.api.send_request('api/devices', method='get',
                                              param={"verbose": 100, "limit": 10, "cursor": 0,
                                                     'serial_number': sn})
             if response.json().get('total') == 1:
-                logging.info(f'check {sn} device exist')
+                logging.debug(f'check {sn} device exist')
                 break
             logging.info(f'check {sn} device is not exist, please wait for {interval}s')
             time.sleep(interval)
         else:
             raise TimeOutError(f'{self.host} {self.username} account not found device {sn}')
 
     def device_state(self, sn: list) -> List[dict]:
@@ -211,26 +211,26 @@
         if state:
             import ipaddress
             for i in range(0, timeout, interval):
                 result = self.device_state([sn])[0]
                 for key, value in state.items():
                     if '${value}' in value:
                         value = replace_str(value, {'${value}': result.get(key)})
-                        logging.info(f'start assert {sn} state {key} {value}')
+                        logging.debug(f'start assert {sn} state {key} {value}')
                         try:
                             if not eval(value, {'ipaddress': ipaddress}):
-                                logging.info(f'the {sn} device {key} info eval {value} is false')
+                                logging.debug(f'the {sn} device {key} info eval {value} is false')
                                 break
                         except Exception as e:
                             logging.error(e)
                             break
                     else:
-                        logging.info(f'start assert {sn} state {key} {value}')
+                        logging.debug(f'start assert {sn} state {key} {value}')
                         if result.get(key) != value:
-                            logging.info(f'the {sn} device {key} info value is {result.get(key)} not {value}')
+                            logging.debug(f'the {sn} device {key} info value is {result.get(key)} not {value}')
                             break
                 else:
                     logging.info(f"check {sn} device all state success")
                     break
                 logging.info(f"check {sn} device state failed, please wait for {interval}s")
                 time.sleep(interval)
             else:
@@ -329,15 +329,15 @@
                                 'version': version(file_name), 'desc': 'auto test upload firmware'}
                         firmware_id = self.api.send_request('api/firmware', 'post', body=body, ).json().get(
                             'result').get(
                             '_id')
                     else:
                         raise FileNotFoundError(f'{firmware} not exist')
                 else:
-                    logging.info(f'This file {firmware} already exists on the cloud {self.host} {self.username}')
+                    logging.debug(f'This file {firmware} already exists on the cloud {self.host} {self.username}')
                     firmware_id = get_firmware.get('result')[0].get('_id')
                 # 已完成固件上传
                 job_id = self.api.send_request(f'api/device/{device_id}/upgrade', method='post',
                                                body={'deviceName': device_name, 'firmwareId': firmware_id,
                                                      'timeout': int(timeout / 60)}).json().get('result').get('_id')
                 for i in range(0, timeout, interval):
                     time.sleep(interval)
@@ -354,15 +354,15 @@
                                 raise UpgradeFailedError(f'upgrade to {file_name} failed!')
                     else:
                         raise UpgradeFailedError('create upgrade task failed!')
                 else:
                     raise TimeOutError('upgrade job check timeout')
                 self.assert_device_state(sn, state={'version': '"${value}" in ' + f'"{file_name}"'}, timeout=300)
             else:
-                logging.info(f'{firmware} not is file or version of same ')
+                logging.debug(f'{firmware} not is file or version of same ')
         else:
             raise Exception(f'the device {sn} is offline or not exist')
 
     def upgrade_firmware(self, sn: str or list, firmware: str) -> None:
         """ 升级固件，只管下发升级任务，不监督是否升级成功
 
         :param sn: 设备序列号
@@ -395,20 +395,20 @@
                             'version': version(file_name), 'desc': 'auto test upload firmware'}
                     firmware_id = self.api.send_request('api/firmware', 'post', body=body, ).json().get(
                         'result').get(
                         '_id')
                 else:
                     raise FileNotFoundError(f'{firmware} not exist')
             else:
-                logging.info(f'This file {firmware} already exists on the cloud {self.host} {self.username}')
+                logging.debug(f'This file {firmware} already exists on the cloud {self.host} {self.username}')
                 firmware_id = get_firmware.get('result')[0].get('_id')
             self.api.send_request(f'api/firmware/{firmware_id}/devices', method='post',
                                   body={'deviceIds': [device.get('id') for device in devices], 'deviceGroupIds': [], })
         else:
-            logging.info(f'{firmware} not is file or device is not exist')
+            logging.debug(f'{firmware} not is file or device is not exist')
 
     def web_remote_online(self, sn: str) -> str:
         """封装远程web访问方法
 
         :param sn: str, 设备序列号
         :return: 远程web管理链接
         """
@@ -444,15 +444,15 @@
         """DM平台设备重启
         """
         response = self.api.send_request('api/devices', method='get',
                                          param={"verbose": 100, "limit": 10, "cursor": 0,
                                                 'serial_number': sn})
         if response.json().get('total') == 1 and response.json().get('result')[0].get('online') == 1:
             device_id = response.json().get('result')[0].get('_id')
-            logging.info(f'{self.host} send to {sn} reboot command')
+            logging.debug(f'{self.host} send to {sn} reboot command')
             status = self.api.send_request(f'api/device/{device_id}/methods', 'post',
                                            body={'method': "reboot", 'timeout': 15000}).json().get('status')
             assert status == 'succeeded', 'reboot error!'
         else:
             raise ResourceNotFoundError(f'the {sn} is not exist or offline')
 
     def remote_maintenance_online(self, sn: str, protocol='http', port=80, local_host='192.168.2.1',
@@ -486,39 +486,39 @@
                                'localAddress': local_host, 'localPort': port, 'deviceId': device_id}
             tunnel_id, tunnel_status, pub_url = find_tunnel(device_id)
             if action == 'connect' and device[0].get('online'):
                 if not tunnel_id:
                     result = self.api.send_request('/api/touch/tunnels', method='post', body=add_tunnel_body).json()
                     tunnel_id = result.get('result').get('_id')
                     tunnel_status = False
-                    logging.info(f'Add {tunnel_des} success, tunnel name is {add_tunnel_body["name"]}')
+                    logging.debug(f'Add {tunnel_des} success, tunnel name is {add_tunnel_body["name"]}')
                 if not tunnel_status:
                     for i in range(0, 3):
                         connect = self.api.send_request(f'/api/touch/tunnels/{tunnel_id}/connect', 'put').json()
                         if connect.get('result').get('connected'):
                             pub_url = connect.get('result').get('publicUrl')
                             logging.info(f'tunnel {tunnel_des} connect success')
                             break
                     else:
                         raise ConnectionError(f'tunnel {tunnel_des} connect failed')
                 else:
-                    logging.info(f'tunnel {tunnel_des} already connect')
+                    logging.debug(f'tunnel {tunnel_des} already connect')
                 return pub_url
             elif action == 'disconnect' and device[0].get('online'):
                 if tunnel_id and tunnel_status:
                     self.api.send_request(f'/api/touch/tunnels/{tunnel_id}/disconnect', 'put')
                     logging.info(f'tunnel {tunnel_des} disconnect success')
                 else:
-                    logging.info(f'tunnel {tunnel_des} not exist or already disconnect')
+                    logging.debug(f'tunnel {tunnel_des} not exist or already disconnect')
             elif action == 'delete':
                 if tunnel_id:
                     self.api.send_request(f'/api/touch/tunnels/{tunnel_id}', 'delete')
                     logging.info(f'tunnel {tunnel_des} delete success')
                 else:
-                    logging.info(f'tunnel {tunnel_des} not exist')
+                    logging.debug(f'tunnel {tunnel_des} not exist')
         else:
             logging.error(f'the device {sn} not exist')
 
     def delete_device(self, sn: str or list) -> None:
         """
 
         :param sn: 设备序列号，一个或多个
@@ -597,15 +597,15 @@
         """
         result = []
         for sn_ in sn:
             response = self.api.send_request('api/invpn/routers', method='get',
                                              param={"limit": 10, "cursor": 0, 'verbose': 100,
                                                     'serialNumber': sn_}).json()
             if response.get('total') == 1:
-                logging.info(f'the device {sn_} exist on {self.host}')
+                logging.debug(f'the device {sn_} exist on {self.host}')
                 res = response.get('result')[0]
                 res_info = self.api.send_request(f'api/devices/{res.get("id")}', method='get',
                                                  param={'verbose': 100}).json().get('result')
                 config_sync = res_info.get('config').get('sync') if res_info.get('config') else None
                 result.append(
                     {'sn': sn_, 'online': res.get('online'), 'iccid': res.get('metadata').get('iccid'),
                      'imei': res.get('metadata').get('imei'), 'imsi': res.get('metadata').get('imsi'),
@@ -750,26 +750,26 @@
         """
         if state:
             for i in range(0, timeout, interval):
                 result = self.device_state([sn])[0]
                 for key, value in state.items():
                     if '${value}' in value:
                         value = replace_str(value, {'${value}': result.get(key)})
-                        logging.info(f'start assert {sn} state {key} {value}')
+                        logging.debug(f'start assert {sn} state {key} {value}')
                         try:
                             if not eval(value):
-                                logging.info(f'the {sn} device {key} info eval {value} is false')
+                                logging.debug(f'the {sn} device {key} info eval {value} is false')
                                 break
                         except Exception as e:
                             logging.error(e)
                             break
                     else:
-                        logging.info(f'start assert {sn} state {key} {value}')
+                        logging.debug(f'start assert {sn} state {key} {value}')
                         if result.get(key) != value:
-                            logging.info(f'the {sn} device {key} info value is {result.get(key)} not {value}')
+                            logging.debug(f'the {sn} device {key} info value is {result.get(key)} not {value}')
                             break
                 else:
                     logging.info(f"check {sn} device all state success")
                     break
                 logging.info(f"check {sn} device state failed, please wait for {interval}s")
                 time.sleep(interval)
             else:
@@ -920,25 +920,25 @@
         elif method == 'PUT':
             if params_type == 'JSON':
                 res = requests.put(url, json=body, params=param, headers=header, verify=False)
             else:
                 res = requests.put(url, data=param, headers=header, verify=False)
         else:
             raise ParameterValueError(f"requests method {method} not support")
-        logging.info(f'Requests Method:[{method}] Code: {res.status_code} URL: {url}, Param: {param}, Body: {body}')
+        logging.debug(f'Requests Method:[{method}] Code: {res.status_code} URL: {url}, Param: {param}, Body: {body}')
         if res.status_code != 401:
             if self.type_ == 'device':
                 if res.status_code == 404:
                     raise Exception('not support API login')
                 if res.status_code == 200 and 'login' in path:
                     if 'error' in res.json().keys():
                         raise UsernameOrPasswordError
             res.encoding = 'utf-8'  # 如返回内容有中文的需要编码正确
             try:
-                logging.info(f'Requests Response json is {res.json()}')
+                logging.debug(f'Requests Response json is {res.json()}')
             except Exception:
                 logging.warning(f'Requests Response json is None')
         else:
             # 当token过期时，统一重新登录后再次调API
             self.__login()
             res = self.send_request(path, method, param, body, expect, file_path, params_type, header, code)
         if code:
```

### Comparing `inhandtest-0.0.50/inhandtest/inserial.py` & `inhandtest-0.0.51/inhandtest/inserial.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,43 +53,43 @@
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
     def __auto_find_com(self):
         if not self.com:
             port_list = list(list_ports.comports())
-            logging.info(port_list)
+            logging.debug(port_list)
             if len(port_list) <= 0:
                 logging.error("The Serial port can't find!")
             else:
                 # 找到第一个可用的串口
                 port_list_0 = list(port_list[0])
                 self.com = port_list_0[0]
 
     def login(self, username=None, password=None):
         username = self.username if not username else username
         password = self.password if not password else password
         try:
             self.serial.write("\n".encode("gbk"))
             flag = self.serial.readlines(2)
-            logging.info(f'{flag[1].decode()}')
+            logging.debug(f'{flag[1].decode()}')
             flag = flag[1].decode("gbk").strip()
             if flag in (self.__config_flag, self.__super_flag, self.__normal_flag, self.__user_flag):
                 pass
             elif 'login:' in flag:
                 self.send_cli({username: ":"})
                 self.serial.write((password + '\n').encode('gbk'))
                 login_flag = self.serial.read_until('>'.encode("gbk")).decode("gbk")
                 if ' \r\n' == login_flag:
                     raise UsernameOrPasswordError
                 else:
                     tag = login_flag.split('\r\n')[-1].strip().replace('>', '')
                     self.__user_flag = f'{tag}#'
                     self.__normal_flag = f'{tag}>'
-                    logging.info(login_flag)
+                    logging.debug(login_flag)
                     pass
             else:
                 logging.error(f'Serial Connect {self.com} Failed')
                 raise ConnectionError
             logging.info(f'Serial Connect {self.com} Successful')
         except Exception:
             raise ConnectionError
@@ -116,15 +116,15 @@
         :param timeout: 接收超时时间
         :param logs_number
         :return:
         """
         self.serial.timeout = 1
         for i in range(0, timeout, 1):
             data = self.serial.readline()  # 获取串口内容
-            logging.info(f'serial com {self.com} read str <{data.decode()}>')
+            logging.debug(f'serial com {self.com} read str <{data.decode()}>')
             if data:
                 self.logs_number.append(data.decode())
             if logs_number == len(self.logs_number):
                 break
             else:
                 time.sleep(1)
         else:
@@ -141,15 +141,15 @@
         @return: 当发送一条命令时直接返回结果，发送多条时返回结果列表
         """
         flag_reacts = []
         if command:
             for com, flag in command.items():
                 self.serial.write(bytes((com + "\r\n").encode("gbk")))
                 flag_react = self.serial.read_until(flag.encode("gbk")).decode("gbk").strip()
-                logging.info(flag_react)
+                logging.debug(flag_react)
                 flag_reacts.append(flag_react)
         if len(flag_reacts) == 1:
             return flag_reacts[0]
         else:
             return flag_reacts
 
     def close(self):
```

### Comparing `inhandtest-0.0.50/inhandtest/insocket.py` & `inhandtest-0.0.51/inhandtest/insocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,44 +33,44 @@
     socket.setdefaulttimeout(timeout)
 
     def client_send_msg_to_server(conn, addr, msg: str or list):
         if msg is not None:
             msg = [msg] if isinstance(msg, str) else [msg_ for msg_ in msg]
             for msg_ in msg:
                 conn.send(msg_.encode('utf-8'))
-                logging.info(f'tcp client {addr} send msg {msg_} to server {host}: {port}')
+                logging.debug(f'tcp client {addr} send msg {msg_} to server {host}: {port}')
 
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:  # 使用with， 不用担心没有关闭server
         s.bind((host, port))  # 绑定服务器IP地址和端口号
         s.listen()  # 等待客户端连接
         try:
             for i_ in range(0, 4):  # 有些端口错误的客户端会连接上来，导致收到的消息始终为空，需要过滤掉
                 client = True
-                logging.info(f'tcp server {host}:{port} start wait client connect')
+                logging.debug(f'tcp server {host}:{port} start wait client connect')
                 __conn, __addr = s.accept()
                 if function is not None:
                     threading.Thread(target=function, kwargs=kwargs).start()
                 with __conn:
                     logging.info(f'tcp server {host}:{port} connect from client {__addr}')
                     datas = b''
                     now_time = int(time.time())
                     send_msg_status = False
                     while int(time.time()) <= now_time + connect_time:
                         # 接收客户端数据
                         recv_data = __conn.recv(1024)
                         if not recv_data:
                             client = False
                             __conn.close()
-                            logging.info(f'client {__addr} is a error client')
+                            logging.debug(f'client {__addr} is a error client')
                             break
                         if not send_msg_status:
                             threading.Thread(target=client_send_msg_to_server,
                                              args=(__conn, __addr, send_msg_to_server)).start()
                             send_msg_status = True
-                        logging.info(f'tcp server {host}:{port} recv client {__addr} data {recv_data}')
+                        logging.debug(f'tcp server {host}:{port} recv client {__addr} data {recv_data}')
                         datas = datas + recv_data
                         all_datas.update({__addr: datas})
                     else:
                         __conn.close()
                 if client:
                     break
         except socket.timeout:
@@ -121,15 +121,15 @@
     datas = b''
 
     def client_send_msg_to_server(client_, msg: str or list):
         if msg is not None:
             msg = [msg] if isinstance(msg, str) else [msg_ for msg_ in msg]
             for msg_ in msg:
                 client_.send(msg_.encode("utf-8"))
-                logging.info(f'tcp client send msg {msg_} to server {server}')
+                logging.debug(f'tcp client send msg {msg_} to server {server}')
 
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:  # 使用with， 不用担心没有关闭server
         if client:
             s.bind(client)  # 绑定客户端IP地址和端口号
         try:
             s.connect(server)  # 客户端连接服务端
             threading.Thread(target=client_send_msg_to_server, args=(s, send_msg_to_server)).start()
@@ -180,22 +180,22 @@
                 msg = [value] if isinstance(value, str) else [value_ for value_ in value]
                 for msg_ in msg:
                     server.sendto(msg_.encode('utf-8'), key)
                     logging.info(f'udp server {host}: {port} send msg {msg_} to client {key}')
 
     with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as s:  # 使用with， 不用担心没有关闭server
         s.bind((host, port))  # 绑定服务器IP地址和端口号
-        logging.info(f'udp server {host}:{port} enable')
+        logging.debug(f'udp server {host}:{port} enable')
         threading.Thread(target=server_send_msg_to_client, args=(s, send_msg_to_client)).start()
         datas = b''
         now_time = int(time.time())
         while int(time.time()) <= now_time + connect_time:
             # 接收客户端数据
             data, addr = s.recvfrom(5024)
-            logging.info(f'udp server {host}:{port} recv data from {addr}: {data}')
+            logging.debug(f'udp server {host}:{port} recv data from {addr}: {data}')
             datas = datas + data
             if recv_content is not None:
                 contents = [recv_content.encode()] if isinstance(recv_content, str) else [c_.encode() for c_ in
                                                                                           recv_content]
                 # 校验数据内容
                 if not list(filter(lambda x: x not in datas, contents)):
                     break
@@ -230,15 +230,15 @@
             s.bind(client)  # 绑定客户端IP地址和端口号
         threading.Thread(target=client_send_msg_to_server, args=(s, send_msg_to_server)).start()
         now_time = int(time.time())
         datas = b''
         while int(time.time()) <= now_time + connect_time:
             # 接收服务端数据
             data, server_addr = s.recvfrom(5024)
-            logging.info(f'upd client recv data from server {server_addr}: {data}')
+            logging.debug(f'upd client recv data from server {server_addr}: {data}')
             datas = datas + data
             if recv_content is not None:
                 contents = [recv_content.encode('utf-8')] if isinstance(recv_content, str) else [c_.encode('utf-8') for
                                                                                                  c_ in recv_content]
                 # 校验数据内容
                 if not list(filter(lambda x: x not in datas, contents)):
                     break
```

### Comparing `inhandtest-0.0.50/inhandtest/inssh.py` & `inhandtest-0.0.51/inhandtest/inssh.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         :return: 返回所有命令执行后的结果
         """
         result = None
         if command:
             stdin, stdout, stderr = self.ssh.exec_command(command)
             logging.info(f'exec command 【{command}】')
             result = stdout.read().decode("utf-8")
-            logging.info(f'command result 【{result}】')
+            logging.debug(f'command result 【{result}】')
         return result
 
     @enable_sftp
     def download_file(self, remote_file, local_file) -> None:
         """
         从服务器上下载文件
         :param remote_file: 远端文件路径
@@ -128,73 +128,73 @@
     def get_file_content(self, file_path: str) -> str:
         """获取文件内容
 
         :param file_path:  文件路径  ex： 'D:\ecoer\sdf.sh'
         :return:
         """
         self.sftp.chdir(os.path.dirname(file_path))
-        logging.info(f'read {file_path} content success')
+        logging.debug(f'read {file_path} content success')
         return self.sftp.file(os.path.basename(file_path), 'r').read().decode(encoding='utf-8')
 
     @enable_sftp
     def write_file_content(self, file_path: str, content: str, mode='w') -> None:
         """像文件写入数据
 
         :param file_path: 文件全路径 ex: 'D:\ecoer\sdf.sh'
         :param content: 写入的文件内容，多行内容使用\n 连接
         :param mode: 'w' 替换文件内容写入， 'a' 追加内容
         :return:
         """
         self.sftp.chdir(os.path.dirname(file_path))
         with self.sftp.open(os.path.basename(file_path), mode) as f:
             f.write(content)
-        logging.info(f'write {file_path} content success')
+        logging.debug(f'write {file_path} content success')
 
     @enable_sftp
     def chmod(self, file_path: str, mode) -> None:
         """更改文件权限
 
         :param file_path:
         :param mode:
         :return:
         """
         self.sftp.chmod(file_path, mode)
-        logging.info(f'chmod {file_path} success')
+        logging.debug(f'chmod {file_path} success')
 
     @enable_sftp
     def mkdir(self, path, mode=511) -> None:
         """创建文件夹
 
         :param path: 路径
         :param mode:  511 即 o777 权限，最大的
         :return:
         """
         self.sftp.mkdir(path, mode)
-        logging.info(f'mkdir {path} success')
+        logging.debug(f'mkdir {path} success')
 
     @enable_sftp
     def rmdir(self, path) -> None:
         """删除文件夹
 
         :param path: 路径
         :return:
         """
         self.sftp.rmdir(path)
-        logging.info(f'remove {path} success')
+        logging.debug(f'remove {path} success')
 
     @enable_sftp
     def rename(self, old_path, new_path) -> None:
         """文件重命名
 
         :param old_path:
         :param new_path:
         :return:
         """
         self.sftp.rename(old_path, new_path)
-        logging.info(f'{old_path} rename success')
+        logging.debug(f'{old_path} rename success')
 
     def close(self) -> None:
         """断开连接
 
         :return:
         """
         self.ssh.close()
```

### Comparing `inhandtest-0.0.50/inhandtest/ip.py` & `inhandtest-0.0.51/inhandtest/ip.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/inhandtest/mail.py` & `inhandtest-0.0.51/inhandtest/mail.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     kill_windows_port(render.get('host'), [port, port + 1])  # port+1 是https端口
     # 启动本地服务，分享报告
     p = subprocess.Popen(f'npx anywhere -h {render.get("host")} -p {port}', cwd=render.get('allure_results_path'),
                          shell=True,
                          stdout=subprocess.PIPE, stderr=subprocess.STDOUT, encoding='gbk')
     while True:
         output = p.stdout.readline()
-        logging.info(output)
+        logging.debug(output)
         if len(re.findall(r'Running at (.*)/', output)) < 1:  # 无论是否启动成功，都会退出循环
             break
     # 读取报告中的summary.json文件，获取测试结果
     summary = json.load(
         open(os.path.join(render.get('allure_results_path'), 'widgets', 'summary.json'), 'r', encoding='utf-8'))
     html_file_path = os.path.join(os.path.dirname(__file__), 'pytest_email.html')
     from emails.template import JinjaTemplate as Te
@@ -138,15 +138,15 @@
                 if receiver_time > datetime.datetime.strptime(kwargs.get('after_date'), '%Y-%m-%d %H:%M:%S'):
                     continue
             subject_ = decode_str(email_message['Subject'])
             sender_from = decode_str(email_message['From'])
             if not ((subject in subject_) and (mail_from[0] in sender_from and mail_from[1] in sender_from)):
                 continue
             else:
-                logging.info(f'get email success! subject: {subject_}, sender: {sender_from}')
+                logging.debug(f'get email success! subject: {subject_}, sender: {sender_from}')
             # 解析邮件正文
             if not kwargs.get('body') and not kwargs.get('html_body'):
                 result = True
                 break
             else:
                 body = html_body = None
                 if email_message.is_multipart():
@@ -173,15 +173,15 @@
                             kwargs.get('body')]
                         for expect_ in expect_body:
                             if expect_ not in body:
                                 logging.warning(f'assert email body failed!')
                                 break
                         else:
                             result = True
-                            logging.info(f'assert email body success!')
+                            logging.debug(f'assert email body success!')
                         break  # 无论是否包含期望的邮件内容，都跳出循环
                 if kwargs.get('html_body'):
                     if not html_body:
                         break
                     else:
                         html_body = etree.HTML(html_body)
                         for xpath_, text_ in kwargs.get('html_body').items():
@@ -192,15 +192,15 @@
                                 logging.warning(f'assert email html_body failed!')
                                 break
                         else:
                             result = True
                             logging.warning(f'assert email html_body success!')
                         break
         else:
-            logging.info(f'not found {subject} email')
+            logging.debug(f'not found {subject} email')
     else:
         logging.error(f'get email failed: {status}')
     # 关闭 IMAP 连接
     imap_server.close()
     imap_server.logout()
     return result
 
@@ -210,15 +210,15 @@
     """邮箱删除收件箱
 
     :param receiver: 接收者('test@inhand.com.cn', '1111124') email, password
     :return:
     """
     imap_server = imaplib.IMAP4_SSL('imap.exmail.qq.com', 993)
     imap_server.login(receiver[0], receiver[1])
-    logging.info(f'login in email {receiver[0]}')
+    logging.debug(f'login in email {receiver[0]}')
     # 选择收件箱
     imap_server.select('inbox')
     # 检索所有邮件的ID
     status, data = imap_server.search(None, 'ALL')
     if status == 'OK':
         # 将每个邮件标记为删除
```

### Comparing `inhandtest-0.0.50/inhandtest/pages/ingateway/edge_computing/edge_computing.py` & `inhandtest-0.0.51/inhandtest/pages/ingateway/edge_computing/edge_computing.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 # @Time    : 2023/5/25 15:33:58
 # @Author  : Pane Li
 # @File    : edge_computing.py
 """
 edge_computing
 
 """
-from inhandtest.pages.ingateway.edge_computing.python_edge_computing import PythonEdgeComputing
+from inhandtest.pages.ingateway.edge_computing.python_edge_computing import PythonEdgeComputing, DockerManager
 
 
 class EdgeComputing:
 
     def __init__(self, host: str, username: str, password: str, protocol='https',
                  port=443, model='IG902', language='en', page=None, locale: dict = None):
         self.python_edge_computing: PythonEdgeComputing = PythonEdgeComputing(host, username, password, protocol, port,
                                                                               model, language, page, locale)
+        self.docker_manager: DockerManager = DockerManager(host, username, password, protocol, port, model, language,
+                                                           page, locale)
```

### Comparing `inhandtest-0.0.50/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py` & `inhandtest-0.0.51/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py`

 * *Files 25% similar despite different names*

```diff
@@ -52,15 +52,15 @@
                password: 123456 ex: password='123456'
                start_all_app: True, False ex: app_all_start=True
                stop_all_app: True, False ex: app_all_stop=True
                restart_all_app: True, False ex: restart_all_app=True
                app: [($action, **kwarg)] ex:
                     [('enable', 'device_supervisor', True)],   # 启用 device_supervisor
                     [('enable', 'device_supervisor', False)]   # 禁用 device_supervisor
-                    [('add', 'C:\\Users\\Administrator\\Downloads\\device_supervisor-1.0.0.tar.gz')] # 添加 device_supervisor
+                    [('install', {'app_package': 'C:\\Users\\Administrator\\Downloads\\device_supervisor-1.0.0.tar.gz'})] # 添加 device_supervisor
                     [('import_config', 'device_supervisor', 'C:\\Users\\Administrator\\Downloads\\device_supervisor-1.0.0.conf')] # 导入device_supervisor配置
                     [('export_config', 'device_supervisor', {'file_path': 'C:\\Users\\Administrator\\Downloads', 'file_name': "device_supervisor-1.0.0.conf"})] # 导出device_supervisor配置， 文件名可以不传
                     [('uninstall', 'device_supervisor')]   # 卸载 device_supervisor
                     [('edit', 'device_supervisor', {'log_file_size': 1, 'number_of_log': 2, 'start_args': ''})]   # 编辑 device_supervisor
                     [('download_log', 'device_supervisor', {'file_path': 'C:\\Users\\Administrator\\Downloads', 'file_name': "device_supervisor-1.0.0.log"})] # 导出device_supervisor日志， 文件名可以不传
                     [('clear_log', 'device_supervisor')]   # 清除 device_supervisor 日志
                     [('start', 'device_supervisor')]  # 启动 device_supervisor
@@ -70,26 +70,114 @@
                         log_file_size: int
                         number_of_log: int
                         start_args: str  启动参数
                         error_text: str or list
                         cancel: True, False
                submit: True,False ex: submit=True
                error_text: str ex: error_text='ip_address_conflict'
-               success_tip: True
+               success_tip: ‘APP start successful’
                reset: True, False ex: reset=True
         """
         self.access_menu('edge computing.python edge computing')
+        self.page.wait_for_load_state(state='networkidle')
+        self.page.wait_for_timeout(1 * 1000)
         if kwargs.get('sdk_upgrade'):
             kwargs.update(
                 {'sdk_upgrade_confirm': True, 'sdk_upgrade_tip': {'messages': 'install_success', 'timeout': 100}})
         if kwargs.get('password'):
             kwargs.update({'edit_password': True, 'submit_password': True})
         if kwargs.get('app'):
             app_list_action = []
             app_status_action = []
             for action in kwargs.pop('app'):
-                if action[0] in ('enable', 'add', 'import_config', 'export_config', 'uninstall', 'edit'):
+                if action[0] in ('enable', 'install', 'import_config', 'export_config', 'uninstall', 'edit'):
+                    app_list_action.append(action)
+                else:
+                    app_status_action.append(action)
+            kwargs.update({'app_list': app_list_action, 'app_status': app_status_action})
+        self.agg_in(self.edge_locators.python_edge_computing_locator, kwargs)
+
+
+class DockerManager(BasePage, IgLocators):
+
+    def __init__(self, host: str, username: str, password: str, protocol='https',
+                 port=443, model='IG902', language='en', page=None, locale: dict = None):
+        super().__init__(host, username, password, protocol, port, model, language, page, locale=locale)
+        IgLocators.__init__(self, page, locale)
+
+    @allure.step('断言Docker Manager状态')
+    @loop_inspector('docker_manager_status')
+    def assert_status(self, **kwargs):
+        """
+        :param kwargs:
+               docker_manager: enable,disable ex: docker_manager='"${value}"=="enable"'
+               docker_version: 1.4.3 ex: docker_version='1.4.3'
+               portainer_manager: enable,disable ex: portainer_manager='"${value}"=="enable"'
+               username: adm ex: username='adm'
+               password: 123456 ex: password='123456'
+               port:  9000 ex: port='9000'
+        """
+        self.access_menu('edge computing.docker manager')
+        return self.eval_locator_attribute(kwargs, self.edge_locators.docker_manager_status_locator)
+
+    @allure.step('获取Docker Manager状态')
+    def get_status(self, keys: str or list) -> str or dict or None:
+        """
+        :param keys:
+               docker_manager, docker_version, portainer_manager, username, password, port
+        """
+        self.access_menu('edge computing.docker manager')
+        self.page.wait_for_timeout(1000)
+        return self.get_text(keys, self.edge_locators.docker_manager_status_locator)
+
+    @allure.step('配置Docker Manager')
+    def config(self, **kwargs):
+        """
+        :param kwargs:
+               python_engine: enable,disable ex: python_engine='enable'
+               sdk_upgrade: file_path ex: sdk_upgrade='C:\\Users\\Administrator\\Downloads\\inhand-1.4.3.tar.gz'
+               password: 123456 ex: password='123456'
+               start_all_app: True, False ex: app_all_start=True
+               stop_all_app: True, False ex: app_all_stop=True
+               restart_all_app: True, False ex: restart_all_app=True
+               app: [($action, **kwarg)] ex:
+                    [('enable', 'device_supervisor', True)],   # 启用 device_supervisor
+                    [('enable', 'device_supervisor', False)]   # 禁用 device_supervisor
+                    [('install', {'app_package': 'C:\\Users\\Administrator\\Downloads\\device_supervisor-1.0.0.tar.gz'})] # 添加 device_supervisor
+                    [('import_config', 'device_supervisor', 'C:\\Users\\Administrator\\Downloads\\device_supervisor-1.0.0.conf')] # 导入device_supervisor配置
+                    [('export_config', 'device_supervisor', {'file_path': 'C:\\Users\\Administrator\\Downloads', 'file_name': "device_supervisor-1.0.0.conf"})] # 导出device_supervisor配置， 文件名可以不传
+                    [('uninstall', 'device_supervisor')]   # 卸载 device_supervisor
+                    [('edit', 'device_supervisor', {'log_file_size': 1, 'number_of_log': 2, 'start_args': ''})]   # 编辑 device_supervisor
+                    [('download_log', 'device_supervisor', {'file_path': 'C:\\Users\\Administrator\\Downloads', 'file_name': "device_supervisor-1.0.0.log"})] # 导出device_supervisor日志， 文件名可以不传
+                    [('clear_log', 'device_supervisor')]   # 清除 device_supervisor 日志
+                    [('start', 'device_supervisor')]  # 启动 device_supervisor
+                    [('stop', 'device_supervisor')]   # 停止 device_supervisor
+                    [('restart', 'device_supervisor')]   # 重启 device_supervisor
+                    edit parameters:
+                        log_file_size: int
+                        number_of_log: int
+                        start_args: str  启动参数
+                        error_text: str or list
+                        cancel: True, False
+               submit: True,False ex: submit=True
+               error_text: str ex: error_text='ip_address_conflict'
+               success_tip: ‘APP start successful’
+               reset: True, False ex: reset=True
+        """
+        self.access_menu('edge computing.python edge computing')
+        self.page.wait_for_load_state(state='networkidle')
+        self.page.wait_for_timeout(1 * 1000)
+        if kwargs.get('sdk_upgrade'):
+            kwargs.update(
+                {'sdk_upgrade_confirm': True, 'sdk_upgrade_tip': {'messages': 'install_success', 'timeout': 100}})
+        if kwargs.get('password'):
+            kwargs.update({'edit_password': True, 'submit_password': True})
+        if kwargs.get('app'):
+            app_list_action = []
+            app_status_action = []
+            for action in kwargs.pop('app'):
+                if action[0] in ('enable', 'install', 'import_config', 'export_config', 'uninstall', 'edit'):
                     app_list_action.append(action)
                 else:
                     app_status_action.append(action)
             kwargs.update({'app_list': app_list_action, 'app_status': app_status_action})
         self.agg_in(self.edge_locators.python_edge_computing_locator, kwargs)
```

### Comparing `inhandtest-0.0.50/inhandtest/pages/ingateway/edge_computing/python_edge_computing_locators.py` & `inhandtest-0.0.51/inhandtest/pages/ingateway/network/ethernet_locators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,84 +1,86 @@
 # -*- coding: utf-8 -*-
-# @Time    : 2023/5/25 15:33:14
+# @Time    : 2023/5/17 11:54:34
 # @Author  : Pane Li
-# @File    : python_edge_computing_locators.py
+# @File    : ethernet_locators.py
 """
-python_edge_computing_locators
+ethernet_locators
 
 """
+
 from playwright.sync_api import Page
 
 
-class PythonEdgeComputingLocators:
+class EthernetLocators:
     def __init__(self, page: Page, locale: dict):
         self.page = page
         self.locale = locale
         self.pop_up = self.page.locator('.ant-modal-content')
 
     @property
-    def python_engine_status_locator(self) -> list:
+    def ethernet_status_locators(self) -> list:
         return [
-            ('python_engine', {'locator': self.page.locator('//button').nth(0), 'type': 'switch_button'}),
-            ('sdk_version',
-             {'locator': self.page.locator('//span', has_text=self.locale.sdk_version).locator('../span[2]').nth(0),
-              'type': 'text'}),
-            ('python_version',
-             {'locator': self.page.locator('//span', has_text=self.locale.python_version).locator('../span[2]').nth(0),
-              'type': 'text'}),
-            ('username',
-             {'locator': self.page.locator('//span', has_text=self.locale.username).locator('../span[2]').nth(0),
-              'type': 'text'}),
-            ('used_user_storage',
-             {'locator': self.page.locator('//span', has_text=self.locale.used_user_storage).locator('../div').nth(0),
-              'type': 'text'}),
-            ('password', {'locator': self.page.locator('.anticon.anticon-copy'), 'type': 'clipboard'}),
+            ('network_type', {'locator': self.page.locator(
+                f'//div[./div[@class="antd-pro-components-description-list-index-term"][text()="{self.locale.network_type}"]]/div[2]'),
+                'type': 'text', 'param': {'static_ip': self.locale.static_ip,
+                                          'dynamic_address_dhcp': self.locale.dynamic_address_dhcp}}),
+            ('ip_address', {'locator': self.page.locator(
+                f'//div[./div[@class="antd-pro-components-description-list-index-term"][text()="{self.locale.ip_address}"]]/div[2]'),
+                'type': 'text'}),
+            ('netmask', {'locator': self.page.locator(
+                f'//div[./div[@class="antd-pro-components-description-list-index-term"][text()="{self.locale.netmask}"]]/div[2]'),
+                'type': 'text'}),
+            ('gateway', {'locator': self.page.locator(
+                f'//div[./div[@class="antd-pro-components-description-list-index-term"][text()="{self.locale.gateway}"]]/div[2]'),
+                'type': 'text'}),
+            ('dns', {'locator': self.page.locator(
+                f'//div[./div[@class="antd-pro-components-description-list-index-term"][text()="{self.locale.dns}"]]/div[2]'),
+                'type': 'text'}),
+            ('mtu', {'locator': self.page.locator(
+                f'//div[./div[@class="antd-pro-components-description-list-index-term"][text()="{self.locale.mtu}"]]/div[2]'),
+                'type': 'text'}),
+            ('status', {'locator': self.page.locator(
+                f'//div[./div[@class="antd-pro-components-description-list-index-term"][text()="{self.locale.status}"]]/div[2]'),
+                'type': 'text', 'param': {'up': 'Up', 'down': 'Down'}}),
+            ('connection_time', {'locator': self.page.locator(
+                f'//div[./div[@class="antd-pro-components-description-list-index-term"][text()="{self.locale.connection_time}"]]/div[2]'),
+                'type': 'text', 'param': {'day': self.locale.day}}),
+            ('description', {'locator': self.page.locator(
+                f'//div[./div[@class="antd-pro-components-description-list-index-term"][text()="{self.locale.description}"]]/div[2]'),
+                'type': 'text'}),
         ]
 
     @property
-    def python_edge_computing_locator(self) -> list:
+    def ethernet_locators(self) -> list:
         return [
-            ('python_engine', {'locator': self.page.locator('//button').nth(0), 'type': 'switch_button'}),
-            ('sdk_upgrade', {'locator': self.page.locator('//button').nth(1), 'type': 'upload_file',
-                             'relation': [('python_engine', 'enable')]}),
-            ('sdk_upgrade_confirm',
-             {'locator': self.pop_up.locator('.ant-btn.ant-btn-primary').nth(0), 'type': 'button'}),
-            ('sdk_upgrade_tip', {'type': 'tip_messages'}),
-            ('edit_password', {'locator': self.page.locator('.anticon.anticon-form').nth(0), 'type': 'button',
-                               'relation': [('python_engine', 'enable')]}),
-            ('password',
-             {'locator': self.page.locator('.ant-input'), 'type': 'text', 'relation': [('python_engine', 'enable')]}),
-            ('submit_password', {'locator': self.page.locator('.anticon.anticon-check').nth(1), 'type': 'button'}),
-            ('start_all_app', {'locator': self.page.locator('.anticon.anticon-play-circle').nth(0),
-                               'type': 'button', 'relation': [('python_engine', 'enable')]}),
-            ('stop_all_app', {'locator': self.page.locator('.anticon.anticon-pause-circle').nth(0),
-                              'type': 'button', 'relation': [('python_engine', 'enable')]}),
-            ('restart_all_app', {'locator': self.page.locator('.anticon.anticon-undo').nth(0),
-                                 'type': 'button', 'relation': [('python_engine', 'enable')]}),
-            ('app_list',
-             {'locator': {
-                 'locator': self.page.locator('.antd-pro-components-in-gateway-editable-table-index-outerBox').nth(0)},
-                 "columns": [
-                     ('app_package',
-                      {'locator': self.pop_up.locator('.anticon.anticon-upload'), 'type': 'upload_file'}),
-                     ('log_file_size', {'locator': self.pop_up.locator('#log_size'), 'type': 'text'}),
-                     ('number_of_log', {'locator': self.pop_up.locator('#log_file_num'), 'type': 'text'}),
-                     ('start_args', {'locator': self.pop_up.locator('#start_args'), 'type': 'text'}),
-                     ('errors_text', {'type': 'text_messages'}),
-                     ('success_tip', {'type': 'tip_messages'}),
-                     ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'),
-                                 'type': 'button'}),
-                     ('save', {'locator': self.pop_up.locator(
-                         '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'})],
-                 'type': 'table_tr', 'relation': [('python_engine', 'enable')]}),
-            ('app_status',
-             {'locator': {
-                 'locator': self.page.locator(
-                     '.ant-table.ant-table-default.ant-table-bordered.ant-table-scroll-position-left').nth(0)},
-                 'type': 'table_tr', 'relation': [('python_engine', 'enable')]}),
+            ('network_type', {'locator': self.page.locator('#internet'), 'type': 'select',
+                              'param': {'static_ip': self.locale.static_ip,
+                                        'dynamic_address_dhcp': self.locale.dynamic_address_dhcp}}),
+            ('ip_address', {'locator': self.page.locator('#primary_ip'), 'type': 'text'}),
+            ('netmask', {'locator': self.page.locator('#netmask'), 'type': 'text'}),
+            ('speed_duplex', {'locator': self.page.locator('#speed_duplex'), 'type': 'select',
+                              'param': {'auto_negotiation': self.locale.auto_negotiation, 'full': self.locale.full,
+                                        'half': self.locale.half, 'duplex': self.locale.duplex, 'm': 'M'}}),
+            ('mtu', {'locator': self.page.locator('#mtu'), 'type': 'text'}),
+            ('track_l2_state', {'locator': self.page.locator('#track_l2_state'), 'type': 'switch_button'}),
+            ('shutdown', {'locator': self.page.locator('#shutdown'), 'type': 'switch_button'}),
+            ('description', {'locator': self.page.locator('#description'), 'type': 'text'}),
+            ('secondary_ip_settings', {'locator': {
+                "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table1-index-outerBox'),
+                "columns": [
+                    ('secondary_ip', {'locator': self.pop_up.locator('#secondary_ip'), 'type': 'text'}),
+                    ('netmask',
+                     {'locator': self.pop_up.locator('#netmask'), 'type': 'text'}),
+                    ('errors_text', {'type': 'text_messages'}),
+                    ('cancel',
+                     {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
+                      'type': 'button'}),
+                    ('save',
+                     {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
+                ]}, 'type': 'table_tr'}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
             ('errors_text', {'type': 'text_messages'}),
             ('success_tip', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
                        'type': 'button'}),
```

### Comparing `inhandtest-0.0.50/inhandtest/pages/ingateway/locale.yml` & `inhandtest-0.0.51/inhandtest/pages/ingateway/locale.yml`

 * *Files 2% similar despite different names*

```diff
@@ -74,17 +74,19 @@
   inside: Inside
   outside: Outside
   'yes': Yes
   'no': No
   sdk_version: SDK Version
   python_version: Python Version
   username: Username
+  user_name: User Name
   used_user_storage: Used User Storage
   password: Password
   install_success: Install success
+  docker_version: Docker Version
 cn:
   client: 客户端
   server: 服务器
   ap: 接入端
   connect: 已连接
   disconnect: 未连接
   enable: 启用
@@ -157,10 +159,12 @@
   inside: 内部
   outside: 外部
   'yes': 是
   'no': 否
   sdk_version: SDK版本
   python_version: Python解释器
   username: 用户名
+  user_name: 用户名
   used_user_storage: 用户存储空间
   password: 密码
   install_success: 安装成功
+  docker_version: Docker版本
```

### Comparing `inhandtest-0.0.50/inhandtest/pages/ingateway/locators.py` & `inhandtest-0.0.51/inhandtest/pages/ingateway/locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/inhandtest/pages/ingateway/network/acl_locators.py` & `inhandtest-0.0.51/inhandtest/pages/ingateway/network/acl_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/inhandtest/pages/ingateway/network/bridge_locators.py` & `inhandtest-0.0.51/inhandtest/pages/ingateway/network/bridge_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/inhandtest/pages/ingateway/network/cellular_locators.py` & `inhandtest-0.0.51/inhandtest/pages/ingateway/network/cellular_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/inhandtest/pages/ingateway/network/dhcp_locators.py` & `inhandtest-0.0.51/inhandtest/pages/ingateway/network/dhcp_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/inhandtest/pages/ingateway/network/dns_locators.py` & `inhandtest-0.0.51/inhandtest/pages/ingateway/network/dns_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/inhandtest/pages/ingateway/network/ethernet_locators.py` & `inhandtest-0.0.51/inhandtest/pages/ingateway/network/wan_locators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 # -*- coding: utf-8 -*-
-# @Time    : 2023/5/17 11:54:34
+# @Time    : 2023/5/19 15:47:12
 # @Author  : Pane Li
-# @File    : ethernet_locators.py
+# @File    : wan_locators.py
 """
-ethernet_locators
+wan_locators
 
 """
-
 from playwright.sync_api import Page
 
 
-class EthernetLocators:
+class WanLocators:
     def __init__(self, page: Page, locale: dict):
         self.page = page
         self.locale = locale
-        self.pop_up = self.page.locator('.ant-modal-content')
 
     @property
-    def ethernet_status_locators(self) -> list:
+    def wan_status_locators(self) -> list:
         return [
             ('network_type', {'locator': self.page.locator(
                 f'//div[./div[@class="antd-pro-components-description-list-index-term"][text()="{self.locale.network_type}"]]/div[2]'),
                 'type': 'text', 'param': {'static_ip': self.locale.static_ip,
                                           'dynamic_address_dhcp': self.locale.dynamic_address_dhcp}}),
             ('ip_address', {'locator': self.page.locator(
                 f'//div[./div[@class="antd-pro-components-description-list-index-term"][text()="{self.locale.ip_address}"]]/div[2]'),
@@ -29,57 +27,58 @@
             ('netmask', {'locator': self.page.locator(
                 f'//div[./div[@class="antd-pro-components-description-list-index-term"][text()="{self.locale.netmask}"]]/div[2]'),
                 'type': 'text'}),
             ('gateway', {'locator': self.page.locator(
                 f'//div[./div[@class="antd-pro-components-description-list-index-term"][text()="{self.locale.gateway}"]]/div[2]'),
                 'type': 'text'}),
             ('dns', {'locator': self.page.locator(
-                f'//div[./div[@class="antd-pro-components-description-list-index-term"][text()="{self.locale.dns}"]]/div[2]'),
+                f'//div[./div[@class="antd-pro-components-description-list-index-term"][text()="DNS"]]/div[2]'),
                 'type': 'text'}),
             ('mtu', {'locator': self.page.locator(
                 f'//div[./div[@class="antd-pro-components-description-list-index-term"][text()="{self.locale.mtu}"]]/div[2]'),
-                'type': 'text'}),
+                'type': 'text', }),
             ('status', {'locator': self.page.locator(
                 f'//div[./div[@class="antd-pro-components-description-list-index-term"][text()="{self.locale.status}"]]/div[2]'),
                 'type': 'text', 'param': {'up': 'Up', 'down': 'Down'}}),
-            ('connection_time', {'locator': self.page.locator(
-                f'//div[./div[@class="antd-pro-components-description-list-index-term"][text()="{self.locale.connection_time}"]]/div[2]'),
-                'type': 'text', 'param': {'day': self.locale.day}}),
             ('description', {'locator': self.page.locator(
                 f'//div[./div[@class="antd-pro-components-description-list-index-term"][text()="{self.locale.description}"]]/div[2]'),
                 'type': 'text'}),
+            ('connection_time', {'locator': self.page.locator(
+                f'//div[./div[@class="antd-pro-components-description-list-index-term"][text()="{self.locale.connection_time}"]]/div[2]'),
+                'type': 'text', 'param': {'day': self.locale.day}}),
         ]
 
     @property
-    def ethernet_locators(self) -> list:
+    def wan_locators(self) -> list:
         return [
+            ('interface_type', {'locator': self.page.locator('#internetType'), 'type': 'radio_select'}),
             ('network_type', {'locator': self.page.locator('#internet'), 'type': 'select',
                               'param': {'static_ip': self.locale.static_ip,
                                         'dynamic_address_dhcp': self.locale.dynamic_address_dhcp}}),
             ('ip_address', {'locator': self.page.locator('#primary_ip'), 'type': 'text'}),
             ('netmask', {'locator': self.page.locator('#netmask'), 'type': 'text'}),
-            ('speed_duplex', {'locator': self.page.locator('#speed_duplex'), 'type': 'select',
-                              'param': {'auto_negotiation': self.locale.auto_negotiation, 'full': self.locale.full,
-                                        'half': self.locale.half, 'duplex': self.locale.duplex, 'm': 'M'}}),
+            ('gateway', {'locator': self.page.locator('#gateway'), 'type': 'text'}),
+            ('dns', {'locator': self.page.locator('#primary_dns'), 'type': 'text'}),
             ('mtu', {'locator': self.page.locator('#mtu'), 'type': 'text'}),
             ('track_l2_state', {'locator': self.page.locator('#track_l2_state'), 'type': 'switch_button'}),
             ('shutdown', {'locator': self.page.locator('#shutdown'), 'type': 'switch_button'}),
             ('description', {'locator': self.page.locator('#description'), 'type': 'text'}),
             ('secondary_ip_settings', {'locator': {
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table1-index-outerBox'),
                 "columns": [
-                    ('secondary_ip', {'locator': self.pop_up.locator('#secondary_ip'), 'type': 'text'}),
+                    ('secondary_ip', {'locator': self.page.locator('#secondary_ip'), 'type': 'text'}),
                     ('netmask',
-                     {'locator': self.pop_up.locator('#netmask'), 'type': 'text'}),
+                     {'locator': self.page.locator('.ant-modal-content').locator('#netmask'), 'type': 'text'}),
                     ('errors_text', {'type': 'text_messages'}),
                     ('cancel',
                      {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
                       'type': 'button'}),
                     ('save',
-                     {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
+                     {'locator': self.page.locator('.ant-modal-content').locator(
+                         '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
                 ]}, 'type': 'table_tr'}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
             ('errors_text', {'type': 'text_messages'}),
             ('success_tip', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
```

### Comparing `inhandtest-0.0.50/inhandtest/pages/ingateway/network/firewall.py` & `inhandtest-0.0.51/inhandtest/pages/ingateway/network/firewall.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/inhandtest/pages/ingateway/network/gps_locators.py` & `inhandtest-0.0.51/inhandtest/pages/ingateway/network/gps_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/inhandtest/pages/ingateway/network/l2tp_locators.py` & `inhandtest-0.0.51/inhandtest/pages/ingateway/network/l2tp_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/inhandtest/pages/ingateway/network/lan_locators.py` & `inhandtest-0.0.51/inhandtest/pages/ingateway/network/lan_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/inhandtest/pages/ingateway/network/loopback_locators.py` & `inhandtest-0.0.51/inhandtest/pages/ingateway/network/loopback_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/inhandtest/pages/ingateway/network/nat_locators.py` & `inhandtest-0.0.51/inhandtest/pages/ingateway/network/nat_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/inhandtest/pages/ingateway/network/network.py` & `inhandtest-0.0.51/inhandtest/pages/ingateway/network/network.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/inhandtest/pages/ingateway/network/network_interface.py` & `inhandtest-0.0.51/inhandtest/pages/ingateway/network/network_interface.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/inhandtest/pages/ingateway/network/network_locators.py` & `inhandtest-0.0.51/inhandtest/pages/ingateway/network/network_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/inhandtest/pages/ingateway/network/network_services.py` & `inhandtest-0.0.51/inhandtest/pages/ingateway/network/network_services.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/inhandtest/pages/ingateway/network/routing.py` & `inhandtest-0.0.51/inhandtest/pages/ingateway/network/routing.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/inhandtest/pages/ingateway/network/routing_status_locators.py` & `inhandtest-0.0.51/inhandtest/pages/ingateway/network/routing_status_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/inhandtest/pages/ingateway/network/static_routing_locators.py` & `inhandtest-0.0.51/inhandtest/pages/ingateway/network/static_routing_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/inhandtest/pages/ingateway/network/vpn.py` & `inhandtest-0.0.51/inhandtest/pages/ingateway/network/vpn.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/inhandtest/pages/ingateway/network/wan_locators.py` & `inhandtest-0.0.51/inhandtest/pages/ingateway/edge_computing/docker_manager_locators.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,85 +1,99 @@
 # -*- coding: utf-8 -*-
-# @Time    : 2023/5/19 15:47:12
+# @Time    : 2023/6/1 10:28:48
 # @Author  : Pane Li
-# @File    : wan_locators.py
+# @File    : docker_manager_locators.py
 """
-wan_locators
+docker_manager_locators
 
 """
 from playwright.sync_api import Page
 
 
-class WanLocators:
+class DockerManagerLocators:
     def __init__(self, page: Page, locale: dict):
         self.page = page
         self.locale = locale
+        self.pop_up = self.page.locator('.ant-modal-content')
 
     @property
-    def wan_status_locators(self) -> list:
+    def docker_manager_status_locator(self) -> list:
         return [
-            ('network_type', {'locator': self.page.locator(
-                f'//div[./div[@class="antd-pro-components-description-list-index-term"][text()="{self.locale.network_type}"]]/div[2]'),
-                'type': 'text', 'param': {'static_ip': self.locale.static_ip,
-                                          'dynamic_address_dhcp': self.locale.dynamic_address_dhcp}}),
-            ('ip_address', {'locator': self.page.locator(
-                f'//div[./div[@class="antd-pro-components-description-list-index-term"][text()="{self.locale.ip_address}"]]/div[2]'),
-                'type': 'text'}),
-            ('netmask', {'locator': self.page.locator(
-                f'//div[./div[@class="antd-pro-components-description-list-index-term"][text()="{self.locale.netmask}"]]/div[2]'),
-                'type': 'text'}),
-            ('gateway', {'locator': self.page.locator(
-                f'//div[./div[@class="antd-pro-components-description-list-index-term"][text()="{self.locale.gateway}"]]/div[2]'),
-                'type': 'text'}),
-            ('dns', {'locator': self.page.locator(
-                f'//div[./div[@class="antd-pro-components-description-list-index-term"][text()="DNS"]]/div[2]'),
-                'type': 'text'}),
-            ('mtu', {'locator': self.page.locator(
-                f'//div[./div[@class="antd-pro-components-description-list-index-term"][text()="{self.locale.mtu}"]]/div[2]'),
-                'type': 'text', }),
-            ('status', {'locator': self.page.locator(
-                f'//div[./div[@class="antd-pro-components-description-list-index-term"][text()="{self.locale.status}"]]/div[2]'),
-                'type': 'text', 'param': {'up': 'Up', 'down': 'Down'}}),
-            ('description', {'locator': self.page.locator(
-                f'//div[./div[@class="antd-pro-components-description-list-index-term"][text()="{self.locale.description}"]]/div[2]'),
-                'type': 'text'}),
-            ('connection_time', {'locator': self.page.locator(
-                f'//div[./div[@class="antd-pro-components-description-list-index-term"][text()="{self.locale.connection_time}"]]/div[2]'),
-                'type': 'text', 'param': {'day': self.locale.day}}),
+            ('docker_manager', {'locator': self.page.locator('#enable').nth(0), 'type': 'switch_button'}),
+            ('docker_version',
+             {'locator': self.page.locator('//label', has_text=self.locale.docker_version).locator(
+                 '../../div[2]/div/span/div/span[1]'),
+                 'type': 'text'}),
+            ('portainer_manager', {'locator': self.page.locator('#enable').nth(0), 'type': 'switch_button'}),
+            ('username',
+             {'locator': self.page.locator('//label', has_text=self.locale.user_name).locator('../../div[2]').nth(0),
+              'type': 'text'}),
+            ('password', {'locator': self.page.locator('#password'), 'type': 'fill'}),
+            ('port', {'locator': self.page.locator('#port'), 'type': 'fill'}),
         ]
 
     @property
-    def wan_locators(self) -> list:
+    def docker_manager_locator(self) -> list:
         return [
-            ('interface_type', {'locator': self.page.locator('#internetType'), 'type': 'radio_select'}),
-            ('network_type', {'locator': self.page.locator('#internet'), 'type': 'select',
-                              'param': {'static_ip': self.locale.static_ip,
-                                        'dynamic_address_dhcp': self.locale.dynamic_address_dhcp}}),
-            ('ip_address', {'locator': self.page.locator('#primary_ip'), 'type': 'text'}),
-            ('netmask', {'locator': self.page.locator('#netmask'), 'type': 'text'}),
-            ('gateway', {'locator': self.page.locator('#gateway'), 'type': 'text'}),
-            ('dns', {'locator': self.page.locator('#primary_dns'), 'type': 'text'}),
-            ('mtu', {'locator': self.page.locator('#mtu'), 'type': 'text'}),
-            ('track_l2_state', {'locator': self.page.locator('#track_l2_state'), 'type': 'switch_button'}),
-            ('shutdown', {'locator': self.page.locator('#shutdown'), 'type': 'switch_button'}),
-            ('description', {'locator': self.page.locator('#description'), 'type': 'text'}),
-            ('secondary_ip_settings', {'locator': {
-                "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table1-index-outerBox'),
-                "columns": [
-                    ('secondary_ip', {'locator': self.page.locator('#secondary_ip'), 'type': 'text'}),
-                    ('netmask',
-                     {'locator': self.page.locator('.ant-modal-content').locator('#netmask'), 'type': 'text'}),
-                    ('errors_text', {'type': 'text_messages'}),
-                    ('cancel',
-                     {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
-                      'type': 'button'}),
-                    ('save',
-                     {'locator': self.page.locator('.ant-modal-content').locator(
-                         '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
-                ]}, 'type': 'table_tr'}),
+
+            ('docker_upgrade', {'locator': self.page.locator('.anticon.anticon-upload'), 'type': 'upload_file'}),
+            ('docker_upgrade_confirm',
+             {'locator': self.pop_up.locator('.ant-btn.ant-btn-primary').nth(0), 'type': 'button',
+              'wait_for': [{'type': 'hidden', 'locator': self.pop_up, 'timeout': 300 * 1000},
+                           {'type': 'timeout', 'timeout': 3 * 1000}]}),
+            ('python_engine', {'locator': self.page.locator('//button').nth(0), 'type': 'switch_button'}),
+            ('sdk_upgrade_confirm',
+             {'locator': self.pop_up.locator('.ant-btn.ant-btn-primary').nth(0), 'type': 'button'}),
+            ('sdk_upgrade_tip', {'type': 'tip_messages'}),
+            ('edit_password', {'locator': self.page.locator('.anticon.anticon-form').nth(0), 'type': 'button',
+                               'relation': [('python_engine', 'enable')]}),
+            ('password',
+             {'locator': self.page.locator('.ant-input'), 'type': 'text', 'relation': [('python_engine', 'enable')]}),
+            ('submit_password', {'locator': self.page.locator('.anticon.anticon-check').nth(1), 'type': 'button'}),
+            ('start_all_app', {'locator': [self.page.locator('.anticon.anticon-play-circle').nth(0),
+                                           self.page.locator('.ant-popover-inner-content').locator(
+                                               '.ant-btn.ant-btn-primary.ant-btn-sm').first],
+                               'type': 'button', 'relation': [('python_engine', 'enable')]}),
+            ('stop_all_app', {'locator': [self.page.locator('.anticon.anticon-pause-circle').nth(0),
+                                          self.page.locator('.ant-popover-inner-content').locator(
+                                              '.ant-btn.ant-btn-primary.ant-btn-sm').first],
+                              'type': 'button', 'relation': [('python_engine', 'enable')]}),
+            ('restart_all_app', {'locator': [self.page.locator('.anticon.anticon-undo').nth(0),
+                                             self.page.locator('.ant-popover-inner-content').locator(
+                                                 '.ant-btn.ant-btn-primary.ant-btn-sm').first],
+                                 'type': 'button', 'relation': [('python_engine', 'enable')]}),
+            ('app_list',
+             {'locator': {
+                 'locator': self.page.locator('.antd-pro-components-in-gateway-editable-table-index-outerBox').nth(0),
+                 'pop_up_locator': self.pop_up,
+                 'action_confirm': self.page.locator('.ant-popover-inner-content').locator(
+                     '.ant-btn.ant-btn-primary.ant-btn-sm').first,
+                 "columns": [
+                     ('app_package',
+                      {'locator': self.pop_up.locator('.anticon.anticon-upload'), 'type': 'upload_file'}),
+                     ('log_file_size', {'locator': self.pop_up.locator('#log_size'), 'type': 'text'}),
+                     ('number_of_log', {'locator': self.pop_up.locator('#log_file_num'), 'type': 'text'}),
+                     ('start_args', {'locator': self.pop_up.locator('#start_args'), 'type': 'text'}),
+                     ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'),
+                                 'type': 'button'}),
+                     ('save', {'locator': self.pop_up.locator(
+                         '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button',
+                         'wait_for': {'type': 'hidden', 'locator': self.pop_up, 'timeout': 300 * 1000}}),
+                     ('errors_text', {'type': 'text_messages'}),
+                     ('success_tip', {'type': 'tip_messages'}),
+                 ]},
+                 'type': 'table_tr', 'relation': [('python_engine', 'enable')]}),
+            ('app_status',
+             {'locator': {
+                 'locator': self.page.locator(
+                     '.ant-table.ant-table-default.ant-table-bordered.ant-table-scroll-position-left').nth(0),
+                 'action_confirm': self.page.locator('.ant-popover-inner-content').locator(
+                     '.ant-btn.ant-btn-primary.ant-btn-sm').first,
+             },
+                 'type': 'table_tr', 'relation': [('python_engine', 'enable')]}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
             ('errors_text', {'type': 'text_messages'}),
             ('success_tip', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
                        'type': 'button'}),
```

### Comparing `inhandtest-0.0.50/inhandtest/pages/ingateway/network/wlan_locators.py` & `inhandtest-0.0.51/inhandtest/pages/ingateway/network/wlan_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/inhandtest/pages/ingateway/overview/overview.py` & `inhandtest-0.0.51/inhandtest/pages/ingateway/overview/overview.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/inhandtest/pages/ingateway/overview/overview_locators.py` & `inhandtest-0.0.51/inhandtest/pages/ingateway/overview/overview_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/inhandtest/pytest_email.html` & `inhandtest-0.0.51/inhandtest/pytest_email.html`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.50/inhandtest/telnet.py` & `inhandtest-0.0.51/inhandtest/telnet.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 class Telnet:
     __doc__ = '使用telnet连接设备，封装下面命令'
 
     def __init__(self, model: str, host: str, super_user: str, super_password: str, user='adm', password='123456',
                  port=23, **kwargs):
         """使用telnet连接设备
 
-        :param model: 设备型号，VG710'|'IR302'|'ER805'|'ER605'|'IG902'|'IG502'|'IR915'
+        :param model: 设备型号，VG710'|'IR302'|'ER805'|'ER605'|'IG902'|'IG502'|'IR915'|'ODU2002'
         :param host: 设备lan ip， 192.168.2.1
         :param super_user: 超级管理员的用户名称
         :param super_password:  超级管理员的密码
         :param user: 用户名
         :param password: 用户密码
         :param port: 端口
         :param kwargs: interface_replace, 字典类型，只替换输入命令 {'wan': 'wan0', 'wifi_sta': 'wan2', 'cellular1': 'wwan0'}
@@ -41,21 +41,21 @@
         self.super_password = super_password
         self.user = user
         self.password = password
         self.port = port
         self.host_name = ''
         self.super_tag = '/www #'
         self.config_tag = '(config)#'
-        self.user_tag = '#'
+        self.user_tag = '#'    # 特权模式
         self.normal_tag = '>'
         self.factory_tag = '(factory)#'  # 仅部分设备支持工厂模式
         self.factory_username = kwargs.get('factory_username')
         self.factory_password = kwargs.get('factory_password')
         self.interface_replace: dict = kwargs.get('interface_replace')
-        if self.model not in ['VG710', 'IR302', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915']:
+        if self.model not in ['VG710', 'IR302', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915', 'ODU2002']:
             raise Exception(f'Not support this device model {self.model}')
         self.tn: telnetlib.Telnet
         self.__login()
 
     def update_hostname(self, hostname: str) -> None:
         """更新hostname 后对应的telnet也需要更新
 
@@ -68,30 +68,31 @@
 
     def __login(self):
         """
 
 
         :return:
         """
-        login_spe = {"VG710": '#', 'IR302': '>', 'ER805': '#', 'ER605': '#', 'IG902': '#', 'IG502': '#', 'IR915': '#'}
+        login_spe = {"VG710": '#', 'IR302': '>', 'ER805': '#', 'ER605': '#', 'IG902': '#', 'IG502': '#', 'IR915': '#',
+                     'ODU2002': '>'}
         try:
             # 连接telnet服务器
-            logging.info("Start telnet 【%s:%s】" % (self.host, self.port))
+            logging.debug("Start telnet 【%s:%s】" % (self.host, self.port))
             self.tn = telnetlib.Telnet(self.host, self.port, timeout=10)
         except:
             raise ConnectionError(f'Device【{self.host}:{self.port} connect failed】')
-        logging.info("Telnet 【%s:%s】 connected" % (self.host, self.port))
+        logging.debug("Telnet 【%s:%s】 connected" % (self.host, self.port))
         self.tn.write("\n".encode("cp936"))
-        logging.info(self.tn.read_until('login:'.encode("cp936")).decode("cp936").strip())
+        logging.debug(self.tn.read_until('login:'.encode("cp936")).decode("cp936").strip())
         # 登录路由器
         self.tn.write("{}\n".format(self.user).encode("cp936"))
-        logging.info(self.tn.read_until('Password:'.encode("cp936")).decode("cp936").strip())
+        logging.debug(self.tn.read_until('Password:'.encode("cp936")).decode("cp936").strip())
         self.tn.write("{}\n".format(self.password).encode("cp936"))
         login_result = self.tn.read_until(login_spe.get(self.model).encode("cp936"), timeout=20).decode("cp936").strip()
-        logging.info(login_result)
+        logging.debug(login_result)
         if 'Login incorrect' in login_result:
             raise Exception('UsernameOrPasswordError')
         self.update_hostname(login_result.split('\r\n')[-1].split(' ')[-1][:-1])
         logging.info(f"Device {self.host} login success. user_tag: {self.user_tag}")
         return self
 
     def __enter__(self):
@@ -122,34 +123,34 @@
         """进入路由器的超级模式
 
         @return:
         """
         self.tn.write(("\003" + "\r").encode("cp936"))
         time.sleep(1)
         read_contents = self.tn.read_very_eager().decode('cp936').strip()
-        logging.info(read_contents)
+        logging.debug(read_contents)
         if self.config_tag in read_contents:
-            if self.model in ['VG710', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915']:
+            if self.model in ['VG710', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915', 'ODU2002']:
                 self.send_cli(["exit", self.super_user + " " + self.super_password])
             elif self.model == 'IR302':
                 self.send_cli(["exit", "exit", "support enable", self.super_user, self.super_password])
         elif self.super_tag in read_contents or (('/' in read_contents) and (' #' in read_contents)):
             self.send_cli(['cd /www'])
         elif self.user_tag in read_contents:
-            if self.model in ['VG710', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915']:
+            if self.model in ['VG710', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915', 'ODU2002']:
                 self.send_cli([self.super_user + " " + self.super_password])
             elif self.model == 'IR302':
                 self.send_cli(["exit", "support enable", self.super_user, self.super_password])
         elif self.normal_tag in read_contents:
-            if self.model in ['VG710', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915']:
+            if self.model in ['VG710', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915', 'ODU2002']:
                 self.send_cli(["enable", self.password, self.super_user + ' ' + self.super_password])
             elif self.model == 'IR302':
                 self.send_cli(["support enable", self.super_user, self.super_password])
         elif self.factory_tag in read_contents:
-            if self.model in ['VG710', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915']:
+            if self.model in ['VG710', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915', 'ODU2002']:
                 self.send_cli(["exit", self.super_user + " " + self.super_password])
             elif self.model == 'IR302':
                 self.send_cli(["exit", "exit", "support enable", self.super_user, self.super_password])
         else:
             logging.warning(f'not support this mode. telnet return contents: {read_contents}')
             self.close()
             self.__login()
@@ -161,30 +162,32 @@
         """配置模式
 
         :return:
         """
         self.tn.write(("\003" + "\r").encode("cp936"))
         time.sleep(1)
         read_contents = self.tn.read_very_eager().decode('cp936').strip()
-        logging.info(read_contents)
+        logging.debug(read_contents)
         if self.config_tag in read_contents:
             pass
         elif self.super_tag in read_contents or (('/' in read_contents) and (' #' in read_contents)):
             if self.model in ['VG710', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915']:
                 self.send_cli(["cli", "con t"], [self.user_tag, None])
             elif self.model == 'IR302':
                 self.send_cli(["console", "enable", self.password, 'con t'])
+            elif self.model == 'ODU2002':
+                self.send_cli(["cli", "enable", self.password, "con t"], [self.normal_tag, None, None, None])
         elif self.user_tag in read_contents:
-            if self.model in ['VG710', 'IR302', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915']:
+            if self.model in ['VG710', 'IR302', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915', 'ODU2002']:
                 self.send_cli(['con t'])
         elif self.normal_tag in read_contents:
-            if self.model in ['VG710', 'IR302', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915']:
+            if self.model in ['VG710', 'IR302', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915', 'ODU2002']:
                 self.send_cli(["enable", self.password, 'con t'])
         elif self.factory_tag in read_contents:
-            if self.model in ['VG710', 'IR302', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915']:
+            if self.model in ['VG710', 'IR302', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915', 'ODU2002']:
                 self.send_cli(['exit', 'con t'])
         else:
             logging.warning(f'not support this mode, last content:{read_contents}')
             self.close()
             self.__login()
             self.config_mode()
         logging.info(f"Device {self.host} access in config mode")
@@ -194,30 +197,32 @@
         """用户特权模式， 默认进入就是用户特权模式
 
         :return:
         """
         self.tn.write(("\003" + "\r").encode("cp936"))
         time.sleep(1)
         read_contents = self.tn.read_very_eager().decode('cp936').strip()
-        logging.info(read_contents)
+        logging.debug(read_contents)
         if self.config_tag in read_contents:
-            if self.model in ['VG710', 'IR302', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915']:
+            if self.model in ['VG710', 'IR302', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915', 'ODU2002']:
                 self.send_cli(['exit'])
         elif self.super_tag in read_contents or (('/' in read_contents) and (' #' in read_contents)):
             if self.model in ['VG710', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915']:
                 self.send_cli(["cli"], [self.user_tag])
             elif self.model in ['IR302']:
                 self.send_cli(["console", "enable", self.password])
+            elif self.model == 'ODU2002':
+                self.send_cli(["cli", "enable", self.password], [self.normal_tag, None, None])
         elif self.user_tag in read_contents:
             pass
         elif self.normal_tag in read_contents:
-            if self.model in ['VG710', 'IR302', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915']:
+            if self.model in ['VG710', 'IR302', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915', 'ODU2002']:
                 self.send_cli(["enable", self.password])
         elif self.factory_tag in read_contents:
-            if self.model in ['VG710', 'IR302', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915']:
+            if self.model in ['VG710', 'IR302', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915', 'ODU2002']:
                 self.send_cli(['exit'])
         else:
             logging.warning(f'not support this mode. telnet return contents: {read_contents}')
             self.close()
             self.__login()
             self.user_mode()
         logging.info(f"Device {self.host} access in user mode")
@@ -227,34 +232,36 @@
         """普通模式
 
         :return:
         """
         self.tn.write(("\003" + "\r").encode("cp936"))  # 普通模式下输入ctrl+c会返回  % Command is not supported!
         time.sleep(1)
         read_contents = self.tn.read_very_eager().decode('cp936').strip()
-        logging.info(read_contents)
+        logging.debug(read_contents)
         if self.config_tag in read_contents:
-            if self.model in ['VG710', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915']:
+            if self.model in ['VG710', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915', 'ODU2002']:
                 self.send_cli(['exit', 'disable'])
             elif self.model in ['IR302']:
                 self.send_cli(['exit', 'exit'])
         elif self.super_tag in read_contents or (('/' in read_contents) and (' #' in read_contents)):
             if self.model in ['VG710', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915']:
                 self.send_cli(["cli", "disable"], [self.user_tag, None])
             elif self.model in ['IR302']:
                 self.send_cli(["console"])
+            elif self.model == 'ODU2002':
+                self.send_cli(["cli"], [self.normal_tag])
         elif self.user_tag in read_contents:
-            if self.model in ['VG710', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915']:
+            if self.model in ['VG710', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915', 'ODU2002']:
                 self.send_cli(['disable'])
             elif self.model in ['IR302']:
                 self.send_cli(['exit'])
         elif self.normal_tag in read_contents:
             pass
         elif self.factory_tag in read_contents:
-            if self.model in ['VG710', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915']:
+            if self.model in ['VG710', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915', 'ODU2002']:
                 self.send_cli(['exit', 'disable'])
             elif self.model in ['IR302']:
                 self.send_cli(['exit', 'exit'])
         else:
             logging.warning(
                 f'not support this mode. telnet return contents: {read_contents} normal_tag: {self.normal_tag}')
             self.close()
@@ -269,15 +276,15 @@
         :return:
         """
         if not self.factory_username or not self.factory_password:
             raise Exception("sure this device support factory mode, and init factory_username、factory_password")
         self.tn.write(("\003" + "\r").encode("cp936"))
         time.sleep(1)
         read_contents = self.tn.read_very_eager().decode('cp936').strip()
-        logging.info(read_contents)
+        logging.debug(read_contents)
         if self.config_tag in read_contents:
             if self.model in ['VG710', 'IR302', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915']:
                 self.send_cli(['exit', self.factory_username + " " + self.factory_password])
         elif self.super_tag in read_contents or (('/' in read_contents) and (' #' in read_contents)):
             if self.model in ['VG710', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915']:
                 self.send_cli(["cli", self.factory_username + " " + self.factory_password], [self.user_tag, None])
             elif self.model in ['IR302']:
@@ -348,15 +355,15 @@
             for com, read_until_ in zip(command, read_until):
                 self.tn.write((com + "\n").encode("cp936"))
                 until_result = []
                 for i in range(0, timeout, 1):  # 30秒没有找到期望的就主动断开
                     time.sleep(1)
                     result = self.tn.read_very_eager().decode('cp936', "ignore").strip()
                     if result:
-                        logging.info(result)
+                        logging.debug(result)
                         result = result.split(com + "\r\n")[-1]
                     if read_until_:
                         until_result.append(result)
                         if isinstance(read_until_, str):
                             if read_until_ in ''.join(until_result):
                                 result = ''.join(until_result)
                                 break
@@ -412,24 +419,25 @@
         if key_replace is None:
             key_replace = {'\r\n': ''}
         if cli is not None:
             for i in range(0, timeout, interval):
                 if key_replace and 'cli' in key_replace_type:
                     cli = replace_str(cli, key_replace)
                     key_replace_type = key_replace_type.replace('cli', '')
-                result = self.send_cli(cli, read_until, type_=type_, key_replace=key_replace, key_replace_type=key_replace_type,
+                result = self.send_cli(cli, read_until, type_=type_, key_replace=key_replace,
+                                       key_replace_type=key_replace_type,
                                        interface_replace_type=interface_replace_type)
                 expect = str(expect) if isinstance(expect, int) else expect
                 check_ = True
                 if expect:
                     if 'expect' in key_replace_type:
                         expect = replace_str(expect, key_replace)
                     if 'expect' in interface_replace_type:
                         expect = replace_str(expect, self.interface_replace)
-                    logging.info(f'start assert cli expect {expect}')
+                    logging.debug(f'start assert cli expect {expect}')
                     if isinstance(expect, str):
                         if expect not in result:
                             check_ = False
                     elif isinstance(expect, list):
                         if [expect_ for expect_ in expect if expect_ not in result]:
                             check_ = False
                     elif isinstance(expect, dict):
@@ -447,26 +455,29 @@
                 if check_:
                     break
                 else:
                     time.sleep(interval)
                     logging.info(f"{expect} assert failure, wait for {interval}s inspection")
             else:
                 raise Exception(f'{expect} not found timeout')
-            logging.info(f'assert cli normal')
+            logging.info(f'assert cli success')
 
     @__auto_login
-    @loop_inspector('Telnet ping', timeout=30)
-    def ping(self, address='www.baidu.com', packets_number=4, params='', key_replace=None, lost_packets=False) -> bool:
+    @loop_inspector('Telnet ping')
+    def ping(self, address='www.baidu.com', packets_number=4, params='', key_replace=None, lost_packets=False,
+             timeout=30, interval=5) -> bool:
         """设备里面ping地址
 
         :param address: 域名或者IP
         :param packets_number, ping 包的个数，默认都是4个
         :param params: 参数 如'-I cellular1'、'-s 32'
         :param key_replace: 字典类型， 传入的参数转换关系表{$old: $new}
         :param lost_packets: True|False 如果为True判断会丢包，如果为False判断不丢包
+        :param timeout: 检测超时时间  秒
+        :param interval: 检测间隔时间 秒
         :return:
         """
         self.super_mode()
         params = params if params.startswith(' ') else ' ' + params
         x = True
         result = self.send_cli("ping " + address + params + f' -c {packets_number}', self.super_tag,
                                key_replace=key_replace, key_replace_type='cli', )
@@ -513,15 +524,15 @@
                 expect = [_ for _ in expect.keys()]
             else:
                 pass
             if not tag_not:  # 判断需要抓到
                 try:
                     self.send_cli(command, [expect], timeout=15, type_='super', key_replace=key_replace,
                                   key_replace_type='cli')
-                    logging.info('find the exception in tcpdump result.')
+                    logging.debug('find the exception in tcpdump result.')
                     self.tn.write(("\003" + "\r").encode("cp936"))
                     break
                 except:
                     time.sleep(interval)
                     continue
             else:  # 判断不需要抓到
                 try:
@@ -532,58 +543,60 @@
                     continue
                 except:
                     break
         else:
             raise Exception('TcpdumpTimeOutError')
 
     @__auto_login
-    @loop_inspector('Telnet regular match content', timeout=20)
+    @loop_inspector('Telnet regular match content')
     def re_match(self, command: str or list, regular: str or list, type_='super',
-                 key_replace=None, key_replace_type='last_read') -> str or List[str]:
+                 key_replace=None, key_replace_type='last_read', timeout=20, interval=5) -> str or List[str]:
         """根据表达式获取最后一次执行命令的匹配值
 
         :param command: 发送命令，可以是一条或多条
         :param regular: 正则表达式，对执行的最后一次命令返回内容进行正则查询，必须要查询到，
                         如果查不到，直至查询超时并报错
                         如果查到不止一个，返回每个正则表达式的第一个
                         列子：硬件地址 r'HWaddr(.*)inet6'， '(([0-9a-fA-F]{2}[:]){5}([0-9a-fA-F]{2})|([0-9a-fA-F]{2}[-]){5}([0-9a-fA-F]{2}))'
         :param type_: 'super'|'config'|'user'|'normal'|'factory'|None
         :param key_replace: dict 替换最后一次命令返回内容的值 默认：{'\r\n':'', ' ': ''}
         :param key_replace_type: 'cli'|'last_read'|'cli_last_read'，仅在key_replace 有值时生效，默认last_read
                                  'cli': 仅替换发出去的命令
                                  'last_read': 仅替换最后读取到的内容
                                  'cli_last_read': 既要替换cli 也要替换最后读取到的内容
+        :param timeout: 超时时间 s
+        :param interval: 检测间隔时间 s
         :return: str or list ，根据正则表达式的个数返回值
         """
         key_replace = {'\r\n': '', ' ': ''} if key_replace is None else key_replace
         key_replace_type = 'last_read' if key_replace_type is None else key_replace_type
         result = self.send_cli(command, type_=type_, key_replace=key_replace, key_replace_type=key_replace_type)
         if isinstance(regular, str):
             re_list = re.findall(regular, result)
             if re_list:
                 for i in re_list:
                     if isinstance(i, str):
                         return re.findall(regular, result)[0]
                     else:
                         return re.findall(regular, result)[0]
             else:
-                logging.info(f'regular {regular} match content None')
+                logging.debug(f'regular {regular} match content None')
                 return False
         elif isinstance(regular, list):
             result_ = []
             for regular_ in regular:
                 re_list = re.findall(regular_, result)
                 if re_list:
                     for i in re_list:
                         if isinstance(i, str):
                             result_.append(re.findall(regular_, result)[0])
                         else:
                             result_.append(re.findall(regular_, result)[0][0])
                 else:
-                    logging.info(f'regular {regular_} match content None')
+                    logging.debug(f'regular {regular_} match content None')
                     return False
             else:
                 return result_
 
     # intools 实现获取信息更改信息
     @__auto_login
     def in_tools(self, get_info: str or list) -> str or List[str] or None:
@@ -637,17 +650,18 @@
         self.tn.close()
         logging.info("Telnet 【%s:%s】 close connect session" % (self.host, self.port))
 
 
 if __name__ == '__main__':
     import sys
 
-    logging.basicConfig(format='%(asctime)s %(levelname)s %(message)s', level=logging.INFO, stream=sys.stdout)
+    logging.basicConfig(format='%(asctime)s %(levelname)s %(message)s', level=logging.DEBUG, stream=sys.stdout)
     device = Telnet('IG902', '10.5.24.96', 'inhand', '64391099@inhand')
-    # device.send_cli('ifconfig', '/www #', 'super')
+    # device.tcpdump(expect='10.5.24.224.62227', interface='eth0.4094',)
+    device.send_cli('ifconfig', '/www #', 'super')
 
-        # device = Telnet('IG902', '
+    # device = Telnet('IG902', '
     # device = Telnet('VG710', '10.5.24.206', 'inhand', '64391099@inhand')
     # a = device.send_cli('ping www.baidu.com -c 4', '/www #', 'super')
     # print(eval('1==2'))
     # device.assert_cli('ifconfig |grep wifi', expect='Local', interface_replace_type='cli_expect_last_read')
     # print(device.re_match('ifconfig eth0', r'HWaddr(.*)inet6', key_replace={'\r\n':'', ' ': ''}))
```

### Comparing `inhandtest-0.0.50/inhandtest/tools.py` & `inhandtest-0.0.51/inhandtest/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             for i in range(0, timeout, interval):
                 result = func(*args, **kwargs)
                 if not result:
                     logging.info(f'{flag} assert failure, wait for {interval}s inspection')
                     time.sleep(interval)
                     continue
                 else:
-                    logging.info(f'{flag} assert normal')
+                    logging.info(f'{flag} assert success')
                     return result
             else:
                 if assertion:
                     raise AssertionError(f'{flag} assert timeout failure')
 
         return inspector
 
@@ -169,19 +169,19 @@
             if isinstance(process_, str) or isinstance(process_, int):
                 command = f'tasklist |findstr {process_}'
             else:
                 raise Exception("not support process type")
             logging.info(command)
             p = subprocess.Popen(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, encoding='gbk')
             task_result = p.communicate()[0].strip()
-            logging.info(f'find {process_} process is: {task_result}')
+            logging.debug(f'find {process_} process is: {task_result}')
             try:
                 task_result = re.sub('\s+', ' ', task_result).split(' ')
-                if len(task_result) == 6:
-                    server_name = task_result[0]
+                if len(task_result) % 6 == 0:  # 判断是6的倍数 说明一个程序打开了一个或多个进程
+                    server_name = list(set([task_result[i] for i in range(len(task_result)) if i % 6 == 0]))
                 else:
                     server_name = False
             except Exception:
                 server_name = False
             return server_name
         else:
             return False
@@ -193,26 +193,27 @@
             return _search(process)
     else:
         process = process if isinstance(process, list) else [process]
         for name_ in process:
             if isinstance(name_, str):
                 pid = _search(name_)
                 if pid:
-                    logging.info(f'taskkill /F /IM {pid}')
-                    p = subprocess.Popen(f'taskkill /F /IM {pid}', shell=True, stdout=subprocess.PIPE,
-                                         stderr=subprocess.STDOUT, encoding='gbk')
-                    logging.info(p.communicate()[0])
-                    time.sleep(3)  # 删除服务应等待几秒，服务完全退出
+                    for process_ in pid:
+                        logging.debug(f'taskkill /F /IM {process_}')
+                        p = subprocess.Popen(f'taskkill /F /IM {process_}', shell=True, stdout=subprocess.PIPE,
+                                             stderr=subprocess.STDOUT, encoding='gbk')
+                        logging.debug(p.communicate()[0])
+                        time.sleep(3)  # 删除服务应等待几秒，服务完全退出
                 else:
-                    logging.info(f'not found task {name_}')
+                    logging.debug(f'not found task {name_}')
             elif isinstance(name_, int):
-                logging.info(f'taskkill /pid {name_} /F')
+                logging.debug(f'taskkill /pid {name_} /F')
                 p = subprocess.Popen(f'taskkill /pid {name_} /F', shell=True, stdout=subprocess.PIPE,
                                      stderr=subprocess.STDOUT, encoding='gbk')
-                logging.info(p.communicate()[0])
+                logging.debug(p.communicate()[0])
                 time.sleep(3)  # 删除服务应等待几秒，服务完全退出
             else:
                 raise Exception("not support process type")
 
 
 def kill_windows_port(ip_, port: int or list) -> None:
     """ 杀死windows 相关端口服务
@@ -226,17 +227,18 @@
         for proc in psutil.process_iter(['pid', 'name']):
             try:
                 conn_list = proc.connections()
             except (psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess):
                 continue
             for conn in conn_list:
                 if conn.status == psutil.CONN_LISTEN and conn.laddr.port == one_port:
-                    logging.info(f"process {proc.pid} already use port {one_port}")
+                    logging.debug(f"process {proc.pid} already use port {one_port}")
                     # 终止进程
                     proc.kill()
+                    time.sleep(3)
                     logging.info(f"kill process {proc.pid} success")
 
     [kill_one_port(port_) for port_ in port] if isinstance(port, list) else kill_one_port(port)
 
 
 def windows_cmd(command: str or list, expect: str or list or dict = None, last_read_replace: dict = None):
     """输入一条或多条命令, 且支持对执行时最后一条命令返回的结果做断言
@@ -253,15 +255,15 @@
     for command_ in command:
         logging.info(f'windows cmd do {command_}')
         if expect is None and last_read_replace is None:
             subprocess.Popen(command_, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, encoding='gbk')
         else:
             p = subprocess.Popen(command_, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, encoding='gbk')
             last_read_content = p.communicate()[0].strip()
-            logging.info(last_read_content)
+            logging.debug(last_read_content)
     if last_read_replace and last_read_content is not None:
         last_read_content = replace_str(last_read_content, last_read_replace)
     if expect is not None:
         if isinstance(expect, str):
             if expect not in last_read_content:
                 raise AssertionError(f'{expect} not in last read content')
         elif isinstance(expect, list):
@@ -312,15 +314,15 @@
                         for co_ in r_hash_file.content.split(b'\n'):
                             if co_.decode('utf-8').endswith(firmware_name):
                                 hash_sha256_value = co_.decode('utf-8').split(' ')[0].upper()
                                 break
                         else:
                             raise Exception(f'{svn_hash_file_path} not contain {firmware_name} hash_sha256 value')
                         if file_hash(local_firmware_path, 'sha256') == hash_sha256_value:
-                            logging.info(f'{local_firmware_path} download success')
+                            logging.debug(f'{local_firmware_path} download success')
                             break
                         else:
                             logging.warning(f'download package failed, try {i + 1} time')
                     else:
                         break
                 else:
                     raise Exception("svn server down error")
@@ -520,15 +522,15 @@
             return expired
 
     if os.path.isdir(file_path):
         for i in os.listdir(file_path):
             if report_expired(i):
                 import shutil
                 shutil.rmtree(os.path.join(file_path, i))
-                logging.info(f'{i} has expired days {days}, auto remove')
+                logging.debug(f'{i} has expired days {days}, auto remove')
 
     return '_'.join([report_file_start_with, get_time_stamp(delta=+8, time_format='%Y-%m-%d-%H')])
 
 
 def stop_thread(thread):
     """某些线程会在后台一直运行，当在外界满足一定条件时，是可以停掉的
 
@@ -548,15 +550,15 @@
             raise ValueError("invalid thread id or thread already stop")
         elif res != 1:
             # """if it returns a number greater than one, you're in trouble,
             # and you should call it again with exc=NULL to revert the effect"""
             ctypes.pythonapi.PyThreadState_SetAsyncExc(tid, None)
             raise SystemError("PyThreadState_SetAsyncExc failed")
         else:
-            logging.info(f'threading {thread} stop success')
+            logging.debug(f'threading {thread} stop success')
 
     try:
         _async_raise(thread.ident, SystemExit)
     except Exception as e:
         logging.warning(e)
 
 
@@ -571,20 +573,20 @@
     for i in range(0, winreg.QueryInfoKey(key)[0]):
         skey_name = winreg.EnumKey(key, i)
         skey = winreg.OpenKey(key, skey_name)
         try:
             value = winreg.QueryValueEx(skey, 'DisplayName')[0]
             all_installed.append(value)
             if name in value:
-                logging.info(f'Found the software {name}')
+                logging.debug(f'Found the software {name}')
                 break
         except:
             pass
     else:
-        logging.info(f'all installed software is {all_installed}')
+        logging.debug(f'all installed software is {all_installed}')
         raise ResourceNotFoundError(f'Not found the software {name}')
 
 
 class DotDict(dict):
     """使用点号深度获取字典key的值
 
     """
```

### Comparing `inhandtest-0.0.50/inhandtest.egg-info/PKG-INFO` & `inhandtest-0.0.51/inhandtest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: inhandtest
-Version: 0.0.50
+Version: 0.0.51
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 Maintainer: liwei
 Maintainer-email: liwei@inhand.com.cn
 License: UNKNOWN
```

### Comparing `inhandtest-0.0.50/inhandtest.egg-info/SOURCES.txt` & `inhandtest-0.0.51/inhandtest.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
-dm/__init__.py
 dm/mqtt.py
 dm/register_v1.py
 inhandtest/__init__.py
 inhandtest/exception.py
 inhandtest/file.py
 inhandtest/inmodbus.py
 inhandtest/inmongodb.py
@@ -34,14 +33,15 @@
 inhandtest/pages/__init__.py
 inhandtest/pages/locale.py
 inhandtest/pages/ingateway/__init__.py
 inhandtest/pages/ingateway/ingateway.py
 inhandtest/pages/ingateway/locale.yml
 inhandtest/pages/ingateway/locators.py
 inhandtest/pages/ingateway/edge_computing/__init__.py
+inhandtest/pages/ingateway/edge_computing/docker_manager_locators.py
 inhandtest/pages/ingateway/edge_computing/edge_computing.py
 inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
 inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
 inhandtest/pages/ingateway/edge_computing/python_edge_computing_locators.py
 inhandtest/pages/ingateway/network/__init__.py
 inhandtest/pages/ingateway/network/acl_locators.py
 inhandtest/pages/ingateway/network/bridge_locators.py
```

### Comparing `inhandtest-0.0.50/setup.py` & `inhandtest-0.0.51/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 """
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(
     name='inhandtest',
-    version='0.0.50',
+    version='0.0.51',
     author='liwei',
     author_email='liwei@inhand.com.cn',
     description='inhand test tools, so easy',
     maintainer='liwei',
     maintainer_email='liwei@inhand.com.cn',
     # py_modules=['inhandtest.tools', 'inhandtest.telnet', 'inhandtest.inmodbus', 'inhandtest.inmqtt', 'inhandtest.file',
     #             'inhandtest.inrequest', 'inhandtest.inssh', 'inhandtest.base_page'],
```

