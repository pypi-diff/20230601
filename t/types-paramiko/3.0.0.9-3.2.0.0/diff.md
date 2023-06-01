# Comparing `tmp/types-paramiko-3.0.0.9.tar.gz` & `tmp/types-paramiko-3.2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-paramiko-3.0.0.9.tar", last modified: Wed May  3 15:15:16 2023, max compression
+gzip compressed data, was "types-paramiko-3.2.0.0.tar", last modified: Thu Jun  1 12:30:26 2023, max compression
```

## Comparing `types-paramiko-3.0.0.9.tar` & `types-paramiko-3.2.0.0.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:16.141493 types-paramiko-3.0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-05-03 15:15:14.000000 types-paramiko-3.0.0.9/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 15:15:14.000000 types-paramiko-3.0.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-03 15:15:16.141493 types-paramiko-3.0.0.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:16.141493 types-paramiko-3.0.0.9/paramiko-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-03 15:15:14.000000 types-paramiko-3.0.0.9/paramiko-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/_winapi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/agent.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/auth_handler.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/ber.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/buffered_pipe.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/channel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/common.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/compress.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/dsskey.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/ecdsakey.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/ed25519key.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/file.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/hostkeys.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/kex_curve25519.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/kex_ecdh_nist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/kex_gex.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/kex_group1.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/kex_group14.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/kex_group16.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/kex_gss.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/message.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/packet.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/pipe.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/pkey.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/primes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/proxy.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/rsakey.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/server.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/sftp.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/sftp_attr.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/sftp_client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/sftp_file.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/sftp_handle.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/sftp_server.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/sftp_si.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/ssh_exception.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/ssh_gss.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/transport.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/win_openssh.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/win_pageant.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 15:15:16.141493 types-paramiko-3.0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-03 15:15:14.000000 types-paramiko-3.0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:16.141493 types-paramiko-3.0.0.9/types_paramiko.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-03 15:15:16.000000 types-paramiko-3.0.0.9/types_paramiko.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-03 15:15:16.000000 types-paramiko-3.0.0.9/types_paramiko.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:15:16.000000 types-paramiko-3.0.0.9/types_paramiko.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 15:15:16.000000 types-paramiko-3.0.0.9/types_paramiko.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-03 15:15:16.000000 types-paramiko-3.0.0.9/types_paramiko.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:30:26.684865 types-paramiko-3.2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-06-01 12:30:24.000000 types-paramiko-3.2.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-01 12:30:24.000000 types-paramiko-3.2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-01 12:30:26.684865 types-paramiko-3.2.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:30:26.680864 types-paramiko-3.2.0.0/paramiko-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-01 12:30:24.000000 types-paramiko-3.2.0.0/paramiko-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/_winapi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/agent.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/auth_handler.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/auth_strategy.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/ber.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/buffered_pipe.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/channel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/common.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/compress.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/dsskey.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/ecdsakey.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/ed25519key.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/file.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/hostkeys.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/kex_curve25519.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/kex_ecdh_nist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/kex_gex.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/kex_group1.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/kex_group14.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/kex_group16.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/kex_gss.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/message.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/packet.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/pipe.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/pkey.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/primes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/proxy.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/rsakey.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/server.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/sftp.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/sftp_attr.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/sftp_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/sftp_file.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/sftp_handle.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/sftp_server.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/sftp_si.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/ssh_exception.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/ssh_gss.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/transport.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/win_openssh.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-01 12:30:06.000000 types-paramiko-3.2.0.0/paramiko-stubs/win_pageant.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 12:30:26.684865 types-paramiko-3.2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-01 12:30:24.000000 types-paramiko-3.2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:30:26.680864 types-paramiko-3.2.0.0/types_paramiko.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-01 12:30:26.000000 types-paramiko-3.2.0.0/types_paramiko.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-01 12:30:26.000000 types-paramiko-3.2.0.0/types_paramiko.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 12:30:26.000000 types-paramiko-3.2.0.0/types_paramiko.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-01 12:30:26.000000 types-paramiko-3.2.0.0/types_paramiko.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-01 12:30:26.000000 types-paramiko-3.2.0.0/types_paramiko.egg-info/top_level.txt
```

### Comparing `types-paramiko-3.0.0.9/CHANGELOG.md` & `types-paramiko-3.2.0.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+## 3.2.0.0 (2023-06-01)
+
+Bump `paramiko` to 3.2.* (#10237)
+
+## 3.0.0.10 (2023-05-10)
+
+Add `partial_stub` metadata field (#10157)
+
 ## 3.0.0.9 (2023-05-03)
 
 paramiko: Improve various bytes-related types (#10109)
 
 ## 3.0.0.8 (2023-04-25)
 
 `paramiko`: Be more lenient for client parameter types (#10083)
```

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/__init__.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/_winapi.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/_winapi.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/agent.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/agent.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -58,11 +58,12 @@
     def close(self) -> None: ...
 
 class AgentKey(PKey):
     agent: AgentSSH
     blob: bytes
     public_blob: None
     name: str
-    def __init__(self, agent: AgentSSH, blob: ReadableBuffer) -> None: ...
+    comment: str
+    def __init__(self, agent: AgentSSH, blob: ReadableBuffer, comment: str = "") -> None: ...
     def asbytes(self) -> bytes: ...
     def get_name(self) -> str: ...
     def sign_ssh_data(self, data: _LikeBytes, algorithm: str | None = None) -> Message: ...
```

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/auth_handler.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/auth_handler.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/ber.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/ber.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/channel.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/channel.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/client.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from collections.abc import Iterable, Mapping
 from typing import NoReturn, Protocol
 
+from paramiko.auth_strategy import AuthStrategy
 from paramiko.channel import Channel, ChannelFile, ChannelStderrFile, ChannelStdinFile
 from paramiko.hostkeys import HostKeys
 from paramiko.pkey import PKey
 from paramiko.sftp_client import SFTPClient
-from paramiko.transport import Transport
+from paramiko.transport import Transport, _SocketLike
 from paramiko.util import ClosingContextManager
 
-from .transport import _SocketLike
-
 class _TransportFactory(Protocol):
     def __call__(
         self,
         __sock: _SocketLike,
         *,
         gss_kex: bool,
         gss_deleg_creds: bool,
@@ -43,18 +42,20 @@
         sock: _SocketLike | None = None,
         gss_auth: bool = False,
         gss_kex: bool = False,
         gss_deleg_creds: bool = True,
         gss_host: str | None = None,
         banner_timeout: float | None = None,
         auth_timeout: float | None = None,
+        channel_timeout: float | None = None,
         gss_trust_dns: bool = True,
         passphrase: str | None = None,
         disabled_algorithms: Mapping[str, Iterable[str]] | None = None,
         transport_factory: _TransportFactory | None = None,
+        auth_strategy: AuthStrategy | None = None,
     ) -> None: ...
     def close(self) -> None: ...
     def exec_command(
         self,
         command: str,
         bufsize: int = -1,
         timeout: float | None = None,
```

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/common.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/common.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/config.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/config.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/dsskey.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/dsskey.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/ecdsakey.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/ecdsakey.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/ed25519key.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/ed25519key.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/file.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/file.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/hostkeys.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/hostkeys.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/kex_curve25519.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/kex_curve25519.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/kex_ecdh_nist.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/kex_ecdh_nist.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/kex_gex.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/kex_gex.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/kex_group1.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/kex_group1.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/kex_gss.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/kex_gss.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/message.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/message.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/packet.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/packet.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/pipe.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/pipe.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/pkey.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/pkey.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/proxy.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/proxy.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/rsakey.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/rsakey.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -23,13 +23,13 @@
     @property
     def public_numbers(self) -> RSAPublicNumbers: ...
     def asbytes(self) -> bytes: ...
     def __hash__(self) -> int: ...
     def get_name(self) -> str: ...
     def get_bits(self) -> int: ...
     def can_sign(self) -> bool: ...
-    def sign_ssh_data(self, data: bytes, algorithm: str = "ssh-rsa") -> Message: ...  # type: ignore[override]
+    def sign_ssh_data(self, data: bytes, algorithm: str | None = None) -> Message: ...  # type: ignore[override]
     def verify_ssh_sig(self, data: bytes, msg: Message) -> bool: ...
     def write_private_key_file(self, filename: str, password: str | None = None) -> None: ...
     def write_private_key(self, file_obj: IO[str], password: str | None = None) -> None: ...
     @staticmethod
     def generate(bits: int, progress_func: Callable[..., object] | None = None) -> RSAKey: ...
```

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/server.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/server.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/sftp.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/sftp.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/sftp_attr.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/sftp_attr.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/sftp_client.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/sftp_client.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/sftp_file.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/sftp_file.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/sftp_server.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/sftp_server.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/sftp_si.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/sftp_si.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/ssh_exception.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/ssh_exception.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/ssh_gss.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/ssh_gss.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/transport.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/transport.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/paramiko-stubs/util.pyi` & `types-paramiko-3.2.0.0/paramiko-stubs/util.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.9/setup.py` & `types-paramiko-3.2.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,33 +11,37 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `paramiko`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/paramiko. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `ec1130adcc12431ba85415a6533da68c3692b2cb`.
+This package was generated from typeshed commit `7595478998957399ffbc7336ca783c648dc569b5`.
 '''.lstrip()
 
 setup(name=name,
-      version="3.0.0.9",
+      version="3.2.0.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/paramiko.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=['cryptography>=37.0.0'],
       packages=['paramiko-stubs'],
-      package_data={'paramiko-stubs': ['__init__.pyi', '_version.pyi', '_winapi.pyi', 'agent.pyi', 'auth_handler.pyi', 'ber.pyi', 'buffered_pipe.pyi', 'channel.pyi', 'client.pyi', 'common.pyi', 'compress.pyi', 'config.pyi', 'dsskey.pyi', 'ecdsakey.pyi', 'ed25519key.pyi', 'file.pyi', 'hostkeys.pyi', 'kex_curve25519.pyi', 'kex_ecdh_nist.pyi', 'kex_gex.pyi', 'kex_group1.pyi', 'kex_group14.pyi', 'kex_group16.pyi', 'kex_gss.pyi', 'message.pyi', 'packet.pyi', 'pipe.pyi', 'pkey.pyi', 'primes.pyi', 'proxy.pyi', 'rsakey.pyi', 'server.pyi', 'sftp.pyi', 'sftp_attr.pyi', 'sftp_client.pyi', 'sftp_file.pyi', 'sftp_handle.pyi', 'sftp_server.pyi', 'sftp_si.pyi', 'ssh_exception.pyi', 'ssh_gss.pyi', 'transport.pyi', 'util.pyi', 'win_openssh.pyi', 'win_pageant.pyi', 'METADATA.toml']},
+      package_data={'paramiko-stubs': ['__init__.pyi', '_version.pyi', '_winapi.pyi', 'agent.pyi', 'auth_handler.pyi', 'auth_strategy.pyi', 'ber.pyi', 'buffered_pipe.pyi', 'channel.pyi', 'client.pyi', 'common.pyi', 'compress.pyi', 'config.pyi', 'dsskey.pyi', 'ecdsakey.pyi', 'ed25519key.pyi', 'file.pyi', 'hostkeys.pyi', 'kex_curve25519.pyi', 'kex_ecdh_nist.pyi', 'kex_gex.pyi', 'kex_group1.pyi', 'kex_group14.pyi', 'kex_group16.pyi', 'kex_gss.pyi', 'message.pyi', 'packet.pyi', 'pipe.pyi', 'pkey.pyi', 'primes.pyi', 'proxy.pyi', 'rsakey.pyi', 'server.pyi', 'sftp.pyi', 'sftp_attr.pyi', 'sftp_client.pyi', 'sftp_file.pyi', 'sftp_handle.pyi', 'sftp_server.pyi', 'sftp_si.pyi', 'ssh_exception.pyi', 'ssh_gss.pyi', 'transport.pyi', 'util.pyi', 'win_openssh.pyi', 'win_pageant.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-paramiko-3.0.0.9/types_paramiko.egg-info/SOURCES.txt` & `types-paramiko-3.2.0.0/types_paramiko.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 paramiko-stubs/METADATA.toml
 paramiko-stubs/__init__.pyi
 paramiko-stubs/_version.pyi
 paramiko-stubs/_winapi.pyi
 paramiko-stubs/agent.pyi
 paramiko-stubs/auth_handler.pyi
+paramiko-stubs/auth_strategy.pyi
 paramiko-stubs/ber.pyi
 paramiko-stubs/buffered_pipe.pyi
 paramiko-stubs/channel.pyi
 paramiko-stubs/client.pyi
 paramiko-stubs/common.pyi
 paramiko-stubs/compress.pyi
 paramiko-stubs/config.pyi
```

