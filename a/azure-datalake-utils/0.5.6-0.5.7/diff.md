# Comparing `tmp/azure_datalake_utils-0.5.6.tar.gz` & `tmp/azure_datalake_utils-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure_datalake_utils-0.5.6.tar", max compression
+gzip compressed data, was "azure_datalake_utils-0.5.7.tar", max compression
```

## Comparing `azure_datalake_utils-0.5.6.tar` & `azure_datalake_utils-0.5.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-05-16 11:19:41.153928 azure_datalake_utils-0.5.6/LICENSE
--rw-r--r--   0        0        0     2311 2023-05-16 11:19:41.153928 azure_datalake_utils-0.5.6/README.md
--rw-r--r--   0        0        0      297 2023-05-16 11:19:41.153928 azure_datalake_utils-0.5.6/azure_datalake_utils/__init__.py
--rw-r--r--   0        0        0    13240 2023-05-16 11:19:41.153928 azure_datalake_utils-0.5.6/azure_datalake_utils/azure_datalake_utils.py
--rw-r--r--   0        0        0     2171 2023-05-16 11:19:41.153928 azure_datalake_utils-0.5.6/azure_datalake_utils/exepctions.py
--rw-r--r--   0        0        0     1685 2023-05-16 11:19:41.153928 azure_datalake_utils-0.5.6/azure_datalake_utils/experimental.py
--rw-r--r--   0        0        0     8728 2023-05-16 11:19:41.153928 azure_datalake_utils-0.5.6/azure_datalake_utils/partitions.py
--rw-r--r--   0        0        0     3106 2023-05-16 11:19:41.157928 azure_datalake_utils-0.5.6/pyproject.toml
--rw-r--r--   0        0        0       50 2023-05-16 11:19:41.157928 azure_datalake_utils-0.5.6/tests/__init__.py
--rw-r--r--   0        0        0     8892 2023-05-16 11:19:41.157928 azure_datalake_utils-0.5.6/tests/test_azure_datalake_utils.py
--rw-r--r--   0        0        0      561 2023-05-16 11:19:41.157928 azure_datalake_utils-0.5.6/tests/test_azure_exepctions.py
--rw-r--r--   0        0        0    13027 2023-05-16 11:19:41.157928 azure_datalake_utils-0.5.6/tests/test_partitions.py
--rw-r--r--   0        0        0     4899 1970-01-01 00:00:00.000000 azure_datalake_utils-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-01 16:01:20.139632 azure_datalake_utils-0.5.7/LICENSE
+-rw-r--r--   0        0        0     2311 2023-06-01 16:01:20.139632 azure_datalake_utils-0.5.7/README.md
+-rw-r--r--   0        0        0      297 2023-06-01 16:01:20.139632 azure_datalake_utils-0.5.7/azure_datalake_utils/__init__.py
+-rw-r--r--   0        0        0    13082 2023-06-01 16:01:20.139632 azure_datalake_utils-0.5.7/azure_datalake_utils/azure_datalake_utils.py
+-rw-r--r--   0        0        0     2171 2023-06-01 16:01:20.139632 azure_datalake_utils-0.5.7/azure_datalake_utils/exepctions.py
+-rw-r--r--   0        0        0     2475 2023-06-01 16:01:20.139632 azure_datalake_utils-0.5.7/azure_datalake_utils/experimental.py
+-rw-r--r--   0        0        0     8728 2023-06-01 16:01:20.139632 azure_datalake_utils-0.5.7/azure_datalake_utils/partitions.py
+-rw-r--r--   0        0        0     3106 2023-06-01 16:01:20.143632 azure_datalake_utils-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-06-01 16:01:20.143632 azure_datalake_utils-0.5.7/tests/__init__.py
+-rw-r--r--   0        0        0     8901 2023-06-01 16:01:20.143632 azure_datalake_utils-0.5.7/tests/test_azure_datalake_utils.py
+-rw-r--r--   0        0        0      561 2023-06-01 16:01:20.143632 azure_datalake_utils-0.5.7/tests/test_azure_exepctions.py
+-rw-r--r--   0        0        0    13027 2023-06-01 16:01:20.143632 azure_datalake_utils-0.5.7/tests/test_partitions.py
+-rw-r--r--   0        0        0     4700 1970-01-01 00:00:00.000000 azure_datalake_utils-0.5.7/PKG-INFO
```

### Comparing `azure_datalake_utils-0.5.6/LICENSE` & `azure_datalake_utils-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `azure_datalake_utils-0.5.6/README.md` & `azure_datalake_utils-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `azure_datalake_utils-0.5.6/azure_datalake_utils/azure_datalake_utils.py` & `azure_datalake_utils-0.5.7/azure_datalake_utils/azure_datalake_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """Main module."""
 import platform
 import re
