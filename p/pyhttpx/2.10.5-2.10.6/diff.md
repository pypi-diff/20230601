# Comparing `tmp/pyhttpx-2.10.5.tar.gz` & `tmp/pyhttpx-2.10.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyhttpx-2.10.5.tar", last modified: Wed May 31 14:33:21 2023, max compression
+gzip compressed data, was "dist\pyhttpx-2.10.6.tar", last modified: Thu Jun  1 08:45:16 2023, max compression
```

## Comparing `pyhttpx-2.10.5.tar` & `pyhttpx-2.10.6.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 14:33:21.000000 pyhttpx-2.10.5/
--rw-rw-rw-   0        0        0     1086 2022-08-12 14:37:21.000000 pyhttpx-2.10.5/LICENSE
--rw-rw-rw-   0        0        0       24 2022-08-15 03:00:31.000000 pyhttpx-2.10.5/MANIFEST.in
--rw-rw-rw-   0        0        0      339 2023-05-31 14:33:21.000000 pyhttpx-2.10.5/PKG-INFO
--rw-rw-rw-   0        0        0     2773 2023-05-31 14:30:16.000000 pyhttpx-2.10.5/README.md
--rw-rw-rw-   0        0        0        0 2022-08-15 02:16:12.000000 pyhttpx-2.10.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-31 14:33:21.000000 pyhttpx-2.10.5/pyhttpx/
--rw-rw-rw-   0        0        0       81 2022-12-05 09:21:49.000000 pyhttpx-2.10.5/pyhttpx/__init__.py
--rw-rw-rw-   0        0        0      262 2022-09-23 08:01:24.000000 pyhttpx-2.10.5/pyhttpx/__version__.py
--rw-rw-rw-   0        0        0      106 2022-09-23 08:01:24.000000 pyhttpx-2.10.5/pyhttpx/compat.py
--rw-rw-rw-   0        0        0     1107 2022-12-05 07:47:21.000000 pyhttpx-2.10.5/pyhttpx/exception.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:33:21.000000 pyhttpx-2.10.5/pyhttpx/layers/
--rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.5/pyhttpx/layers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:33:21.000000 pyhttpx-2.10.5/pyhttpx/layers/tls/
--rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.5/pyhttpx/layers/tls/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:33:21.000000 pyhttpx-2.10.5/pyhttpx/layers/tls/crypto/
--rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.5/pyhttpx/layers/tls/crypto/__init__.py
--rw-rw-rw-   0        0        0     2308 2022-09-23 08:01:24.000000 pyhttpx-2.10.5/pyhttpx/layers/tls/crypto/aes.py
--rw-rw-rw-   0        0        0     1114 2022-09-23 08:01:24.000000 pyhttpx-2.10.5/pyhttpx/layers/tls/crypto/chacha20_poly1305.py
--rw-rw-rw-   0        0        0     4618 2022-09-23 08:01:24.000000 pyhttpx-2.10.5/pyhttpx/layers/tls/crypto/cipher_aead.py
--rw-rw-rw-   0        0        0     3910 2022-09-23 08:01:24.000000 pyhttpx-2.10.5/pyhttpx/layers/tls/crypto/cipher_block.py
--rw-rw-rw-   0        0        0      266 2022-09-23 08:01:24.000000 pyhttpx-2.10.5/pyhttpx/layers/tls/crypto/ciphers.py
--rw-rw-rw-   0        0        0     4293 2022-09-23 08:01:24.000000 pyhttpx-2.10.5/pyhttpx/layers/tls/crypto/ecc.py
--rw-rw-rw-   0        0        0     6180 2023-01-31 06:58:53.000000 pyhttpx-2.10.5/pyhttpx/layers/tls/crypto/hkdf.py
--rw-rw-rw-   0        0        0      947 2022-09-23 08:01:24.000000 pyhttpx-2.10.5/pyhttpx/layers/tls/crypto/kx_algs.py
--rw-rw-rw-   0        0        0     1771 2022-09-23 08:01:24.000000 pyhttpx-2.10.5/pyhttpx/layers/tls/crypto/prf.py
--rw-rw-rw-   0        0        0     8016 2023-05-23 13:46:40.000000 pyhttpx-2.10.5/pyhttpx/layers/tls/extensions.py
--rw-rw-rw-   0        0        0      123 2022-09-23 08:01:24.000000 pyhttpx-2.10.5/pyhttpx/layers/tls/fields.py
--rw-rw-rw-   0        0        0     1232 2022-10-27 08:35:29.000000 pyhttpx-2.10.5/pyhttpx/layers/tls/handshake.py
--rw-rw-rw-   0        0        0     6750 2023-04-03 08:04:05.000000 pyhttpx-2.10.5/pyhttpx/layers/tls/keyexchange.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:33:21.000000 pyhttpx-2.10.5/pyhttpx/layers/tls/linux/
--rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.5/pyhttpx/layers/tls/linux/__init__.py
--rw-rw-rw-   0        0        0    10351 2023-05-29 10:31:50.000000 pyhttpx-2.10.5/pyhttpx/layers/tls/pyaiossl.py
--rw-rw-rw-   0        0        0    19396 2023-05-23 13:31:03.000000 pyhttpx-2.10.5/pyhttpx/layers/tls/pyssl.py
--rw-rw-rw-   0        0        0     2357 2023-05-17 03:53:54.000000 pyhttpx-2.10.5/pyhttpx/layers/tls/socks.py
--rw-rw-rw-   0        0        0     4513 2022-09-23 08:01:24.000000 pyhttpx-2.10.5/pyhttpx/layers/tls/suites.py
--rw-rw-rw-   0        0        0    19146 2023-05-20 08:13:11.000000 pyhttpx-2.10.5/pyhttpx/layers/tls/tls_context.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:33:21.000000 pyhttpx-2.10.5/pyhttpx/layers/tls/window/
--rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.5/pyhttpx/layers/tls/window/__init__.py
--rw-rw-rw-   0        0        0     9276 2023-05-26 09:23:48.000000 pyhttpx-2.10.5/pyhttpx/models.py
--rw-rw-rw-   0        0        0    16850 2023-05-31 14:32:44.000000 pyhttpx-2.10.5/pyhttpx/session.py
--rw-rw-rw-   0        0        0     1991 2023-05-23 12:56:47.000000 pyhttpx-2.10.5/pyhttpx/utils.py
--rw-rw-rw-   0        0        0     8142 2023-05-30 00:24:03.000000 pyhttpx-2.10.5/pyhttpx/websocket.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:33:21.000000 pyhttpx-2.10.5/pyhttpx.egg-info/
--rw-rw-rw-   0        0        0      339 2023-05-31 14:33:21.000000 pyhttpx-2.10.5/pyhttpx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1248 2023-05-31 14:33:21.000000 pyhttpx-2.10.5/pyhttpx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 14:33:21.000000 pyhttpx-2.10.5/pyhttpx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-08-15 06:28:23.000000 pyhttpx-2.10.5/pyhttpx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       68 2023-05-31 14:33:21.000000 pyhttpx-2.10.5/pyhttpx.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-31 14:33:21.000000 pyhttpx-2.10.5/pyhttpx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 14:33:21.000000 pyhttpx-2.10.5/setup.cfg
--rw-rw-rw-   0        0        0     1576 2023-05-31 14:33:18.000000 pyhttpx-2.10.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:33:21.000000 pyhttpx-2.10.5/tests/
--rw-rw-rw-   0        0        0        0 2022-08-15 03:02:17.000000 pyhttpx-2.10.5/tests/__init__.py
--rw-rw-rw-   0        0        0     1033 2023-05-31 14:30:48.000000 pyhttpx-2.10.5/tests/requestTest.py
--rw-rw-rw-   0        0        0     1707 2023-05-31 14:30:48.000000 pyhttpx-2.10.5/tests/websocketTest.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:45:16.000000 pyhttpx-2.10.6/
+-rw-rw-rw-   0        0        0     1086 2022-08-12 14:37:21.000000 pyhttpx-2.10.6/LICENSE
+-rw-rw-rw-   0        0        0       24 2022-08-15 03:00:31.000000 pyhttpx-2.10.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      339 2023-06-01 08:45:16.000000 pyhttpx-2.10.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2592 2023-05-31 14:45:44.000000 pyhttpx-2.10.6/README.md
+-rw-rw-rw-   0        0        0        0 2022-08-15 02:16:12.000000 pyhttpx-2.10.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-01 08:45:16.000000 pyhttpx-2.10.6/pyhttpx/
+-rw-rw-rw-   0        0        0       81 2022-12-05 09:21:49.000000 pyhttpx-2.10.6/pyhttpx/__init__.py
+-rw-rw-rw-   0        0        0      262 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/__version__.py
+-rw-rw-rw-   0        0        0      106 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/compat.py
+-rw-rw-rw-   0        0        0     1107 2022-12-05 07:47:21.000000 pyhttpx-2.10.6/pyhttpx/exception.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:45:16.000000 pyhttpx-2.10.6/pyhttpx/layers/
+-rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/layers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:45:16.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/
+-rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:45:16.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/
+-rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/__init__.py
+-rw-rw-rw-   0        0        0     2308 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/aes.py
+-rw-rw-rw-   0        0        0     1114 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/chacha20_poly1305.py
+-rw-rw-rw-   0        0        0     4618 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/cipher_aead.py
+-rw-rw-rw-   0        0        0     3910 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/cipher_block.py
+-rw-rw-rw-   0        0        0      266 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/ciphers.py
+-rw-rw-rw-   0        0        0     4293 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/ecc.py
+-rw-rw-rw-   0        0        0     6180 2023-01-31 06:58:53.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/hkdf.py
+-rw-rw-rw-   0        0        0      947 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/kx_algs.py
+-rw-rw-rw-   0        0        0     1771 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/prf.py
+-rw-rw-rw-   0        0        0     8016 2023-05-23 13:46:40.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/extensions.py
+-rw-rw-rw-   0        0        0      123 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/fields.py
+-rw-rw-rw-   0        0        0     1232 2022-10-27 08:35:29.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/handshake.py
+-rw-rw-rw-   0        0        0     6750 2023-04-03 08:04:05.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/keyexchange.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:45:16.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/linux/
+-rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/linux/__init__.py
+-rw-rw-rw-   0        0        0    10351 2023-05-29 10:31:50.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/pyaiossl.py
+-rw-rw-rw-   0        0        0    19396 2023-05-23 13:31:03.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/pyssl.py
+-rw-rw-rw-   0        0        0     2357 2023-05-17 03:53:54.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/socks.py
+-rw-rw-rw-   0        0        0     4513 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/suites.py
+-rw-rw-rw-   0        0        0    19146 2023-05-20 08:13:11.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/tls_context.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:45:16.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/window/
+-rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/window/__init__.py
+-rw-rw-rw-   0        0        0     9335 2023-06-01 08:43:29.000000 pyhttpx-2.10.6/pyhttpx/models.py
+-rw-rw-rw-   0        0        0    16766 2023-06-01 08:44:23.000000 pyhttpx-2.10.6/pyhttpx/session.py
+-rw-rw-rw-   0        0        0     1991 2023-05-23 12:56:47.000000 pyhttpx-2.10.6/pyhttpx/utils.py
+-rw-rw-rw-   0        0        0     8142 2023-05-30 00:24:03.000000 pyhttpx-2.10.6/pyhttpx/websocket.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:45:16.000000 pyhttpx-2.10.6/pyhttpx.egg-info/
+-rw-rw-rw-   0        0        0      339 2023-06-01 08:45:16.000000 pyhttpx-2.10.6/pyhttpx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1248 2023-06-01 08:45:16.000000 pyhttpx-2.10.6/pyhttpx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 08:45:16.000000 pyhttpx-2.10.6/pyhttpx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-08-15 06:28:23.000000 pyhttpx-2.10.6/pyhttpx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       68 2023-06-01 08:45:16.000000 pyhttpx-2.10.6/pyhttpx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-01 08:45:16.000000 pyhttpx-2.10.6/pyhttpx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 08:45:16.000000 pyhttpx-2.10.6/setup.cfg
+-rw-rw-rw-   0        0        0     1576 2023-06-01 08:45:10.000000 pyhttpx-2.10.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:45:16.000000 pyhttpx-2.10.6/tests/
+-rw-rw-rw-   0        0        0        0 2022-08-15 03:02:17.000000 pyhttpx-2.10.6/tests/__init__.py
+-rw-rw-rw-   0        0        0     1007 2023-06-01 08:44:23.000000 pyhttpx-2.10.6/tests/requestTest.py
+-rw-rw-rw-   0        0        0     1707 2023-05-31 14:30:48.000000 pyhttpx-2.10.6/tests/websocketTest.py
```

### Comparing `pyhttpx-2.10.5/LICENSE` & `pyhttpx-2.10.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.5/README.md` & `pyhttpx-2.10.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -19,24 +19,14 @@
 ```
 cryptography==36.0.1
 rsa==4.8
 pyOpenSSL==21.0.0
 
 brotli==1.0.9
 hpack==4.0.0
-
-
-
-
-## HttpSession
-
->>>sess = pyhttpx.HttpSession(browser_type='chrome', http2=True)
->>>r = sess.get('https://tls.peet.ws/api/all')
->>>r.text
-... "ja3": "771,4865-4866...
 ```
 
 ## GET
 ```
 >>> import pyhttpx
 >>> sess = pyhttpx.HttpSession()
 >>> r = sess.get('https://httpbin.org/get',headers={'User-Agent':'3301'},cookies={'k':'3301')
```

