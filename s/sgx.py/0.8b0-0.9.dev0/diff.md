# Comparing `tmp/sgx.py-0.8b0.tar.gz` & `tmp/sgx.py-0.9.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sgx.py-0.8b0.tar", last modified: Thu Feb 10 14:00:36 2022, max compression
+gzip compressed data, was "sgx.py-0.9.dev0.tar", last modified: Thu Jun  1 18:59:10 2023, max compression
```

## Comparing `sgx.py-0.8b0.tar` & `sgx.py-0.9.dev0.tar`

### file list

```diff
@@ -1,20 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-10 14:00:36.000000 sgx.py-0.8b0/
--rw-r--r--   0 runner    (1001) docker     (116)      292 2022-02-10 14:00:36.000000 sgx.py-0.8b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      298 2022-02-10 13:59:24.000000 sgx.py-0.8b0/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-02-10 14:00:36.000000 sgx.py-0.8b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      868 2022-02-10 14:00:36.000000 sgx.py-0.8b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-10 14:00:36.000000 sgx.py-0.8b0/sgx/
--rw-r--r--   0 runner    (1001) docker     (116)       51 2022-02-10 13:59:24.000000 sgx.py-0.8b0/sgx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      223 2022-02-10 13:59:24.000000 sgx.py-0.8b0/sgx/constants.py
--rw-r--r--   0 runner    (1001) docker     (116)       80 2022-02-10 13:59:24.000000 sgx.py-0.8b0/sgx/generate.sh
--rw-r--r--   0 runner    (1001) docker     (116)     3500 2022-02-10 13:59:24.000000 sgx.py-0.8b0/sgx/http.py
--rw-r--r--   0 runner    (1001) docker     (116)     9341 2022-02-10 13:59:24.000000 sgx.py-0.8b0/sgx/sgx.py
--rw-r--r--   0 runner    (1001) docker     (116)     9394 2022-02-10 13:59:24.000000 sgx.py-0.8b0/sgx/sgx_rpc_handler.py
--rw-r--r--   0 runner    (1001) docker     (116)    11605 2022-02-10 13:59:24.000000 sgx.py-0.8b0/sgx/sgx_zmq.py
--rw-r--r--   0 runner    (1001) docker     (116)     2116 2022-02-10 13:59:24.000000 sgx.py-0.8b0/sgx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-10 14:00:36.000000 sgx.py-0.8b0/sgx.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      292 2022-02-10 14:00:36.000000 sgx.py-0.8b0/sgx.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      290 2022-02-10 14:00:36.000000 sgx.py-0.8b0/sgx.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-02-10 14:00:36.000000 sgx.py-0.8b0/sgx.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      199 2022-02-10 14:00:36.000000 sgx.py-0.8b0/sgx.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        4 2022-02-10 14:00:36.000000 sgx.py-0.8b0/sgx.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:59:10.477043 sgx.py-0.9.dev0/
+-rw-r--r--   0 runner    (1001) docker     (122)    34522 2023-06-01 18:57:38.000000 sgx.py-0.9.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      261 2023-06-01 18:59:10.477043 sgx.py-0.9.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      298 2023-06-01 18:57:38.000000 sgx.py-0.9.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-01 18:59:10.477043 sgx.py-0.9.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      867 2023-06-01 18:59:10.000000 sgx.py-0.9.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:59:10.477043 sgx.py-0.9.dev0/sgx/
+-rw-r--r--   0 runner    (1001) docker     (122)       51 2023-06-01 18:57:38.000000 sgx.py-0.9.dev0/sgx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-06-01 18:57:38.000000 sgx.py-0.9.dev0/sgx/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-06-01 18:57:38.000000 sgx.py-0.9.dev0/sgx/generate.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     3500 2023-06-01 18:57:38.000000 sgx.py-0.9.dev0/sgx/http.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9345 2023-06-01 18:57:38.000000 sgx.py-0.9.dev0/sgx/sgx.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9394 2023-06-01 18:57:38.000000 sgx.py-0.9.dev0/sgx/sgx_rpc_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11656 2023-06-01 18:57:38.000000 sgx.py-0.9.dev0/sgx/sgx_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2121 2023-06-01 18:57:38.000000 sgx.py-0.9.dev0/sgx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:59:10.477043 sgx.py-0.9.dev0/sgx.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      261 2023-06-01 18:59:10.000000 sgx.py-0.9.dev0/sgx.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-06-01 18:59:10.000000 sgx.py-0.9.dev0/sgx.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 18:59:10.000000 sgx.py-0.9.dev0/sgx.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      195 2023-06-01 18:59:10.000000 sgx.py-0.9.dev0/sgx.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        4 2023-06-01 18:59:10.000000 sgx.py-0.9.dev0/sgx.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:59:10.477043 sgx.py-0.9.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     6282 2023-06-01 18:57:38.000000 sgx.py-0.9.dev0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13957 2023-06-01 18:57:38.000000 sgx.py-0.9.dev0/tests/test_dkg.py
+-rw-r--r--   0 runner    (1001) docker     (122)      849 2023-06-01 18:57:38.000000 sgx.py-0.9.dev0/tests/test_http.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sgx.py-0.8b0/sgx/http.py` & `sgx.py-0.9.dev0/sgx/http.py`

 * *Files identical despite different names*

### Comparing `sgx.py-0.8b0/sgx/sgx.py` & `sgx.py-0.9.dev0/sgx/sgx.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #     GNU Affero General Public License for more details.
 #
 #     You should have received a copy of the GNU Affero General Public License
 #     along with sgx.py.  If not, see <https://www.gnu.org/licenses/>.
 
 import logging
 from dataclasses import dataclass
-from collections import Mapping
+from collections.abc import Mapping
 from hexbytes import HexBytes
 from eth_account.datastructures import SignedTransaction, SignedMessage
 from eth_utils.curried import keccak
 from cytoolz import dissoc
 from sgx.sgx_rpc_handler import SgxRPCHandler
 from sgx.sgx_zmq import SgxZmq
 from sgx.utils import public_key_to_address
```

### Comparing `sgx.py-0.8b0/sgx/sgx_rpc_handler.py` & `sgx.py-0.9.dev0/sgx/sgx_rpc_handler.py`

 * *Files identical despite different names*

### Comparing `sgx.py-0.8b0/sgx/sgx_zmq.py` & `sgx.py-0.9.dev0/sgx/sgx_zmq.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,14 +253,16 @@
         params['n'] = self.n
         response = self.__send_request("blsSignMessageHash", params)
         result = response["signatureShare"]
 
         return result
 
     def __send_request(self, method, params=None):
+        if not params:
+            params = dict()
         params["type"] = self.method_to_type[method]
         if self.path_to_cert:
             params["cert"] = self.cert
             msgSig = self.__sign_msg(params)
             params["msgSig"] = msgSig
         msg = json.dumps(params, separators=(',', ':'))
         p_id = os.getpid()
```

### Comparing `sgx.py-0.8b0/sgx/utils.py` & `sgx.py-0.9.dev0/sgx/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,9 +65,9 @@
         logger.error('Error during shell execution:')
         logger.error(res.stderr.decode('UTF-8').rstrip())
         raise subprocess.CalledProcessError(res.returncode, cmd)
     return res
 
 
 def public_key_to_address(pk):
-    hash_ = Web3.sha3(hexstr=str(pk))
-    return Web3.toChecksumAddress(Web3.toHex(hash_[-20:]))
+    hash_ = Web3.keccak(hexstr=str(pk))
+    return Web3.to_checksum_address(Web3.to_hex(hash_[-20:]))
```