-from typing import Any, Dict, Optional, Union, List
+from typing import Any, Dict, List, Optional, Union
 
 import numpy as np
 import pandas as pd
-import azure_datalake_utils.experimental as exp
-
-from azure.identity import InteractiveBrowserCredential
-from azure.identity.aio import DefaultAzureCredential as AIODefaultAzureCredential
 from adlfs import AzureBlobFileSystem
+from azure.identity import InteractiveBrowserCredential
+
+import azure_datalake_utils.experimental as exp
 from azure_datalake_utils.exepctions import ExtensionIncorrecta, raiseArchivoNoEncontrado
 from azure_datalake_utils.partitions import HivePartitiion
 
 
 class Datalake(object):
     """Clase para representar operaciones de Datalake."""
 
@@ -38,26 +37,24 @@
                 - https://github.com/fsspec/adlfs/issues/391
                 - https://github.com/Azure/azure-sdk-for-python/issues/28312
         """
         self.datalake_name = datalake_name
 
         if account_key is None:
             self.tenant_id = tenant_id
-            credentials = InteractiveBrowserCredential(tenant_id=self.tenant_id)
-            credentials.authenticate()
-            self._credentials = credentials
+            credential = exp.AioCredentialWrapper(InteractiveBrowserCredential(tenant_id=self.tenant_id))
             # TODO: verificar https://github.com/fsspec/adlfs/issues/270
             # para ver como evoluciona y evitar este condicional.
             if platform.system().lower() != 'windows':
                 storage_options = {'account_name': self.datalake_name, 'anon': False}
             else:
                 storage_options = {
                     'account_name': self.datalake_name,
                     'anon': False,
-                    'credential': AIODefaultAzureCredential(),
+                    'credential': credential,
                 }
 
         else:
             storage_options = {'account_name': self.datalake_name, 'account_key': account_key}
             self.fs = AzureBlobFileSystem(account_name=self.datalake_name, account_key=account_key)
 
         if not fsspec_cache:
```

### Comparing `azure_datalake_utils-0.5.6/azure_datalake_utils/exepctions.py` & `azure_datalake_utils-0.5.7/azure_datalake_utils/exepctions.py`

 * *Files identical despite different names*

### Comparing `azure_datalake_utils-0.5.6/azure_datalake_utils/partitions.py` & `azure_datalake_utils-0.5.7/azure_datalake_utils/partitions.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 import itertools
 import logging
-
 from typing import Dict, List, Tuple
+
 from adlfs import AzureBlobFileSystem
 
 
 class HivePartitiion:
     """Clase para tratar con la particiones tipo hive.
 
     Una partición tipo hive son archivos que son almacenados de la forma