### Comparing `pyhttpx-2.10.5/pyhttpx/exception.py` & `pyhttpx-2.10.6/pyhttpx/exception.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.5/pyhttpx/layers/tls/crypto/aes.py` & `pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.5/pyhttpx/layers/tls/crypto/chacha20_poly1305.py` & `pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/chacha20_poly1305.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.5/pyhttpx/layers/tls/crypto/cipher_aead.py` & `pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/cipher_aead.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.5/pyhttpx/layers/tls/crypto/cipher_block.py` & `pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/cipher_block.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.5/pyhttpx/layers/tls/crypto/ecc.py` & `pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/ecc.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.5/pyhttpx/layers/tls/crypto/hkdf.py` & `pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/hkdf.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.5/pyhttpx/layers/tls/crypto/kx_algs.py` & `pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/kx_algs.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.5/pyhttpx/layers/tls/crypto/prf.py` & `pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/prf.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.5/pyhttpx/layers/tls/extensions.py` & `pyhttpx-2.10.6/pyhttpx/layers/tls/extensions.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.5/pyhttpx/layers/tls/handshake.py` & `pyhttpx-2.10.6/pyhttpx/layers/tls/handshake.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.5/pyhttpx/layers/tls/keyexchange.py` & `pyhttpx-2.10.6/pyhttpx/layers/tls/keyexchange.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.5/pyhttpx/layers/tls/pyaiossl.py` & `pyhttpx-2.10.6/pyhttpx/layers/tls/pyaiossl.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.5/pyhttpx/layers/tls/pyssl.py` & `pyhttpx-2.10.6/pyhttpx/layers/tls/pyssl.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.5/pyhttpx/layers/tls/socks.py` & `pyhttpx-2.10.6/pyhttpx/layers/tls/socks.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.5/pyhttpx/layers/tls/suites.py` & `pyhttpx-2.10.6/pyhttpx/layers/tls/suites.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.5/pyhttpx/layers/tls/tls_context.py` & `pyhttpx-2.10.6/pyhttpx/layers/tls/tls_context.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.5/pyhttpx/models.py` & `pyhttpx-2.10.6/pyhttpx/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,38 +225,37 @@
     def flush(self, frame):
 
         head, body = frame[:9],frame[9:]
         self.stream_id = struct.unpack('!I', head[5:9])[0]
         if frame[3] == 1:
             # 头部
             if body[:3] == b'\x3f\xe1\x5f':
