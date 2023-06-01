# Comparing `tmp/qoqo_qiskit-0.1.3.tar.gz` & `tmp/qoqo_qiskit-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qoqo_qiskit-0.1.3.tar", last modified: Tue May 16 12:01:43 2023, max compression
+gzip compressed data, was "qoqo_qiskit-0.1.4.tar", last modified: Thu Jun  1 09:22:37 2023, max compression
```

## Comparing `qoqo_qiskit-0.1.3.tar` & `qoqo_qiskit-0.1.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:01:43.942847 qoqo_qiskit-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-16 12:01:25.000000 qoqo_qiskit-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-05-16 12:01:43.942847 qoqo_qiskit-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-16 12:01:25.000000 qoqo_qiskit-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:01:43.938846 qoqo_qiskit-0.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-16 12:01:25.000000 qoqo_qiskit-0.1.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-05-16 12:01:25.000000 qoqo_qiskit-0.1.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-16 12:01:25.000000 qoqo_qiskit-0.1.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-16 12:01:25.000000 qoqo_qiskit-0.1.3/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-16 12:01:25.000000 qoqo_qiskit-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 12:01:43.942847 qoqo_qiskit-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:01:43.938846 qoqo_qiskit-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:01:43.938846 qoqo_qiskit-0.1.3/src/qoqo_qiskit/
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-16 12:01:25.000000 qoqo_qiskit-0.1.3/src/qoqo_qiskit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:01:43.938846 qoqo_qiskit-0.1.3/src/qoqo_qiskit/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-16 12:01:25.000000 qoqo_qiskit-0.1.3/src/qoqo_qiskit/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-05-16 12:01:25.000000 qoqo_qiskit-0.1.3/src/qoqo_qiskit/backend/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:01:43.938846 qoqo_qiskit-0.1.3/src/qoqo_qiskit/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-16 12:01:25.000000 qoqo_qiskit-0.1.3/src/qoqo_qiskit/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-16 12:01:25.000000 qoqo_qiskit-0.1.3/src/qoqo_qiskit/interface/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:01:43.938846 qoqo_qiskit-0.1.3/src/qoqo_qiskit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-05-16 12:01:43.000000 qoqo_qiskit-0.1.3/src/qoqo_qiskit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-16 12:01:43.000000 qoqo_qiskit-0.1.3/src/qoqo_qiskit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 12:01:43.000000 qoqo_qiskit-0.1.3/src/qoqo_qiskit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-16 12:01:43.000000 qoqo_qiskit-0.1.3/src/qoqo_qiskit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 12:01:43.000000 qoqo_qiskit-0.1.3/src/qoqo_qiskit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:01:43.942847 qoqo_qiskit-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-16 12:01:25.000000 qoqo_qiskit-0.1.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:01:43.942847 qoqo_qiskit-0.1.3/tests/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-16 12:01:25.000000 qoqo_qiskit-0.1.3/tests/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-05-16 12:01:25.000000 qoqo_qiskit-0.1.3/tests/backend/test_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:01:43.942847 qoqo_qiskit-0.1.3/tests/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-16 12:01:25.000000 qoqo_qiskit-0.1.3/tests/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-05-16 12:01:25.000000 qoqo_qiskit-0.1.3/tests/interface/test_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:22:37.949056 qoqo_qiskit-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14379 2023-06-01 09:22:37.949056 qoqo_qiskit-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:22:37.945057 qoqo_qiskit-0.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 09:22:37.949056 qoqo_qiskit-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:22:37.945057 qoqo_qiskit-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:22:37.945057 qoqo_qiskit-0.1.4/src/qoqo_qiskit/
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/src/qoqo_qiskit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:22:37.949056 qoqo_qiskit-0.1.4/src/qoqo_qiskit/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/src/qoqo_qiskit/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/src/qoqo_qiskit/backend/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:22:37.949056 qoqo_qiskit-0.1.4/src/qoqo_qiskit/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/src/qoqo_qiskit/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/src/qoqo_qiskit/interface/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:22:37.945057 qoqo_qiskit-0.1.4/src/qoqo_qiskit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14379 2023-06-01 09:22:37.000000 qoqo_qiskit-0.1.4/src/qoqo_qiskit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-01 09:22:37.000000 qoqo_qiskit-0.1.4/src/qoqo_qiskit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 09:22:37.000000 qoqo_qiskit-0.1.4/src/qoqo_qiskit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-01 09:22:37.000000 qoqo_qiskit-0.1.4/src/qoqo_qiskit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 09:22:37.000000 qoqo_qiskit-0.1.4/src/qoqo_qiskit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:22:37.949056 qoqo_qiskit-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:22:37.949056 qoqo_qiskit-0.1.4/tests/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/tests/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/tests/backend/test_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:22:37.949056 qoqo_qiskit-0.1.4/tests/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/tests/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/tests/interface/test_interface.py
```

### Comparing `qoqo_qiskit-0.1.3/LICENSE` & `qoqo_qiskit-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.1.3/PKG-INFO` & `qoqo_qiskit-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoqo_qiskit
-Version: 0.1.3
+Version: 0.1.4
 Author-email: HQS Quantum Simulation GmbH <info@quantumsimulations.de>
 Maintainer-email: Matteo Lodi <matteo.lodi@quantumsimulations.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -211,21 +211,31 @@
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 <img src="../qoqo_Logo_vertical_color.png" alt="qoqo logo" width="300" />
 
 # qoqo_qiskit
