# Comparing `tmp/dapr-ext-workflow-0.0.1rc1.tar.gz` & `tmp/dapr-ext-workflow-0.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dapr-ext-workflow-0.0.1rc1.tar", last modified: Wed Apr 19 22:47:03 2023, max compression
+gzip compressed data, was "dist/dapr-ext-workflow-0.1.0rc1.tar", last modified: Thu Jun  1 16:51:50 2023, max compression
```

## Comparing `dapr-ext-workflow-0.0.1rc1.tar` & `dapr-ext-workflow-0.1.0rc1.tar`

### file list

```diff
@@ -1,17 +1,24 @@
-drwxr-xr-x   0 bverst     (501) staff       (20)        0 2023-04-19 22:47:03.000000 dapr-ext-workflow-0.0.1rc1/
--rw-r--r--   0 bverst     (501) staff       (20)    11377 2023-04-19 22:17:57.000000 dapr-ext-workflow-0.0.1rc1/LICENSE
--rw-r--r--   0 bverst     (501) staff       (20)     1596 2023-04-19 22:47:03.000000 dapr-ext-workflow-0.0.1rc1/PKG-INFO
--rw-r--r--   0 bverst     (501) staff       (20)      435 2023-04-19 22:31:52.000000 dapr-ext-workflow-0.0.1rc1/README.rst
-drwxr-xr-x   0 bverst     (501) staff       (20)        0 2023-04-19 22:47:03.000000 dapr-ext-workflow-0.0.1rc1/dapr/
-drwxr-xr-x   0 bverst     (501) staff       (20)        0 2023-04-19 22:47:03.000000 dapr-ext-workflow-0.0.1rc1/dapr/ext/
-drwxr-xr-x   0 bverst     (501) staff       (20)        0 2023-04-19 22:47:03.000000 dapr-ext-workflow-0.0.1rc1/dapr/ext/workflow/
--rw-r--r--   0 bverst     (501) staff       (20)      745 2023-04-19 22:36:51.000000 dapr-ext-workflow-0.0.1rc1/dapr/ext/workflow/__init__.py
--rw-r--r--   0 bverst     (501) staff       (20)      613 2023-04-19 22:46:49.000000 dapr-ext-workflow-0.0.1rc1/dapr/ext/workflow/version.py
-drwxr-xr-x   0 bverst     (501) staff       (20)        0 2023-04-19 22:47:03.000000 dapr-ext-workflow-0.0.1rc1/dapr_ext_workflow.egg-info/
--rw-r--r--   0 bverst     (501) staff       (20)     1596 2023-04-19 22:47:03.000000 dapr-ext-workflow-0.0.1rc1/dapr_ext_workflow.egg-info/PKG-INFO
--rw-r--r--   0 bverst     (501) staff       (20)      300 2023-04-19 22:47:03.000000 dapr-ext-workflow-0.0.1rc1/dapr_ext_workflow.egg-info/SOURCES.txt
--rw-r--r--   0 bverst     (501) staff       (20)        1 2023-04-19 22:47:03.000000 dapr-ext-workflow-0.0.1rc1/dapr_ext_workflow.egg-info/dependency_links.txt
--rw-r--r--   0 bverst     (501) staff       (20)       23 2023-04-19 22:47:03.000000 dapr-ext-workflow-0.0.1rc1/dapr_ext_workflow.egg-info/requires.txt
--rw-r--r--   0 bverst     (501) staff       (20)        5 2023-04-19 22:47:03.000000 dapr-ext-workflow-0.0.1rc1/dapr_ext_workflow.egg-info/top_level.txt
--rw-r--r--   0 bverst     (501) staff       (20)      887 2023-04-19 22:47:03.000000 dapr-ext-workflow-0.0.1rc1/setup.cfg
--rw-r--r--   0 bverst     (501) staff       (20)     2181 2023-04-19 22:33:40.000000 dapr-ext-workflow-0.0.1rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:51:50.000000 dapr-ext-workflow-0.1.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-06-01 16:51:31.000000 dapr-ext-workflow-0.1.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-01 16:51:50.000000 dapr-ext-workflow-0.1.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-01 16:51:31.000000 dapr-ext-workflow-0.1.0rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:51:50.000000 dapr-ext-workflow-0.1.0rc1/dapr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:51:50.000000 dapr-ext-workflow-0.1.0rc1/dapr/ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:51:50.000000 dapr-ext-workflow-0.1.0rc1/dapr/ext/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-01 16:51:31.000000 dapr-ext-workflow-0.1.0rc1/dapr/ext/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10443 2023-06-01 16:51:31.000000 dapr-ext-workflow-0.1.0rc1/dapr/ext/workflow/dapr_workflow_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-06-01 16:51:31.000000 dapr-ext-workflow-0.1.0rc1/dapr/ext/workflow/dapr_workflow_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-01 16:51:31.000000 dapr-ext-workflow-0.1.0rc1/dapr/ext/workflow/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-01 16:51:31.000000 dapr-ext-workflow-0.1.0rc1/dapr/ext/workflow/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-01 16:51:31.000000 dapr-ext-workflow-0.1.0rc1/dapr/ext/workflow/workflow_activity_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-06-01 16:51:31.000000 dapr-ext-workflow-0.1.0rc1/dapr/ext/workflow/workflow_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-01 16:51:31.000000 dapr-ext-workflow-0.1.0rc1/dapr/ext/workflow/workflow_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-01 16:51:31.000000 dapr-ext-workflow-0.1.0rc1/dapr/ext/workflow/workflow_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:51:50.000000 dapr-ext-workflow-0.1.0rc1/dapr_ext_workflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-01 16:51:50.000000 dapr-ext-workflow-0.1.0rc1/dapr_ext_workflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-01 16:51:50.000000 dapr-ext-workflow-0.1.0rc1/dapr_ext_workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 16:51:50.000000 dapr-ext-workflow-0.1.0rc1/dapr_ext_workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-01 16:51:50.000000 dapr-ext-workflow-0.1.0rc1/dapr_ext_workflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 16:51:50.000000 dapr-ext-workflow-0.1.0rc1/dapr_ext_workflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-01 16:51:50.000000 dapr-ext-workflow-0.1.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-01 16:51:31.000000 dapr-ext-workflow-0.1.0rc1/setup.py
```

### Comparing `dapr-ext-workflow-0.0.1rc1/LICENSE` & `dapr-ext-workflow-0.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-0.0.1rc1/PKG-INFO` & `dapr-ext-workflow-0.1.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr-ext-workflow
-Version: 0.0.1rc1
+Version: 0.1.0rc1
 Summary: The official release of Dapr Python SDK Workflow Authoring Extension.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-ext-workflow-0.0.1rc1/dapr/ext/workflow/__init__.py` & `dapr-ext-workflow-0.1.0rc1/dapr/ext/workflow/util.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-# Import your main classes here