-                #
                 i = 3
-
             elif body[:4] == b'?\xe1\xff\x03':
                 i = 4
             else:
                 i= 0
 
             data = self.hpack_decode.decode(body[i:])
-
             for h in data:
                 k,v = h
                 if k == 'set-cookie':
                     self.headers[k].append(v)
                 else:
                     self.headers[k] = v
 
             if self.headers.get('content-length') != None:
                 self.content_length = int(self.headers.get('content-length', 0))
+
             self.status_code = int(self.headers.get(':status', 200))
+            if self.content_length == 0:
+                self.read_ended = True
 
         elif frame[3] == 0:
             self.body += body
-
             if head[4] == 1:
                 self.read_ended = True
 
         elif frame[3] == 4:
             # SETTINGS
             pass
         elif frame[3] == 8:
```

### Comparing `pyhttpx-2.10.5/pyhttpx/session.py` & `pyhttpx-2.10.6/pyhttpx/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,21 +63,21 @@
         self.ja3 = kwargs.get('ja3')
         self.browser_type = kwargs.get('browser_type')
         self.exts_payload = kwargs.get('exts_payload')
 
         self.http2 = kwargs.get('http2')
         self.poolconnections = LifoQueue(maxsize=self.maxsize)
         self.lock = RLock()
-        self.shuffle_protocol = kwargs.get('shuffle_extension_protocol')
+        self.shuffle_proto = kwargs.get('shuffle_extension_protocol')
 
     def _new_conn(self):
 
         context = pyssl.SSLContext(http2=self.http2)
         context.set_payload(self.browser_type, self.ja3, self.exts_payload,
-                            self.shuffle_protocol
+                            self.shuffle_proto
                             )
         conn = context.wrap_socket(
             sock=None,server_hostname=None)
 
         conn.connect(
             (self.req.host,self.req.port),
             timeout=self.req.timeout,
@@ -107,28 +107,28 @@
             )
 
 
 class HttpSession(object):
     def __init__(self, ja3=None,
                  exts_payload=None,
                  browser_type=None,
-                 http2=True ,
+                 http2=False ,
                  ):
         #默认开启http2, 最终协议由服务器协商完成
         self.http2 = http2
         self.tls_session = None
         self.cookie_manger = CookieManger()
         self.browser_type = None
         self.active_addr = None
         self.tlss = {}
         self.browser_type = browser_type or 'chrome'
         self.exts_payload = exts_payload
         self.lock = RLock()
         self.ja3 = ja3
