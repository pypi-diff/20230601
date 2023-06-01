# Comparing `tmp/vysion-1.0.4.tar.gz` & `tmp/vysion-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vysion-1.0.4.tar", max compression
+gzip compressed data, was "vysion-1.0.5.tar", max compression
```

## Comparing `vysion-1.0.4.tar` & `vysion-1.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    11356 2023-04-12 11:01:34.010455 vysion-1.0.4/LICENSE
--rw-r--r--   0        0        0     1976 2023-04-12 11:01:34.010455 vysion-1.0.4/README.md
--rw-r--r--   0        0        0      977 2023-04-12 11:34:08.041449 vysion-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      704 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/__init__.py
--rw-r--r--   0        0        0      630 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/client/__init__.py
--rw-r--r--   0        0        0    10354 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/client/client.py
--rw-r--r--   0        0        0     1176 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/client/error.py
--rw-r--r--   0        0        0      605 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/dto/__init__.py
--rw-r--r--   0        0        0     6809 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/dto/dto.py
--rw-r--r--   0        0        0     1441 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/dto/tag.py
--rw-r--r--   0        0        0     4169 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/dto/util.py
--rw-r--r--   0        0        0      627 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/model/__init__.py
--rw-r--r--   0        0        0      690 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/model/enum/__init__.py
--rw-r--r--   0        0        0     4206 2023-04-12 11:11:50.831436 vysion-1.0.4/vysion/model/enum/languages.py
--rw-r--r--   0        0        0      789 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/model/enum/networks.py
--rw-r--r--   0        0        0     1527 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/model/enum/ransom_groups.py
--rw-r--r--   0        0        0     5569 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/model/enum/services.py
--rw-r--r--   0        0        0     4961 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/model/model.py
--rw-r--r--   0        0        0      635 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/taxonomy/__init__.py
--rw-r--r--   0        0        0     2347 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/taxonomy/flavours.py
--rw-r--r--   0        0        0    12263 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/taxonomy/taxonomy.py
--rw-r--r--   0        0        0      610 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/version.py
--rw-r--r--   0        0        0     3011 1970-01-01 00:00:00.000000 vysion-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-04-12 11:01:34.010455 vysion-1.0.5/LICENSE
+-rw-r--r--   0        0        0     1049 2023-06-01 14:40:26.070285 vysion-1.0.5/README.md
+-rw-r--r--   0        0        0      977 2023-06-01 14:51:52.160926 vysion-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      664 2023-06-01 14:40:26.070285 vysion-1.0.5/vysion/__init__.py
+-rw-r--r--   0        0        0      630 2023-06-01 14:40:26.070285 vysion-1.0.5/vysion/client/__init__.py
+-rw-r--r--   0        0        0     8867 2023-06-01 14:40:26.070285 vysion-1.0.5/vysion/client/client.py
+-rw-r--r--   0        0        0     1176 2023-04-12 11:01:34.010455 vysion-1.0.5/vysion/client/error.py
+-rw-r--r--   0        0        0      605 2023-04-12 11:01:34.010455 vysion-1.0.5/vysion/dto/__init__.py
+-rw-r--r--   0        0        0     6776 2023-06-01 14:40:26.070285 vysion-1.0.5/vysion/dto/dto.py
+-rw-r--r--   0        0        0     1442 2023-06-01 14:40:26.070285 vysion-1.0.5/vysion/dto/tag.py
+-rw-r--r--   0        0        0     4170 2023-06-01 14:40:26.070285 vysion-1.0.5/vysion/dto/util.py
+-rw-r--r--   0        0        0      627 2023-06-01 14:40:26.070285 vysion-1.0.5/vysion/model/__init__.py
+-rw-r--r--   0        0        0      690 2023-06-01 14:40:26.070285 vysion-1.0.5/vysion/model/enum/__init__.py
+-rw-r--r--   0        0        0     4206 2023-04-12 11:11:50.831436 vysion-1.0.5/vysion/model/enum/languages.py
+-rw-r--r--   0        0        0      789 2023-04-12 11:01:34.010455 vysion-1.0.5/vysion/model/enum/networks.py
+-rw-r--r--   0        0        0     1527 2023-04-12 11:01:34.010455 vysion-1.0.5/vysion/model/enum/ransom_groups.py
+-rw-r--r--   0        0        0     5569 2023-04-12 11:01:34.010455 vysion-1.0.5/vysion/model/enum/services.py
+-rw-r--r--   0        0        0     4962 2023-06-01 14:40:26.070285 vysion-1.0.5/vysion/model/model.py
+-rw-r--r--   0        0        0      635 2023-06-01 14:40:26.070285 vysion-1.0.5/vysion/taxonomy/__init__.py
+-rw-r--r--   0        0        0     2347 2023-04-12 11:01:34.010455 vysion-1.0.5/vysion/taxonomy/flavours.py
+-rw-r--r--   0        0        0    12275 2023-06-01 14:40:26.070285 vysion-1.0.5/vysion/taxonomy/taxonomy.py
+-rw-r--r--   0        0        0      610 2023-04-12 11:01:34.010455 vysion-1.0.5/vysion/version.py
+-rw-r--r--   0        0        0     2084 1970-01-01 00:00:00.000000 vysion-1.0.5/PKG-INFO
```

### Comparing `vysion-1.0.4/LICENSE` & `vysion-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vysion-1.0.4/pyproject.toml` & `vysion-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vysion"
-version = "1.0.4"
+version = "1.0.5"
 description = "The official Python client library for Vysion"
 homepage = "https://vysion.ai"
 repository = "https://gitlab.com/byronlabs/vysion/vysion-py"
 documentation = "https://developers.vysion.ai"
 authors = [
   "Javier Junquera-Sánchez <javier.junquera@byronlabs.io>"
 ]