-
+[![Documentation Status](https://img.shields.io/badge/docs-documentation-green)](https://hqsquantumsimulations.github.io/qoqo-qiskit/)
+[![PyPI](https://img.shields.io/pypi/v/qoqo_qiskit)](https://pypi.org/project/qoqo_qiskit/)
 
 Qiskit interface for the qoqo quantum toolkit by [HQS Quantum Simulations](https://quantumsimulations.de).
 
-__General__
+### Installation
+
+We provide pre-built binaries for linux, macos and windows on x86_64 hardware and macos on arm64. Simply install the pre-built wheels with
+
+```shell
+pip install qoqo-qiskit
+```
+
+## General
+
+Qiskit is under the Apache-2.0 license ( see https://github.com/Qiskit/qiskit/blob/master/LICENSE.txt ).
 
-qoqo_qiskit provides an interface to Qiskit's package.
-Qiskit is under the Apache-2.0 license ( see https://github.com/Qiskit/qiskit/blob/master/LICENSE.txt ). qoqo_qiskit itself is also provided under the Apache-2.0 license.
+qoqo_qiskit itself is also provided under the Apache-2.0 license.
 
-__Testing__
+## Testing
 
 This software is still in the beta stage. Functions and documentation are not yet complete and breaking changes can occur.
 
 If you find unexpected behaviour please open a github issue. You can also run the pytests in qoqo_qiskit/tests/ locally.
```

### Comparing `qoqo_qiskit-0.1.3/docs/Makefile` & `qoqo_qiskit-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.1.3/docs/conf.py` & `qoqo_qiskit-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.1.3/pyproject.toml` & `qoqo_qiskit-0.1.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "qoqo_qiskit"
-version = "0.1.3"
+version = "0.1.4"
 license = {file="LICENSE"}
 authors = [
     {name="HQS Quantum Simulation GmbH", email="info@quantumsimulations.de"}
 ]
 maintainers = [
     {name="Matteo Lodi", email="matteo.lodi@quantumsimulations.de"}
 ]
@@ -30,15 +30,14 @@
     'flake8-pydocstyle',
     'darglint',
     'bandit',
     'mypy',
     'black'
 ]
 docs = [
-    'numpy',
     'sphinx>=2.1',
     'nbsphinx',
     'pygments',
     'recommonmark',
     'myst_parser',
     'sphinx_rtd_theme',
     'tomli'
```

### Comparing `qoqo_qiskit-0.1.3/src/qoqo_qiskit/__init__.py` & `qoqo_qiskit-0.1.4/src/qoqo_qiskit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 Translates qoqo operations and circuits to qiskit equivalents.
 
 .. autosummary::
     :toctree: generated/
 
     to_qiskit_circuit
-    QoqoQiskitSimulator
+    QoqoQiskitBackend
 
 """
 
 
 from qoqo_qiskit.backend import QoqoQiskitBackend
 from qoqo_qiskit.interface import to_qiskit_circuit
```

### Comparing `qoqo_qiskit-0.1.3/src/qoqo_qiskit/backend/__init__.py` & `qoqo_qiskit-0.1.4/src/qoqo_qiskit/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.1.3/src/qoqo_qiskit/backend/backend.py` & `qoqo_qiskit-0.1.4/src/qoqo_qiskit/backend/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,16 +59,16 @@
         Currently only one simulation is performed, meaning different measurements on different
         registers are not supported.
 
         Args:
             circuit (Circuit): the Circuit to simulate.
 
         Returns:
-            Tuple[Dict[str, List[List[bool]]],
-                  Dict[str, List[List[float]]],
+            Tuple[Dict[str, List[List[bool]]],\
+                  Dict[str, List[List[float]]],\
                   Dict[str, List[List[complex]]]]: bit, float and complex registers dictionaries.
 
         Raises:
             ValueError: the Circuit does not contain Measurement operations
         """
         clas_regs_sizes: Dict[str, int] = dict()
 
@@ -197,16 +197,16 @@
     ]:
         """Run all circuits of a measurement with the Qiskit backend.
 
         Args:
             measurement: The measurement that is run.
 
         Returns:
-            Tuple[Dict[str, List[List[bool]]],
-                  Dict[str, List[List[float]]],
+            Tuple[Dict[str, List[List[bool]]],\
+                  Dict[str, List[List[float]]],\
                   Dict[str, List[List[complex]]]]
         """
         constant_circuit = measurement.constant_circuit()
         output_bit_register_dict: Dict[str, List[List[bool]]] = dict()
         output_float_register_dict: Dict[str, List[List[float]]] = dict()
         output_complex_register_dict: Dict[str, List[List[complex]]] = dict()
```

### Comparing `qoqo_qiskit-0.1.3/src/qoqo_qiskit/interface/__init__.py` & `qoqo_qiskit-0.1.4/src/qoqo_qiskit/interface/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,13 +5,13 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
-"""Qoqo-qiskit backend package for compatibility and simulation purposes."""
+"""Qiskit interface for qoqo circuits."""
 
 
 from qoqo_qiskit.interface.interface import to_qiskit_circuit
 
 __all__ = "to_qiskit_circuit"
```

### Comparing `qoqo_qiskit-0.1.3/src/qoqo_qiskit/interface/interface.py` & `qoqo_qiskit-0.1.4/src/qoqo_qiskit/interface/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     """Applies the qoqo Circuit -> Qiskit QuantumCircuit conversion.
 
     Args:
         circuit (Circuit): the qoqo Circuit to port.
         qubit_register_name (Optional[str]): the name of the qubit register.
 
     Returns:
-        Tuple[QuantumCircuit, Dict[str, int]]: the equivalent QuantumCircuit and the dict
+        Tuple[QuantumCircuit, Dict[str, int]]: equivalent QuantumCircuit and dict\
                                             containing info for Qiskit's backend.
 
     Raises:
         ValueError: the circuit contains a symbolic PragmaLoop operation.
     """
     # Populating dict output. Currently handling:
     #   - PragmaSetStateVector (continues further down)
```

### Comparing `qoqo_qiskit-0.1.3/src/qoqo_qiskit.egg-info/PKG-INFO` & `qoqo_qiskit-0.1.4/src/qoqo_qiskit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoqo-qiskit
-Version: 0.1.3
+Version: 0.1.4
 Author-email: HQS Quantum Simulation GmbH <info@quantumsimulations.de>
 Maintainer-email: Matteo Lodi <matteo.lodi@quantumsimulations.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -211,21 +211,31 @@
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 <img src="../qoqo_Logo_vertical_color.png" alt="qoqo logo" width="300" />
 
 # qoqo_qiskit
-
+[![Documentation Status](https://img.shields.io/badge/docs-documentation-green)](https://hqsquantumsimulations.github.io/qoqo-qiskit/)
+[![PyPI](https://img.shields.io/pypi/v/qoqo_qiskit)](https://pypi.org/project/qoqo_qiskit/)
 
 Qiskit interface for the qoqo quantum toolkit by [HQS Quantum Simulations](https://quantumsimulations.de).
 
-__General__
+### Installation
+
+We provide pre-built binaries for linux, macos and windows on x86_64 hardware and macos on arm64. Simply install the pre-built wheels with
+
+```shell
+pip install qoqo-qiskit
+```
+
+## General
+
+Qiskit is under the Apache-2.0 license ( see https://github.com/Qiskit/qiskit/blob/master/LICENSE.txt ).
 
-qoqo_qiskit provides an interface to Qiskit's package.
-Qiskit is under the Apache-2.0 license ( see https://github.com/Qiskit/qiskit/blob/master/LICENSE.txt ). qoqo_qiskit itself is also provided under the Apache-2.0 license.
+qoqo_qiskit itself is also provided under the Apache-2.0 license.
 
-__Testing__
+## Testing
 
 This software is still in the beta stage. Functions and documentation are not yet complete and breaking changes can occur.
 
 If you find unexpected behaviour please open a github issue. You can also run the pytests in qoqo_qiskit/tests/ locally.
```

### Comparing `qoqo_qiskit-0.1.3/src/qoqo_qiskit.egg-info/SOURCES.txt` & `qoqo_qiskit-0.1.4/src/qoqo_qiskit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.1.3/tests/__init__.py` & `qoqo_qiskit-0.1.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.1.3/tests/backend/__init__.py` & `qoqo_qiskit-0.1.4/tests/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.1.3/tests/backend/test_backend.py` & `qoqo_qiskit-0.1.4/tests/backend/test_backend.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.1.3/tests/interface/__init__.py` & `qoqo_qiskit-0.1.4/tests/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.1.3/tests/interface/test_interface.py` & `qoqo_qiskit-0.1.4/tests/interface/test_interface.py`

 * *Files identical despite different names*