-        self.shuffle_protocol = False
+        self.shuffle_proto = False
         
     def handle_cookie(self, req, set_cookies):
         #
         if not set_cookies:
             return
         c = {}
         if isinstance(set_cookies, str):
@@ -266,15 +266,15 @@
             connpool = HTTPSConnectionPool(request=req,
                                            host=req.host,
                                            port=req.host,
                                            ja3=self.ja3,
                                            exts_payload=self.exts_payload,
                                            browser_type = self.browser_type,
                                            http2 = self.http2,
-                                           shuffle_extension_protocol =self.shuffle_protocol
+                                           shuffle_extension_protocol =self.shuffle_proto
 
                                            )
 
 
             # 代理连接池没有实现,如果使用代理,会导致使用同一个代理ip连接
             # http2 存在bug
             # closed
@@ -391,15 +391,15 @@
             weight,
             request_msg
         ])
         #update = b'\x00\x00\x04\x08\x00' + struct.pack('!I', self.stream_id) + b'\x00\xbe\x00\x00'
 
         if self.first_load or 1==1:
             self.conn.sendall(self.settings)
-            #self.conn.sendall(update)
+
 
         self.conn.sendall(stream_header)
         if req.method == 'POST':
             size = 2 ** 12
             while req_body:
                 block = req_body[:size]
                 req_body = req_body[size:]