```

### Comparing `vysion-1.0.4/vysion/__init__.py` & `vysion-1.0.5/vysion/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,13 +11,9 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from . import client
-from . import taxonomy
-from . import model
-from . import dto
-
+from . import client, dto, model, taxonomy
 from .version import __version__
```

### Comparing `vysion-1.0.4/vysion/client/__init__.py` & `vysion-1.0.5/vysion/client/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -11,9 +11,9 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from .client import *
 from . import error
+from .client import *
```

### Comparing `vysion-1.0.4/vysion/client/error.py` & `vysion-1.0.5/vysion/client/error.py`

 * *Files identical despite different names*

### Comparing `vysion-1.0.4/vysion/dto/__init__.py` & `vysion-1.0.5/vysion/dto/__init__.py`

 * *Files identical despite different names*

### Comparing `vysion-1.0.4/vysion/dto/dto.py` & `vysion-1.0.5/vysion/dto/dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,37 +10,36 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from enum import Enum
 import hashlib
-
 from datetime import datetime
-from vysion.model import enum
+from enum import Enum
 
+from vysion.model import enum
 from vysion.taxonomy import Monero_Address, Ripple_Address
 
 try:
     from types import NoneType
 except:
     NoneType: type = type(None)
 
 from typing import List, Optional, Union
 from urllib.parse import urlparse
 
-from pydantic import BaseModel, Field # , constr
-from .tag import *
+from pydantic import BaseModel, Field  # , constr
 
-from urllib.parse import urlparse
 from vysion import taxonomy as vystaxonomy
 from vysion.model import URL as URL_model
-from vysion.model.enum import Services, Network, Language, RansomGroup
+from vysion.model.enum import Language, Network, RansomGroup, Services
+
+from .tag import *
 
 
 class Email(BaseModel):
 
     _taxonomy = [vystaxonomy.Email]
 
     # RFC 5322 Official Standard (https://www.emailregex.com/)
```

### Comparing `vysion-1.0.4/vysion/dto/tag.py` & `vysion-1.0.5/vysion/dto/tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
+import re
+from typing import Optional
+
 from pydantic import BaseModel
 from softenum import Softenum
-from typing import Optional
-import re
 
 '''
 https://github.com/MISP/misp-taxonomies
 '''
 
 
 class Namespace(str, Softenum):
```

### Comparing `vysion-1.0.4/vysion/dto/util.py` & `vysion-1.0.5/vysion/dto/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,23 +11,24 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import json
+
 from pymisp import MISPAttribute, MISPEvent, MISPObject, MISPTag
 
 try:
     from types import NoneType
 except:
     NoneType = type(None)
 
 import vysion.dto as dto
-from vysion.dto import Hit, RansomFeedHit, Page, URL
+from vysion.dto import URL, Hit, Page, RansomFeedHit
 
 
 class MISPProcessor:
 
     def __init__(self):
         self.misp_event = MISPEvent()
```

### Comparing `vysion-1.0.4/vysion/model/__init__.py` & `vysion-1.0.5/vysion/model/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -10,9 +10,9 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from .model import *
 from . import enum
+from .model import *
```

### Comparing `vysion-1.0.4/vysion/model/enum/__init__.py` & `vysion-1.0.5/vysion/model/enum/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from .languages import *
-from .services import *
 from .networks import *
 from .ransom_groups import *