```

### Comparing `azure_datalake_utils-0.5.6/pyproject.toml` & `azure_datalake_utils-0.5.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "azure_datalake_utils"
-version = "0.5.6"
+version = "0.5.7"
 homepage = "https://github.com/centraal-api/azure-datalake-utils"
 description = "Utilidades para interactuar con Azure Datalake."
 authors = ["centraal.studio <equipo@centraal.studio>"]
 readme = "README.md"
 license =  "Apache-2.0"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `azure_datalake_utils-0.5.6/tests/test_azure_datalake_utils.py` & `azure_datalake_utils-0.5.7/tests/test_azure_datalake_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 # under the License.
 import platform
 from unittest.mock import Mock, patch
 
 import pandas as pd
 import pytest
 from azure.identity import AuthenticationRecord
-from azure.identity.aio import DefaultAzureCredential
 from azure.core.exceptions import ResourceNotFoundError
 from adlfs import AzureBlobFileSystem
 
 from azure_datalake_utils import Datalake
 from azure_datalake_utils.exepctions import ExtensionIncorrecta
+from azure_datalake_utils.experimental import AioCredentialWrapper
 
 fake_record = AuthenticationRecord("tenant-id", "client-id", "localhost", "object.tenant", "username")
 
 
 @pytest.fixture
 def dl_account() -> Datalake:
     """DL instancia incilizada."""
@@ -54,15 +54,15 @@
     with patch('azure.identity.InteractiveBrowserCredential.authenticate', return_value=fake_record):
         dl = Datalake('name', 'tenant')
         if platform.system().lower() != 'windows':
             assert dl.storage_options == {'account_name': 'name', 'anon': False}
         else:
             assert dl.storage_options['account_name'] == 'name'
             assert not dl.storage_options['anon']
-            assert isinstance(dl.storage_options['credential'], DefaultAzureCredential)
+            assert isinstance(dl.storage_options['credential'], AioCredentialWrapper)
 
     with patch('azure.identity.InteractiveBrowserCredential.authenticate', return_value=fake_record):
         dl = Datalake('name', 'tenant', fsspec_cache=False)
         if platform.system().lower() != 'windows':
             assert dl.storage_options == {
                 'account_name': 'name',
                 'anon': False,
@@ -70,15 +70,15 @@
                 'default_fill_cache': False,
                 'skip_instance_cache': True,
             }
         else:
             assert dl.storage_options['account_name'] == 'name'
             assert dl.storage_options['default_cache_type'] is None, "no se esta invalidando el cache."
             assert not dl.storage_options['anon']
-            assert isinstance(dl.storage_options['credential'], DefaultAzureCredential)
+            assert isinstance(dl.storage_options['credential'], AioCredentialWrapper)
 
 
 def test_datalake_should_init_from_account_key():
     """Test para inicializacion del datalake con key account."""
     dl = Datalake.from_account_key('name', 'key')
     assert dl.storage_options == {'account_name': 'name', 'account_key': 'key'}
```

### Comparing `azure_datalake_utils-0.5.6/tests/test_azure_exepctions.py` & `azure_datalake_utils-0.5.7/tests/test_azure_exepctions.py`

 * *Files identical despite different names*

### Comparing `azure_datalake_utils-0.5.6/tests/test_partitions.py` & `azure_datalake_utils-0.5.7/tests/test_partitions.py`

 * *Files identical despite different names*

### Comparing `azure_datalake_utils-0.5.6/PKG-INFO` & `azure_datalake_utils-0.5.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-datalake-utils
-Version: 0.5.6
+Version: 0.5.7
 Summary: Utilidades para interactuar con Azure Datalake.
 Home-page: https://github.com/centraal-api/azure-datalake-utils
 License: Apache-2.0
 Author: centraal.studio
 Author-email: equipo@centraal.studio
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -12,18 +12,14 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
 Requires-Dist: Jinja2 (>=2.11.1,<3.0) ; extra == "test"
 Requires-Dist: adlfs (<=2022.11.2)
 Requires-Dist: azure-identity (>=1.10.0,<2.0.0)
 Requires-Dist: black (>=22.3.0,<23.0.0) ; extra == "test"
```