@@ -415,14 +415,15 @@
                 ])
                 self.conn.sendall(stream_data)
 
         response = Http2Response()
         cache = b''
         self.first_load = False
         while 1:
+
             r = self.conn.recv()
             if not r:
                 self.conn.isclosed = True
                 break
 
             cache += r
             while cache:
@@ -436,15 +437,15 @@
                             # goway
                             # conn.sendall(bytes.fromhex('0000080700000000000000000000000000'))
                             pass
                         elif frame[3] == 4:
                             # setting
                             if frame[4] == 1:
                                 self.conn.sendall(bytes.fromhex('000000040100000000'))
-                                pass
+
 
                         elif frame[3] == 6:
                             pass
 
                         elif frame[3] == 8:
                             pass
                     else:
```

### Comparing `pyhttpx-2.10.5/pyhttpx/utils.py` & `pyhttpx-2.10.6/pyhttpx/utils.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.5/pyhttpx/websocket.py` & `pyhttpx-2.10.6/pyhttpx/websocket.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.5/pyhttpx.egg-info/SOURCES.txt` & `pyhttpx-2.10.6/pyhttpx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.5/setup.py` & `pyhttpx-2.10.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         sys.exit(errno)
 
 
 
 packages = find_packages()
 setup(
     name = "pyhttpx",
-    version = "2.10.5",
+    version = "2.10.6",
     keywords = ["pip", "pyhttpx"],
     description = "HTTP library.",
     long_description = "HTTP library, TLS supported version：tls1.2/tls1.3, HTTP supported version: http1.1/http2",
     license = "MIT Licence",
 
     url = "https://github.com/zero3301/pyhttpx",
     author = "3301",
```

### Comparing `pyhttpx-2.10.5/tests/requestTest.py` & `pyhttpx-2.10.6/tests/requestTest.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 import pyhttpx
 import time
 import json
 from pprint import pprint as pp
 import time
 import random
 import os
-import concurrent
-import threading
 import requests
-
+import aiohttp
+import asyncio
 headers={
 'Host': '*',
 'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36',
 'Pragma': 'no-cache',
 'Cache-Control': 'no-cache',
 'sec-ch-ua-platform': '"Windows"',
 'sec-ch-ua-mobile': '?0',
@@ -25,34 +24,34 @@
 'Accept-Encoding': 'gzip, deflate, br',
 'Accept-Language': 'zh,zh-CN;q=0.9,en;q=0.8',
 
 }
 
 
 def main():
-    sess = pyhttpx.HttpSession()
+    sess = pyhttpx.HttpSession(browser_type='chrome')
 
     url='https://tls.peet.ws/api/all'
     #url = 'https://httpbin.org/ip'
     proxies = {
         'https': 'http://username:password@host:port'
     }
-    r = sess.get(url,headers=headers)
-    print(r.status_code)
+    r = sess.get(url)
     print(r.text)
 
 if __name__ == '__main__':
     main()
 
 
 
 
 
 
 
+
```

### Comparing `pyhttpx-2.10.5/tests/websocketTest.py` & `pyhttpx-2.10.6/tests/websocketTest.py`

 * *Files identical despite different names*