+from .services import *
```

### Comparing `vysion-1.0.4/vysion/model/enum/languages.py` & `vysion-1.0.5/vysion/model/enum/languages.py`

 * *Files identical despite different names*

### Comparing `vysion-1.0.4/vysion/model/enum/networks.py` & `vysion-1.0.5/vysion/model/enum/networks.py`

 * *Files identical despite different names*

### Comparing `vysion-1.0.4/vysion/model/enum/ransom_groups.py` & `vysion-1.0.5/vysion/model/enum/ransom_groups.py`

 * *Files identical despite different names*

### Comparing `vysion-1.0.4/vysion/model/enum/services.py` & `vysion-1.0.5/vysion/model/enum/services.py`

 * *Files identical despite different names*

### Comparing `vysion-1.0.4/vysion/model/model.py` & `vysion-1.0.5/vysion/model/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,31 +10,31 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from .enum import Enum
 import hashlib
 import uuid
 from datetime import datetime
 
+from .enum import Enum
+
 try:
     from types import NoneType
 except:
     NoneType: type = type(None)
 
+import re
 from typing import List, Optional, Union
 
-from pydantic import BaseModel, Field # , constr
-
-from .enum import Services, Network
+from pydantic import BaseModel, Field  # , constr
 
-import re
+from .enum import Network, Services
 
 NULL_UUID = uuid.UUID("00000000-0000-0000-0000-000000000000")
 
 class URL(BaseModel):
 
     protocol: Optional[str] 
     domain: Optional[str]
```

### Comparing `vysion-1.0.4/vysion/taxonomy/__init__.py` & `vysion-1.0.5/vysion/taxonomy/__init__.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -11,9 +11,9 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from .taxonomy import *
 from . import flavours
+from .taxonomy import *
```

### Comparing `vysion-1.0.4/vysion/taxonomy/flavours.py` & `vysion-1.0.5/vysion/taxonomy/flavours.py`

 * *Files identical despite different names*

### Comparing `vysion-1.0.4/vysion/taxonomy/taxonomy.py` & `vysion-1.0.5/vysion/taxonomy/taxonomy.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,22 +11,17 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 from typing import Dict
-from vysion.taxonomy.flavours import (
-    Flavour,
-    Flavours,
-    EmptyFlavour,
-    DBSafe,
-    MISP,
-    Vysion,
-)
+
+from vysion.taxonomy.flavours import (MISP, DBSafe, EmptyFlavour, Flavour,
+                                      Flavours, Vysion)
 
 """
     
     # Vysion taxonomy 1.0
 
     Siguiendo metodología de MISP:
```

### Comparing `vysion-1.0.4/vysion/version.py` & `vysion-1.0.5/vysion/version.py`

 * *Files identical despite different names*

### Comparing `vysion-1.0.4/PKG-INFO` & `vysion-1.0.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vysion
-Version: 1.0.4
+Version: 1.0.5
 Summary: The official Python client library for Vysion
 Home-page: https://vysion.ai
 License: Apache-2.0
 Author: Javier Junquera-Sánchez
 Author-email: javier.junquera@byronlabs.io
 Requires-Python: >=3.7.0,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -45,45 +45,20 @@
 ### Taxonomy
 
 - https://github.com/MISP/misp-taxonomies/blob/main/tools/machinetag.py
 - https://www.misp-project.org/taxonomies.html#_mapping_of_taxonomies
 - https://github.com/MISP/misp-taxonomies
 - https://github.com/MISP/misp-taxonomies/blob/main/tools/docs/images/taxonomy-explanation.png
 
-## Entorno
+## Development
 
 - vs-code
-    - Extensiones:
+    - Extensions:
         - snyk
         - flake8
+        - isort 
 
-## The Zen of Python
-
-```python
-import this
-> The Zen of Python, by Tim Peters
-> 
-> Beautiful is better than ugly.
-> Explicit is better than implicit.
-> Simple is better than complex.
-> Complex is better than complicated.
-> Flat is better than nested.
-> Sparse is better than dense.
-> Readability counts.
-> Special cases aren't special enough to break the rules.
-> Although practicality beats purity.
-> Errors should never pass silently.
-> Unless explicitly silenced.
-> In the face of ambiguity, refuse the temptation to guess.
-> There should be one-- and preferably only one --obvious way to do it.
-> Although that way may not be obvious at first unless you're Dutch.
-> Now is better than never.
-> Although never is often better than *right* now.
-> If the implementation is hard to explain, it's a bad idea.
-> If the implementation is easy to explain, it may be a good idea.
-> Namespaces are one honking great idea -- let's do more of those!
-```
 
 # Ackowledgement
 
 We really appreciate the documentation of https://github.com/VirusTotal/vt-py
```

