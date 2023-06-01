# Comparing `tmp/pulumi_proxmoxve-5.0.1.tar.gz` & `tmp/pulumi_proxmoxve-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_proxmoxve-5.0.1.tar", last modified: Sat May 27 06:39:18 2023, max compression
+gzip compressed data, was "pulumi_proxmoxve-5.1.0.tar", last modified: Thu Jun  1 11:06:50 2023, max compression
```

## Comparing `pulumi_proxmoxve-5.0.1.tar` & `pulumi_proxmoxve-5.1.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:39:18.964917 pulumi_proxmoxve-5.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-05-27 06:39:18.964917 pulumi_proxmoxve-5.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:39:18.956917 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7372 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/certifi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:39:18.960917 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/cluster/get_nodes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:39:18.960917 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:39:18.960917 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/ct/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/ct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/ct/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    37407 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/ct/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    15863 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/ct/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/get_dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/get_hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/get_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/get_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/hosts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:39:18.960917 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/network/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/network/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13547 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/network/firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/network/firewall_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/network/firewall_ip_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    29546 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/network/firewall_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    11681 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/network/firewall_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    15125 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/network/firewall_security_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/network/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:39:18.960917 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/permission/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/permission/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/permission/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/permission/get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/permission/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/permission/get_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/permission/get_pools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/permission/get_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/permission/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/permission/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/permission/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/permission/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/permission/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/permission/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/permission/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    22997 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/permission/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:39:18.964917 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/storage/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17318 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/storage/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/storage/get_datastores.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/storage/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:39:18.964917 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/vm/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/vm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34450 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/vm/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/vm/get_virtual_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/vm/get_virtual_machines.py
--rw-r--r--   0 runner    (1001) docker     (123)    28465 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/vm/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    83159 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/vm/virtual_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:39:18.956917 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/pulumi_proxmoxve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 06:39:18.964917 pulumi_proxmoxve-5.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-27 06:39:18.000000 pulumi_proxmoxve-5.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:06:50.128763 pulumi_proxmoxve-5.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-06-01 11:06:50.124763 pulumi_proxmoxve-5.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:06:50.116763 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/certifi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:06:50.116763 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/cluster/get_nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:06:50.116763 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:06:50.116763 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/ct/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/ct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/ct/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37407 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/ct/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15863 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/ct/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/get_dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/get_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/get_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/get_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/hosts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:06:50.120763 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/network/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13547 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/network/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/network/firewall_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/network/firewall_ip_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29546 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/network/firewall_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11681 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/network/firewall_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15125 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/network/firewall_security_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/network/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:06:50.124763 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/permission/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/permission/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/permission/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/permission/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/permission/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/permission/get_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/permission/get_pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/permission/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/permission/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/permission/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/permission/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/permission/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/permission/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/permission/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/permission/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22997 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/permission/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12698 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:06:50.124763 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/storage/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17318 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/storage/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/storage/get_datastores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/storage/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:06:50.124763 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/vm/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/vm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34450 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/vm/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/vm/get_virtual_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/vm/get_virtual_machines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28465 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/vm/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83159 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/vm/virtual_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:06:50.116763 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-06-01 11:06:50.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-01 11:06:50.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 11:06:50.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 11:06:50.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-01 11:06:50.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-01 11:06:50.000000 pulumi_proxmoxve-5.1.0/pulumi_proxmoxve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 11:06:50.128763 pulumi_proxmoxve-5.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-01 11:06:49.000000 pulumi_proxmoxve-5.1.0/setup.py
```

### Comparing `pulumi_proxmoxve-5.0.1/PKG-INFO` & `pulumi_proxmoxve-5.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pulumi_proxmoxve
-Version: 5.0.1
+Version: 5.1.0
 Summary: A Pulumi package for creating and managing Proxmox Virtual Environment cloud resources.
 Home-page: https://github.com/muhlba91/pulumi-proxmoxve
 License: Apache-2.0
 Project-URL: Repository, https://github.com/muhlba91/pulumi-proxmoxve
 Keywords: pulumi proxmox proxmoxve
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Proxmox VE Resource Provider
 
 [![](https://img.shields.io/github/license/muhlba91/pulumi-proxmoxve?style=for-the-badge)](LICENSE)
-[![](https://img.shields.io/github/actions/workflow/status/muhlba91/pulumi-proxmoxve/release.yml?style=for-the-badge)](https://github.com/muhlba91/pulumi-proxmoxve/actions)
+[![](https://img.shields.io/github/actions/workflow/status/muhlba91/pulumi-proxmoxve/verify.yml?style=for-the-badge)](https://github.com/muhlba91/pulumi-proxmoxve/actions/workflows/verify.yml)
 [![](https://img.shields.io/github/release-date/muhlba91/pulumi-proxmoxve?style=for-the-badge)](https://github.com/muhlba91/pulumi-proxmoxve/releases)
 [![](https://img.shields.io/pypi/v/pulumi-proxmoxve?style=for-the-badge)](https://pypi.org/project/pulumi-proxmoxve/)
 [![](https://img.shields.io/pypi/dm/pulumi-proxmoxve?style=for-the-badge)](https://pypi.org/project/pulumi-proxmoxve/)
 [![](https://img.shields.io/nuget/v/Pulumi.ProxmoxVE?style=for-the-badge)](https://www.nuget.org/packages/Pulumi.ProxmoxVE/)
 [![](https://img.shields.io/nuget/dt/Pulumi.ProxmoxVE?style=for-the-badge)](https://www.nuget.org/packages/Pulumi.ProxmoxVE/)
 [![](https://img.shields.io/npm/v/@muhlba91/pulumi-proxmoxve?style=for-the-badge)](https://www.npmjs.com/package/@muhlba91/pulumi-proxmoxve)
 [![](https://img.shields.io/npm/dm/@muhlba91/pulumi-proxmoxve?style=for-the-badge)](https://www.npmjs.com/package/@muhlba91/pulumi-proxmoxve)
@@ -29,14 +29,15 @@
 The provider is built on https://github.com/bpg/terraform-provider-proxmox.
 
 ## Installing
 
 This package is available in many languages in the standard packaging formats.
 
 ### Installing the Plugin
+
 1. Download the appropriate archive file from the Releases page:
    `wget https://github.com/muhlba91/pulumi-proxmoxve/releases/download/vX.Y.Z/pulumi-resource-proxmoxve-vX.Y.Z-OPERATING_SYSTEM-ARCH.tar.gz`
 2. Add the plugin to Pulumi:
    `pulumi plugin install resource proxmoxve X.Y.Z -f ./pulumi-resource-proxmoxve-vX.Y.Z-OPERATING_SYSTEM-ARCH.tar.gz`
 
 ### Node.js (JavaScript/TypeScript)
 
@@ -78,14 +79,15 @@
 
 ## Configuration
 
 Unfortunately, configuration via environment variables is not (yet) working.
 To configure the provider you must create and pass it through.
 
 Example for *Typescript*:
+
 ```typescript
 import * as proxmox from '@muhlba91/pulumi-proxmoxve';
 
 const provider = new proxmox.Provider('proxmoxve', {
   endpoint: process.env.PROXMOX_VE_ENDPOINT,
   insecure: process.env.PROXMOX_VE_INSECURE,
   username: process.env.PROXMOX_VE_USERNAME,
```

### Comparing `pulumi_proxmoxve-5.0.1/README.md` & `pulumi_proxmoxve-5.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Proxmox VE Resource Provider
 
 [![](https://img.shields.io/github/license/muhlba91/pulumi-proxmoxve?style=for-the-badge)](LICENSE)
-[![](https://img.shields.io/github/actions/workflow/status/muhlba91/pulumi-proxmoxve/release.yml?style=for-the-badge)](https://github.com/muhlba91/pulumi-proxmoxve/actions)
+[![](https://img.shields.io/github/actions/workflow/status/muhlba91/pulumi-proxmoxve/verify.yml?style=for-the-badge)](https://github.com/muhlba91/pulumi-proxmoxve/actions/workflows/verify.yml)
 [![](https://img.shields.io/github/release-date/muhlba91/pulumi-proxmoxve?style=for-the-badge)](https://github.com/muhlba91/pulumi-proxmoxve/releases)
 [![](https://img.shields.io/pypi/v/pulumi-proxmoxve?style=for-the-badge)](https://pypi.org/project/pulumi-proxmoxve/)
 [![](https://img.shields.io/pypi/dm/pulumi-proxmoxve?style=for-the-badge)](https://pypi.org/project/pulumi-proxmoxve/)
 [![](https://img.shields.io/nuget/v/Pulumi.ProxmoxVE?style=for-the-badge)](https://www.nuget.org/packages/Pulumi.ProxmoxVE/)
 [![](https://img.shields.io/nuget/dt/Pulumi.ProxmoxVE?style=for-the-badge)](https://www.nuget.org/packages/Pulumi.ProxmoxVE/)
 [![](https://img.shields.io/npm/v/@muhlba91/pulumi-proxmoxve?style=for-the-badge)](https://www.npmjs.com/package/@muhlba91/pulumi-proxmoxve)
 [![](https://img.shields.io/npm/dm/@muhlba91/pulumi-proxmoxve?style=for-the-badge)](https://www.npmjs.com/package/@muhlba91/pulumi-proxmoxve)
@@ -17,14 +17,15 @@
 The provider is built on https://github.com/bpg/terraform-provider-proxmox.
 
 ## Installing
 
 This package is available in many languages in the standard packaging formats.
 
 ### Installing the Plugin
+
 1. Download the appropriate archive file from the Releases page:
    `wget https://github.com/muhlba91/pulumi-proxmoxve/releases/download/vX.Y.Z/pulumi-resource-proxmoxve-vX.Y.Z-OPERATING_SYSTEM-ARCH.tar.gz`
 2. Add the plugin to Pulumi:
    `pulumi plugin install resource proxmoxve X.Y.Z -f ./pulumi-resource-proxmoxve-vX.Y.Z-OPERATING_SYSTEM-ARCH.tar.gz`
 
 ### Node.js (JavaScript/TypeScript)
 
@@ -66,14 +67,15 @@
 
 ## Configuration
 
 Unfortunately, configuration via environment variables is not (yet) working.
 To configure the provider you must create and pass it through.
 
 Example for *Typescript*:
+
 ```typescript
 import * as proxmox from '@muhlba91/pulumi-proxmoxve';
 
 const provider = new proxmox.Provider('proxmoxve', {
   endpoint: process.env.PROXMOX_VE_ENDPOINT,
   insecure: process.env.PROXMOX_VE_INSECURE,
   username: process.env.PROXMOX_VE_USERNAME,
```

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/__init__.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/_inputs.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/_inputs.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
     'HostsEntryArgs',
     'ProviderSshArgs',
+    'ProviderSshNodeArgs',
     'ProviderVirtualEnvironmentArgs',
     'ProviderVirtualEnvironmentSshArgs',
+    'ProviderVirtualEnvironmentSshNodeArgs',
 ]
 
 @pulumi.input_type
 class HostsEntryArgs:
     def __init__(__self__, *,
                  address: pulumi.Input[str],
                  hostnames: pulumi.Input[Sequence[pulumi.Input[str]]]):
@@ -44,20 +46,23 @@
 
 
 @pulumi.input_type
 class ProviderSshArgs:
     def __init__(__self__, *,
                  agent: Optional[pulumi.Input[bool]] = None,
                  agent_socket: Optional[pulumi.Input[str]] = None,
+                 node: Optional[pulumi.Input['ProviderSshNodeArgs']] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         if agent is not None:
             pulumi.set(__self__, "agent", agent)
         if agent_socket is not None:
             pulumi.set(__self__, "agent_socket", agent_socket)
+        if node is not None:
+            pulumi.set(__self__, "node", node)
         if password is not None:
             pulumi.set(__self__, "password", password)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -75,14 +80,23 @@
 
     @agent_socket.setter
     def agent_socket(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "agent_socket", value)
 
     @property
     @pulumi.getter
+    def node(self) -> Optional[pulumi.Input['ProviderSshNodeArgs']]:
+        return pulumi.get(self, "node")
+
+    @node.setter
+    def node(self, value: Optional[pulumi.Input['ProviderSshNodeArgs']]):
+        pulumi.set(self, "node", value)
+
+    @property
+    @pulumi.getter
     def password(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "password")
 
     @password.setter
     def password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "password", value)
 
@@ -93,36 +107,75 @@
 
     @username.setter
     def username(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "username", value)
 
 
 @pulumi.input_type
+class ProviderSshNodeArgs:
+    def __init__(__self__, *,
+                 address: pulumi.Input[str],
+                 name: pulumi.Input[str]):
+        pulumi.set(__self__, "address", address)
+        pulumi.set(__self__, "name", name)
+
+    @property
+    @pulumi.getter
+    def address(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "address")
+
+    @address.setter
+    def address(self, value: pulumi.Input[str]):
+        pulumi.set(self, "address", value)
+
+    @property
+    @pulumi.getter
+    def name(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
+
+
+@pulumi.input_type
 class ProviderVirtualEnvironmentArgs:
     def __init__(__self__, *,
+                 api_token: Optional[pulumi.Input[str]] = None,
                  endpoint: Optional[pulumi.Input[str]] = None,
                  insecure: Optional[pulumi.Input[bool]] = None,
                  otp: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  ssh: Optional[pulumi.Input['ProviderVirtualEnvironmentSshArgs']] = None,
                  username: Optional[pulumi.Input[str]] = None):
+        if api_token is not None:
+            pulumi.set(__self__, "api_token", api_token)
         if endpoint is not None:
             pulumi.set(__self__, "endpoint", endpoint)
         if insecure is not None:
             pulumi.set(__self__, "insecure", insecure)
         if otp is not None:
             pulumi.set(__self__, "otp", otp)
         if password is not None:
             pulumi.set(__self__, "password", password)
         if ssh is not None:
             pulumi.set(__self__, "ssh", ssh)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
+    @pulumi.getter(name="apiToken")
+    def api_token(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "api_token")
+
+    @api_token.setter
+    def api_token(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "api_token", value)
+
+    @property
     @pulumi.getter
     def endpoint(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "endpoint")
 
     @endpoint.setter
     def endpoint(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "endpoint", value)
@@ -174,20 +227,23 @@
 
 
 @pulumi.input_type
 class ProviderVirtualEnvironmentSshArgs:
     def __init__(__self__, *,
                  agent: Optional[pulumi.Input[bool]] = None,
                  agent_socket: Optional[pulumi.Input[str]] = None,
+                 node: Optional[pulumi.Input['ProviderVirtualEnvironmentSshNodeArgs']] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         if agent is not None:
             pulumi.set(__self__, "agent", agent)
         if agent_socket is not None:
             pulumi.set(__self__, "agent_socket", agent_socket)
+        if node is not None:
+            pulumi.set(__self__, "node", node)
         if password is not None:
             pulumi.set(__self__, "password", password)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -205,14 +261,23 @@
 
     @agent_socket.setter
     def agent_socket(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "agent_socket", value)
 
     @property
     @pulumi.getter
+    def node(self) -> Optional[pulumi.Input['ProviderVirtualEnvironmentSshNodeArgs']]:
+        return pulumi.get(self, "node")
+
+    @node.setter
+    def node(self, value: Optional[pulumi.Input['ProviderVirtualEnvironmentSshNodeArgs']]):
+        pulumi.set(self, "node", value)
+
+    @property
+    @pulumi.getter
     def password(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "password")
 
     @password.setter
     def password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "password", value)
 
@@ -222,7 +287,34 @@
         return pulumi.get(self, "username")
 
     @username.setter
     def username(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "username", value)
 
 
+@pulumi.input_type
+class ProviderVirtualEnvironmentSshNodeArgs:
+    def __init__(__self__, *,
+                 address: pulumi.Input[str],
+                 name: pulumi.Input[str]):
+        pulumi.set(__self__, "address", address)
+        pulumi.set(__self__, "name", name)
+
+    @property
+    @pulumi.getter
+    def address(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "address")
+
+    @address.setter
+    def address(self, value: pulumi.Input[str]):
+        pulumi.set(self, "address", value)
+
+    @property
+    @pulumi.getter
+    def name(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
+
+
```

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/_utilities.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/certifi.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/certifi.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/cluster/get_nodes.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/cluster/get_nodes.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/config/outputs.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/config/outputs.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,29 +8,34 @@
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 
 __all__ = [
     'Ssh',
+    'SshNode',
     'VirtualEnvironment',
     'VirtualEnvironmentSsh',
+    'VirtualEnvironmentSshNode',
 ]
 
 @pulumi.output_type
 class Ssh(dict):
     def __init__(__self__, *,
                  agent: Optional[bool] = None,
                  agent_socket: Optional[str] = None,
+                 node: Optional['outputs.SshNode'] = None,
                  password: Optional[str] = None,
                  username: Optional[str] = None):
         if agent is not None:
             pulumi.set(__self__, "agent", agent)
         if agent_socket is not None:
             pulumi.set(__self__, "agent_socket", agent_socket)
+        if node is not None:
+            pulumi.set(__self__, "node", node)
         if password is not None:
             pulumi.set(__self__, "password", password)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -40,46 +45,78 @@
     @property
     @pulumi.getter(name="agentSocket")
     def agent_socket(self) -> Optional[str]:
         return pulumi.get(self, "agent_socket")
 
     @property
     @pulumi.getter
+    def node(self) -> Optional['outputs.SshNode']:
+        return pulumi.get(self, "node")
+
+    @property
+    @pulumi.getter
     def password(self) -> Optional[str]:
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
+class SshNode(dict):
+    def __init__(__self__, *,
+                 address: str,
+                 name: str):
+        pulumi.set(__self__, "address", address)
+        pulumi.set(__self__, "name", name)
+
+    @property
+    @pulumi.getter
+    def address(self) -> str:
+        return pulumi.get(self, "address")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        return pulumi.get(self, "name")
+
+
+@pulumi.output_type
 class VirtualEnvironment(dict):
     def __init__(__self__, *,
+                 api_token: Optional[str] = None,
                  endpoint: Optional[str] = None,
                  insecure: Optional[bool] = None,
                  otp: Optional[str] = None,
                  password: Optional[str] = None,
                  ssh: Optional['outputs.VirtualEnvironmentSsh'] = None,
                  username: Optional[str] = None):
+        if api_token is not None:
+            pulumi.set(__self__, "api_token", api_token)
         if endpoint is not None:
             pulumi.set(__self__, "endpoint", endpoint)
         if insecure is not None:
             pulumi.set(__self__, "insecure", insecure)
         if otp is not None:
             pulumi.set(__self__, "otp", otp)
         if password is not None:
             pulumi.set(__self__, "password", password)
         if ssh is not None:
             pulumi.set(__self__, "ssh", ssh)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
+    @pulumi.getter(name="apiToken")
+    def api_token(self) -> Optional[str]:
+        return pulumi.get(self, "api_token")
+
+    @property
     @pulumi.getter
     def endpoint(self) -> Optional[str]:
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter
     def insecure(self) -> Optional[bool]:
@@ -107,20 +144,23 @@
 
 
 @pulumi.output_type
 class VirtualEnvironmentSsh(dict):
     def __init__(__self__, *,
                  agent: Optional[bool] = None,
                  agent_socket: Optional[str] = None,
+                 node: Optional['outputs.VirtualEnvironmentSshNode'] = None,
                  password: Optional[str] = None,
                  username: Optional[str] = None):
         if agent is not None:
             pulumi.set(__self__, "agent", agent)
         if agent_socket is not None:
             pulumi.set(__self__, "agent_socket", agent_socket)
+        if node is not None:
+            pulumi.set(__self__, "node", node)
         if password is not None:
             pulumi.set(__self__, "password", password)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -130,16 +170,40 @@
     @property
     @pulumi.getter(name="agentSocket")
     def agent_socket(self) -> Optional[str]:
         return pulumi.get(self, "agent_socket")
 
     @property
     @pulumi.getter
+    def node(self) -> Optional['outputs.VirtualEnvironmentSshNode']:
+        return pulumi.get(self, "node")
+
+    @property
+    @pulumi.getter
     def password(self) -> Optional[str]:
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
         return pulumi.get(self, "username")
 
 
+@pulumi.output_type
+class VirtualEnvironmentSshNode(dict):
+    def __init__(__self__, *,
+                 address: str,
+                 name: str):
+        pulumi.set(__self__, "address", address)
+        pulumi.set(__self__, "name", name)
+
+    @property
+    @pulumi.getter
+    def address(self) -> str:
+        return pulumi.get(self, "address")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        return pulumi.get(self, "name")
+
+
```

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/config/vars.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/config/vars.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,21 @@
 import types
 
 __config__ = pulumi.Config('proxmoxve')
 
 
 class _ExportableConfig(types.ModuleType):
     @property
+    def api_token(self) -> Optional[str]:
+        """
+        The API token for the Proxmox Virtual Environment API
+        """
+        return __config__.get('apiToken')
+
+    @property
     def endpoint(self) -> Optional[str]:
         """
         The endpoint for the Proxmox Virtual Environment API
         """
         return __config__.get('endpoint')
 
     @property
```

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/ct/_inputs.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/ct/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/ct/container.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/ct/container.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/ct/outputs.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/ct/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/dns.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/dns.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/get_dns.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/get_dns.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/get_hosts.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/get_hosts.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/get_time.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/get_time.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/get_version.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/get_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/hosts.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/hosts.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/network/_inputs.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/network/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/network/firewall.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/network/firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/network/firewall_alias.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/network/firewall_alias.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/network/firewall_ip_set.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/network/firewall_ip_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/network/firewall_options.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/network/firewall_options.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/network/firewall_rules.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/network/firewall_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/network/firewall_security_group.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/network/firewall_security_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/network/outputs.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/network/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/outputs.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/permission/__init__.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/permission/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/permission/_inputs.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/permission/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/permission/get_group.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/permission/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/permission/get_groups.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/permission/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/permission/get_pool.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/permission/get_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/permission/get_pools.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/permission/get_pools.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/permission/get_role.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/permission/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/permission/get_roles.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/permission/get_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/permission/get_user.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/permission/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/permission/get_users.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/permission/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/permission/group.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/permission/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/permission/outputs.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/permission/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/permission/pool.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/permission/pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/permission/role.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/permission/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/permission/user.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/permission/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/provider.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/provider.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,30 +11,34 @@
 from ._inputs import *
 
 __all__ = ['ProviderArgs', 'Provider']
 
 @pulumi.input_type
 class ProviderArgs:
     def __init__(__self__, *,
+                 api_token: Optional[pulumi.Input[str]] = None,
                  endpoint: Optional[pulumi.Input[str]] = None,
                  insecure: Optional[pulumi.Input[bool]] = None,
                  otp: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  ssh: Optional[pulumi.Input['ProviderSshArgs']] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  virtual_environment: Optional[pulumi.Input['ProviderVirtualEnvironmentArgs']] = None):
         """
         The set of arguments for constructing a Provider resource.
+        :param pulumi.Input[str] api_token: The API token for the Proxmox Virtual Environment API
         :param pulumi.Input[str] endpoint: The endpoint for the Proxmox Virtual Environment API
         :param pulumi.Input[bool] insecure: Whether to skip the TLS verification step
         :param pulumi.Input[str] otp: The one-time password for the Proxmox Virtual Environment API
         :param pulumi.Input[str] password: The password for the Proxmox Virtual Environment API
         :param pulumi.Input['ProviderSshArgs'] ssh: The SSH connection configuration to a Proxmox node
         :param pulumi.Input[str] username: The username for the Proxmox Virtual Environment API
         """
+        if api_token is not None:
+            pulumi.set(__self__, "api_token", api_token)
         if endpoint is not None:
             pulumi.set(__self__, "endpoint", endpoint)
         if insecure is not None:
             pulumi.set(__self__, "insecure", insecure)
         if otp is not None:
             pulumi.set(__self__, "otp", otp)
         if password is not None:
@@ -46,14 +50,26 @@
         if virtual_environment is not None:
             warnings.warn("""Move attributes out of virtual_environment block""", DeprecationWarning)
             pulumi.log.warn("""virtual_environment is deprecated: Move attributes out of virtual_environment block""")
         if virtual_environment is not None:
             pulumi.set(__self__, "virtual_environment", virtual_environment)
 
     @property
+    @pulumi.getter(name="apiToken")
+    def api_token(self) -> Optional[pulumi.Input[str]]:
+        """
+        The API token for the Proxmox Virtual Environment API
+        """
+        return pulumi.get(self, "api_token")
+
+    @api_token.setter
+    def api_token(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "api_token", value)
+
+    @property
     @pulumi.getter
     def endpoint(self) -> Optional[pulumi.Input[str]]:
         """
         The endpoint for the Proxmox Virtual Environment API
         """
         return pulumi.get(self, "endpoint")
 
@@ -132,14 +148,15 @@
 
 
 class Provider(pulumi.ProviderResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 api_token: Optional[pulumi.Input[str]] = None,
                  endpoint: Optional[pulumi.Input[str]] = None,
                  insecure: Optional[pulumi.Input[bool]] = None,
                  otp: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  ssh: Optional[pulumi.Input[pulumi.InputType['ProviderSshArgs']]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  virtual_environment: Optional[pulumi.Input[pulumi.InputType['ProviderVirtualEnvironmentArgs']]] = None,
@@ -148,14 +165,15 @@
         The provider type for the proxmoxve package. By default, resources use package-wide configuration
         settings, however an explicit `Provider` instance may be created and passed during resource
         construction to achieve fine-grained programmatic control over provider settings. See the
         [documentation](https://www.pulumi.com/docs/reference/programming-model/#providers) for more information.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] api_token: The API token for the Proxmox Virtual Environment API
         :param pulumi.Input[str] endpoint: The endpoint for the Proxmox Virtual Environment API
         :param pulumi.Input[bool] insecure: Whether to skip the TLS verification step
         :param pulumi.Input[str] otp: The one-time password for the Proxmox Virtual Environment API
         :param pulumi.Input[str] password: The password for the Proxmox Virtual Environment API
         :param pulumi.Input[pulumi.InputType['ProviderSshArgs']] ssh: The SSH connection configuration to a Proxmox node
         :param pulumi.Input[str] username: The username for the Proxmox Virtual Environment API
         """
@@ -182,14 +200,15 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 api_token: Optional[pulumi.Input[str]] = None,
                  endpoint: Optional[pulumi.Input[str]] = None,
                  insecure: Optional[pulumi.Input[bool]] = None,
                  otp: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  ssh: Optional[pulumi.Input[pulumi.InputType['ProviderSshArgs']]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  virtual_environment: Optional[pulumi.Input[pulumi.InputType['ProviderVirtualEnvironmentArgs']]] = None,
@@ -198,31 +217,42 @@
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProviderArgs.__new__(ProviderArgs)
 
+            __props__.__dict__["api_token"] = None if api_token is None else pulumi.Output.secret(api_token)
             __props__.__dict__["endpoint"] = endpoint
             __props__.__dict__["insecure"] = pulumi.Output.from_input(insecure).apply(pulumi.runtime.to_json) if insecure is not None else None
             __props__.__dict__["otp"] = otp
-            __props__.__dict__["password"] = password
+            __props__.__dict__["password"] = None if password is None else pulumi.Output.secret(password)
             __props__.__dict__["ssh"] = pulumi.Output.from_input(ssh).apply(pulumi.runtime.to_json) if ssh is not None else None
             __props__.__dict__["username"] = username
             if virtual_environment is not None and not opts.urn:
                 warnings.warn("""Move attributes out of virtual_environment block""", DeprecationWarning)
                 pulumi.log.warn("""virtual_environment is deprecated: Move attributes out of virtual_environment block""")
             __props__.__dict__["virtual_environment"] = pulumi.Output.from_input(virtual_environment).apply(pulumi.runtime.to_json) if virtual_environment is not None else None
+        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["apiToken", "password"])
+        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(Provider, __self__).__init__(
             'proxmoxve',
             resource_name,
             __props__,
             opts)
 
     @property
+    @pulumi.getter(name="apiToken")
+    def api_token(self) -> pulumi.Output[Optional[str]]:
+        """
+        The API token for the Proxmox Virtual Environment API
+        """
+        return pulumi.get(self, "api_token")
+
+    @property
     @pulumi.getter
     def endpoint(self) -> pulumi.Output[Optional[str]]:
         """
         The endpoint for the Proxmox Virtual Environment API
         """
         return pulumi.get(self, "endpoint")
```

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/storage/_inputs.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/storage/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/storage/file.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/storage/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/storage/get_datastores.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/storage/get_datastores.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/storage/outputs.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/storage/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/time.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/time.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/vm/_inputs.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/vm/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/vm/get_virtual_machine.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/vm/get_virtual_machine.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/vm/get_virtual_machines.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/vm/get_virtual_machines.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/vm/outputs.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/vm/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve/vm/virtual_machine.py` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve/vm/virtual_machine.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve.egg-info/PKG-INFO` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pulumi-proxmoxve
-Version: 5.0.1
+Version: 5.1.0
 Summary: A Pulumi package for creating and managing Proxmox Virtual Environment cloud resources.
 Home-page: https://github.com/muhlba91/pulumi-proxmoxve
 License: Apache-2.0
 Project-URL: Repository, https://github.com/muhlba91/pulumi-proxmoxve
 Keywords: pulumi proxmox proxmoxve
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Proxmox VE Resource Provider
 
 [![](https://img.shields.io/github/license/muhlba91/pulumi-proxmoxve?style=for-the-badge)](LICENSE)
-[![](https://img.shields.io/github/actions/workflow/status/muhlba91/pulumi-proxmoxve/release.yml?style=for-the-badge)](https://github.com/muhlba91/pulumi-proxmoxve/actions)
+[![](https://img.shields.io/github/actions/workflow/status/muhlba91/pulumi-proxmoxve/verify.yml?style=for-the-badge)](https://github.com/muhlba91/pulumi-proxmoxve/actions/workflows/verify.yml)
 [![](https://img.shields.io/github/release-date/muhlba91/pulumi-proxmoxve?style=for-the-badge)](https://github.com/muhlba91/pulumi-proxmoxve/releases)
 [![](https://img.shields.io/pypi/v/pulumi-proxmoxve?style=for-the-badge)](https://pypi.org/project/pulumi-proxmoxve/)
 [![](https://img.shields.io/pypi/dm/pulumi-proxmoxve?style=for-the-badge)](https://pypi.org/project/pulumi-proxmoxve/)
 [![](https://img.shields.io/nuget/v/Pulumi.ProxmoxVE?style=for-the-badge)](https://www.nuget.org/packages/Pulumi.ProxmoxVE/)
 [![](https://img.shields.io/nuget/dt/Pulumi.ProxmoxVE?style=for-the-badge)](https://www.nuget.org/packages/Pulumi.ProxmoxVE/)
 [![](https://img.shields.io/npm/v/@muhlba91/pulumi-proxmoxve?style=for-the-badge)](https://www.npmjs.com/package/@muhlba91/pulumi-proxmoxve)
 [![](https://img.shields.io/npm/dm/@muhlba91/pulumi-proxmoxve?style=for-the-badge)](https://www.npmjs.com/package/@muhlba91/pulumi-proxmoxve)
@@ -29,14 +29,15 @@
 The provider is built on https://github.com/bpg/terraform-provider-proxmox.
 
 ## Installing
 
 This package is available in many languages in the standard packaging formats.
 
 ### Installing the Plugin
+
 1. Download the appropriate archive file from the Releases page:
    `wget https://github.com/muhlba91/pulumi-proxmoxve/releases/download/vX.Y.Z/pulumi-resource-proxmoxve-vX.Y.Z-OPERATING_SYSTEM-ARCH.tar.gz`
 2. Add the plugin to Pulumi:
    `pulumi plugin install resource proxmoxve X.Y.Z -f ./pulumi-resource-proxmoxve-vX.Y.Z-OPERATING_SYSTEM-ARCH.tar.gz`
 
 ### Node.js (JavaScript/TypeScript)
 
@@ -78,14 +79,15 @@
 
 ## Configuration
 
 Unfortunately, configuration via environment variables is not (yet) working.
 To configure the provider you must create and pass it through.
 
 Example for *Typescript*:
+
 ```typescript
 import * as proxmox from '@muhlba91/pulumi-proxmoxve';
 
 const provider = new proxmox.Provider('proxmoxve', {
   endpoint: process.env.PROXMOX_VE_ENDPOINT,
   insecure: process.env.PROXMOX_VE_INSECURE,
   username: process.env.PROXMOX_VE_USERNAME,
```

### Comparing `pulumi_proxmoxve-5.0.1/pulumi_proxmoxve.egg-info/SOURCES.txt` & `pulumi_proxmoxve-5.1.0/pulumi_proxmoxve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.0.1/setup.py` & `pulumi_proxmoxve-5.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "5.0.1"
-PLUGIN_VERSION = "5.0.1"
+VERSION = "5.1.0"
+PLUGIN_VERSION = "5.1.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'proxmoxve', PLUGIN_VERSION, '--server', 'github://api.github.com/muhlba91/pulumi-proxmoxve'])
         except OSError as error:
```