-# from dapr.ext.workflow.creator import Creator, Workflow   # type:ignore
+from typing import Optional
 
+from dapr.conf import settings
 
-__all__ = [
-    # 'Creator',
-    # 'Workflow',
-]
+
+def getAddress(host: Optional[str] = None, port: Optional[str] = None) -> str:
+    host = host or settings.DAPR_RUNTIME_HOST
+    port = port or settings.DAPR_GRPC_PORT
+    address = f"{host}:{port}"
+    return address
```

### Comparing `dapr-ext-workflow-0.0.1rc1/dapr/ext/workflow/version.py` & `dapr-ext-workflow-0.1.0rc1/dapr/ext/workflow/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-__version__ = "0.0.1rc1"
+__version__ = "0.1.0rc1"
```

### Comparing `dapr-ext-workflow-0.0.1rc1/dapr_ext_workflow.egg-info/PKG-INFO` & `dapr-ext-workflow-0.1.0rc1/dapr_ext_workflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr-ext-workflow
-Version: 0.0.1rc1
+Version: 0.1.0rc1
 Summary: The official release of Dapr Python SDK Workflow Authoring Extension.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-ext-workflow-0.0.1rc1/setup.cfg` & `dapr-ext-workflow-0.1.0rc1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 	Source = https://github.com/dapr/python-sdk
 
 [options]
 python_requires = >=3.7
 packages = find_namespace:
 include_package_data = True
 install_requires = 
-	dapr-dev >= 1.9.0rc1.dev
+	dapr >= 1.10.0rc1
+	durabletask >= 0.1.0a2
 
 [options.packages.find]
 include = 
 	dapr.*
 exclude = 
 	tests
```

### Comparing `dapr-ext-workflow-0.0.1rc1/setup.py` & `dapr-ext-workflow-0.1.0rc1/setup.py`

 * *Files identical despite different names*

