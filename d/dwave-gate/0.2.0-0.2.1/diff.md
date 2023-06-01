# Comparing `tmp/dwave-gate-0.2.0.tar.gz` & `tmp/dwave-gate-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwave-gate-0.2.0.tar", last modified: Thu Feb  9 19:08:17 2023, max compression
+gzip compressed data, was "dwave-gate-0.2.1.tar", last modified: Thu Jun  1 14:57:32 2023, max compression
```

## Comparing `dwave-gate-0.2.0.tar` & `dwave-gate-0.2.1.tar`

### file list

```diff
@@ -1,45 +1,44 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-09 19:08:17.624256 dwave-gate-0.2.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11351 2023-02-09 19:08:06.000000 dwave-gate-0.2.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)       87 2023-02-09 19:08:06.000000 dwave-gate-0.2.0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4740 2023-02-09 19:08:17.624256 dwave-gate-0.2.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3791 2023-02-09 19:08:06.000000 dwave-gate-0.2.0/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-09 19:08:17.616256 dwave-gate-0.2.0/dwave/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      678 2023-02-09 19:08:06.000000 dwave-gate-0.2.0/dwave/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-09 19:08:17.620256 dwave-gate-0.2.0/dwave/gate/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      742 2023-02-09 19:08:06.000000 dwave-gate-0.2.0/dwave/gate/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    30481 2023-02-09 19:08:06.000000 dwave-gate-0.2.0/dwave/gate/circuit.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4836 2023-02-09 19:08:06.000000 dwave-gate-0.2.0/dwave/gate/mixedproperty.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-09 19:08:17.620256 dwave-gate-0.2.0/dwave/gate/operations/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      786 2023-02-09 19:08:06.000000 dwave-gate-0.2.0/dwave/gate/operations/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26268 2023-02-09 19:08:06.000000 dwave-gate-0.2.0/dwave/gate/operations/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26782 2023-02-09 19:08:06.000000 dwave-gate-0.2.0/dwave/gate/operations/operations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5798 2023-02-09 19:08:06.000000 dwave-gate-0.2.0/dwave/gate/primitives.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-09 19:08:17.620256 dwave-gate-0.2.0/dwave/gate/registers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      894 2023-02-09 19:08:06.000000 dwave-gate-0.2.0/dwave/gate/registers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   617152 2023-02-09 19:08:16.000000 dwave-gate-0.2.0/dwave/gate/registers/cyregister.cpp
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1332 2023-02-09 19:08:06.000000 dwave-gate-0.2.0/dwave/gate/registers/cyregister.pxd
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15052 2023-02-09 19:08:06.000000 dwave-gate-0.2.0/dwave/gate/registers/cyregister.pyx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7049 2023-02-09 19:08:06.000000 dwave-gate-0.2.0/dwave/gate/registers/registers.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-09 19:08:17.620256 dwave-gate-0.2.0/dwave/gate/simulator/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      905 2023-02-09 19:08:06.000000 dwave-gate-0.2.0/dwave/gate/simulator/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27915 2023-02-09 19:08:06.000000 dwave-gate-0.2.0/dwave/gate/simulator/operation_generation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    43293 2023-02-09 19:08:15.000000 dwave-gate-0.2.0/dwave/gate/simulator/ops.h
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23912 2023-02-09 19:08:15.000000 dwave-gate-0.2.0/dwave/gate/simulator/ops.pxd
--rw-r--r--   0 circleci  (1001) circleci  (1002)  1319433 2023-02-09 19:08:17.000000 dwave-gate-0.2.0/dwave/gate/simulator/simulator.cpp
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6999 2023-02-09 19:08:06.000000 dwave-gate-0.2.0/dwave/gate/simulator/simulator.pyx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-09 19:08:17.620256 dwave-gate-0.2.0/dwave/gate/tools/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      957 2023-02-09 19:08:06.000000 dwave-gate-0.2.0/dwave/gate/tools/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3467 2023-02-09 19:08:06.000000 dwave-gate-0.2.0/dwave/gate/tools/counters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1591 2023-02-09 19:08:06.000000 dwave-gate-0.2.0/dwave/gate/tools/samples.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5789 2023-02-09 19:08:06.000000 dwave-gate-0.2.0/dwave/gate/tools/unitary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3140 2023-02-09 19:08:06.000000 dwave-gate-0.2.0/dwave/gate/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-09 19:08:17.624256 dwave-gate-0.2.0/dwave_gate.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4740 2023-02-09 19:08:17.000000 dwave-gate-0.2.0/dwave_gate.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      995 2023-02-09 19:08:17.000000 dwave-gate-0.2.0/dwave_gate.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-02-09 19:08:17.000000 dwave-gate-0.2.0/dwave_gate.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-02-09 19:08:17.000000 dwave-gate-0.2.0/dwave_gate.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-02-09 19:08:17.000000 dwave-gate-0.2.0/dwave_gate.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-02-09 19:08:17.000000 dwave-gate-0.2.0/dwave_gate.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1045 2023-02-09 19:08:06.000000 dwave-gate-0.2.0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1027 2023-02-09 19:08:17.624256 dwave-gate-0.2.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1720 2023-02-09 19:08:06.000000 dwave-gate-0.2.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 14:57:32.861528 dwave-gate-0.2.1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11351 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       87 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4740 2023-06-01 14:57:32.861528 dwave-gate-0.2.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3791 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 14:57:32.857528 dwave-gate-0.2.1/dwave/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      678 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 14:57:32.857528 dwave-gate-0.2.1/dwave/gate/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      742 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32825 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/circuit.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4836 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/mixedproperty.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 14:57:32.857528 dwave-gate-0.2.1/dwave/gate/operations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      786 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/operations/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27036 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/operations/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26782 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/operations/operations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5798 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/primitives.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 14:57:32.857528 dwave-gate-0.2.1/dwave/gate/registers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      894 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/registers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   617152 2023-06-01 14:57:31.000000 dwave-gate-0.2.1/dwave/gate/registers/cyregister.cpp
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1332 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/registers/cyregister.pxd
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15052 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/registers/cyregister.pyx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7049 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/registers/registers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 14:57:32.861528 dwave-gate-0.2.1/dwave/gate/simulator/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      921 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/simulator/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27915 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/simulator/operation_generation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43293 2023-06-01 14:57:30.000000 dwave-gate-0.2.1/dwave/gate/simulator/ops.h
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23912 2023-06-01 14:57:30.000000 dwave-gate-0.2.1/dwave/gate/simulator/ops.pxd
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  1320438 2023-06-01 14:57:32.000000 dwave-gate-0.2.1/dwave/gate/simulator/simulator.cpp
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7582 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/simulator/simulator.pyx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 14:57:32.861528 dwave-gate-0.2.1/dwave/gate/tools/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      957 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/tools/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3467 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/tools/counters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5789 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/tools/unitary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3140 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 14:57:32.861528 dwave-gate-0.2.1/dwave_gate.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4740 2023-06-01 14:57:32.000000 dwave-gate-0.2.1/dwave_gate.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      967 2023-06-01 14:57:32.000000 dwave-gate-0.2.1/dwave_gate.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-01 14:57:32.000000 dwave-gate-0.2.1/dwave_gate.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-01 14:57:32.000000 dwave-gate-0.2.1/dwave_gate.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-06-01 14:57:32.000000 dwave-gate-0.2.1/dwave_gate.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-06-01 14:57:32.000000 dwave-gate-0.2.1/dwave_gate.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1045 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1027 2023-06-01 14:57:32.861528 dwave-gate-0.2.1/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1720 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/setup.py
```

### Comparing `dwave-gate-0.2.0/LICENSE` & `dwave-gate-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.0/PKG-INFO` & `dwave-gate-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwave-gate
-Version: 0.2.0
+Version: 0.2.1
 Summary: Gate model library.
 Home-page: https://github.com/dwavesystems/dwave-gate
 Author: D-Wave Systems Inc.
 Author-email: tools@dwavesys.com
 License: UNKNOWN
 Download-URL: https://github.com/dwavesystems/dwave-gate/releases
 Platform: UNKNOWN
```

### Comparing `dwave-gate-0.2.0/README.rst` & `dwave-gate-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.0/dwave/__init__.py` & `dwave-gate-0.2.1/dwave/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.0/dwave/gate/__init__.py` & `dwave-gate-0.2.1/dwave/gate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 from dwave.gate.circuit import *
 from dwave.gate.mixedproperty import *
 from dwave.gate.primitives import *
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
```

### Comparing `dwave-gate-0.2.0/dwave/gate/circuit.py` & `dwave-gate-0.2.1/dwave/gate/circuit.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,21 @@
 operations and instructions for running the circuits on simulators or hardware. See
 :py:mod:`dwave.gate.operations` for details on which operations are supported.
 """
 
 from __future__ import annotations
 
 import itertools
+import warnings
+from typing import TYPE_CHECKING
+
+import numpy as np
+
+if TYPE_CHECKING:
+    from numpy.typing import NDArray
 
 __all__ = [
     "CircuitError",
     "Circuit",
     "ParametricCircuit",
     "CircuitContext",
     "ParametricCircuitContext",
@@ -91,15 +98,18 @@
 
         if num_qubits is not None:
             self.add_qregister(num_qubits=num_qubits)
 
         if num_bits is not None:
             self.add_cregister(num_bits=num_bits)
 
-        self._locked = False
+        self._state: NDArray = None
+        self._density_matrix: NDArray = None
+
+        self._locked: bool = False
 
     def __call__(self, qubits: Qubits) -> None:
         """Apply all the operations in the circuit within a circuit context.
 
         Args:
             qubits: Qubits on which the circuit operations should be applied. The qubits used in
                 the circuit will be exchanged with the corresponding ones (e.g., with the same
@@ -217,14 +227,65 @@
         bit_reg = ClassicalRegister()
         for creg in self.cregisters.values():
             bit_reg += creg
 
         return bit_reg
 
     @property
+    def state(self) -> Optional[NDArray]:
+        """The resulting state after simulating the circuit."""
+        if self._state is None and self._density_matrix is not None:
+            raise CircuitError("State is mixed. Use 'Circuit.density_matrix' to access.")
+        return self._state
+
+    @property
+    def density_matrix(self) -> Optional[NDArray]:
+        """The density matrix representation of the state."""
+        if self._state is not None and self._density_matrix is None:
+            self._density_matrix = self._state.reshape(-1, 1) @ self._state.reshape(1, -1)
+        return self._density_matrix
+
+    def set_state(self, state: NDArray, force: bool = False, normalize: bool = False) -> None:
+        """Set the state of the circuit (used primarily with simulator).
+
+        Sets either the ``Circuit.state`` attribute or the ``Circuit.density_matrix`` attribute
+        depending on the shape of the state.
+
+        Args:
+            state: The state (pure or mixed) to set.
+            force: Whether to overwrite an already set state or not.
+            normalize: Whether to normalize the state before setting.
+        """
+        state_is_set = self._state is not None or self._density_matrix is not None
+        if not force and state_is_set:
+            raise CircuitError("State already set. Use 'force=True' to force set new state.")
+
+        if normalize:
+            state = state / np.linalg.norm(state)
+
+        self._assert_state(state)
+
+        if state.ndim == 1:
+            self._state = state
+            self._density_matrix = None
+
+        else:  # if state.ndim == 2:
+            self._state = None
+            self._density_matrix = state
+
+    def _assert_state(self, state: NDArray) -> None:
+        """Check whether a state is the correct shape and is normalized."""
+        size = 2 << (self.num_qubits - 1)
+        if state.shape != (size,) and state.shape != (size, size):
+            raise ValueError(f"State has incorrect shape. Should have size {size}.")
+
+        if not np.isclose(np.linalg.norm(state), 1):
+            raise ValueError("State is not normalized.")
+
+    @property
     def num_qubits(self) -> int:
         """Number of qubits in the circuit."""
         return len(self.qubits)
 
     @property
     def num_bits(self) -> int:
         """Number of bits in the circuit."""
```

### Comparing `dwave-gate-0.2.0/dwave/gate/mixedproperty.py` & `dwave-gate-0.2.1/dwave/gate/mixedproperty.py`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.0/dwave/gate/operations/__init__.py` & `dwave-gate-0.2.1/dwave/gate/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.0/dwave/gate/operations/base.py` & `dwave-gate-0.2.1/dwave/gate/operations/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "Measurement",
     "Barrier",
     "create_operation",
 ]
 
 import copy
 import warnings
-from abc import ABCMeta, abstractproperty
+from abc import ABCMeta
 from itertools import chain
 from typing import (
     TYPE_CHECKING,
     Hashable,
     List,
     Mapping,
     Optional,
@@ -45,19 +45,19 @@
     TypeVar,
     Union,
     overload,
 )
 
 import numpy as np
 
-from dwave.gate.circuit import Circuit, CircuitContext, ParametricCircuit
+from dwave.gate.circuit import Circuit, CircuitContext, CircuitError, ParametricCircuit
 from dwave.gate.mixedproperty import mixedproperty
 from dwave.gate.primitives import Bit, Qubit
 from dwave.gate.registers.registers import ClassicalRegister, Variable
-from dwave.gate.tools.samples import sample
+from dwave.gate.simulator.simulator import sample_qubit
 from dwave.gate.tools.unitary import build_controlled_unitary, build_unitary
 
 if TYPE_CHECKING:
     from numpy.typing import NDArray
 
 
 Qubits = Union[Qubit, Sequence[Qubit]]
@@ -688,48 +688,71 @@
         return self._bits
 
     @property
     def state(self) -> Optional[NDArray]:
         """The circuit state when measured."""
         return self._measured_state
 
-    def sample(self, qubit: Optional[int] = None, num_samples: int = 1) -> Optional[Sequence[int]]:
+    def sample(
+        self,
+        qubits: Optional[Sequence[int]] = None,
+        num_samples: int = 1,
+        as_bitstring: bool = False,
+    ) -> List[Union[int, str]]:
         """Sample the measured state.
 
         Args:
-            qubit: The qubit to sample. Not required if measurement is on a single qubit.
-            num_samples: The number of samples to measure.
+            qubits: The qubits to sample. If not given, all measured qubits are sampled.
+            num_samples: The number of samples to to return.
+            as_bitstring: Whether to return the samples as bitstrings or as
+                lists of integers (default).
 
         Returns:
-            Sequence[int]: The measurement samples.
+            List[Union[int, str]]: The measurement samples for each qubit.
         """
-        if qubit is None and self.num_qubits != 1:
-            raise ValueError("Measurement has several qubit. Must specify which to sample.")
+        if self.state is None:
+            raise CircuitError(
+                "Measurement has no state. Likely due to circuit not having been simulated."
+            )
+
+        if qubits is None:
+            qubits = self._measured_qubit_indices
+
+        num_qubits = len(self.state).bit_length() - 1
 
-        if self.state is not None:
-            return sample(
-                qubit or self._measured_qubit_indices[0], self.state, num_samples=num_samples
+        if max(qubits) >= num_qubits:
+            raise ValueError(
+                f"Cannot sample qubit {max(qubits)} (count. from 0). "
+                f"State has only {num_qubits} qubits."
+            )
+
+        rng = np.random.default_rng()
+        samples = []
+        for _ in range(num_samples):
+            state_copy = self.state.copy()
+            samples.append(
+                [sample_qubit(qb, state_copy, rng, collapse_state=True) for qb in qubits]
             )
-        return None
 
-    def expval(self, qubit: Optional[int] = None, num_samples: int = 1000) -> Optional[float]:
+        if as_bitstring:
+            return ["".join(map(str, s)) for s in samples]
+        return samples
+
+    def expval(self, qubits: Optional[int] = None, num_samples: int = 1000) -> List[float]:
         """Calculate the expectation value of a measurement.
 
         Args:
             qubit: The qubit to sample. Not required if measurement is on a single qubit.
             num_samples: The number of samples to use when calculating the expectation value.
 
         Returns:
-            float: The expectation value of the measurement.
+            list[float]: The expectation values for each qubit measurement.
         """
-        samples = self.sample(qubit, num_samples)
-
-        if samples is not None:
-            return np.mean(samples, dtype=float)
-        return None
+        samples = self.sample(qubits, num_samples=num_samples)
+        return np.transpose(samples).mean(axis=1).tolist()
 
 
 class Barrier(Operation):
     """Class representing a barrier operation.
 
     Args:
         qubits: Qubits on which the barrier operation should be applied.
```

### Comparing `dwave-gate-0.2.0/dwave/gate/operations/operations.py` & `dwave-gate-0.2.1/dwave/gate/operations/operations.py`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.0/dwave/gate/primitives.py` & `dwave-gate-0.2.1/dwave/gate/primitives.py`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.0/dwave/gate/registers/__init__.py` & `dwave-gate-0.2.1/dwave/gate/registers/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.0/dwave/gate/registers/cyregister.cpp` & `dwave-gate-0.2.1/dwave/gate/registers/cyregister.cpp`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.0/dwave/gate/registers/cyregister.pxd` & `dwave-gate-0.2.1/dwave/gate/registers/cyregister.pxd`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.0/dwave/gate/registers/cyregister.pyx` & `dwave-gate-0.2.1/dwave/gate/registers/cyregister.pyx`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.0/dwave/gate/registers/registers.py` & `dwave-gate-0.2.1/dwave/gate/registers/registers.py`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.0/dwave/gate/simulator/__init__.py` & `dwave-gate-0.2.1/dwave/gate/simulator/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 """Simulators for running circuits locally.
 
 Contains a state-vector simulator able to return the resulting state vector after running a circuit
 on an all-zero initialized basis state. Supports both the little- and big-endian conventions.
 """
 
-from dwave.gate.simulator.simulator import *
+from dwave.gate.simulator.simulator import *  # type: ignore
```

### Comparing `dwave-gate-0.2.0/dwave/gate/simulator/operation_generation.py` & `dwave-gate-0.2.1/dwave/gate/simulator/operation_generation.py`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.0/dwave/gate/simulator/ops.h` & `dwave-gate-0.2.1/dwave/gate/simulator/ops.h`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.0/dwave/gate/simulator/ops.pxd` & `dwave-gate-0.2.1/dwave/gate/simulator/ops.pxd`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.0/dwave/gate/simulator/simulator.cpp` & `dwave-gate-0.2.1/dwave/gate/simulator/simulator.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -2776,18 +2776,18 @@
 static __Pyx_TypeInfo __Pyx_TypeInfo___pyx_t_double_complex = { "double complex", NULL, sizeof(__pyx_t_double_complex), { 0 }, 0, 'C', 0, 0 };
 #define __Pyx_MODULE_NAME "dwave.gate.simulator.simulator"
 extern int __pyx_module_is_main_dwave__gate__simulator__simulator;
 int __pyx_module_is_main_dwave__gate__simulator__simulator = 0;
 
 /* Implementation of 'dwave.gate.simulator.simulator' */
 static PyObject *__pyx_builtin_ValueError;
+static PyObject *__pyx_builtin_round;
 static PyObject *__pyx_builtin_enumerate;
 static PyObject *__pyx_builtin_IndexError;
 static PyObject *__pyx_builtin_TypeError;
-static PyObject *__pyx_builtin_round;
 static PyObject *__pyx_builtin_ImportError;
 static PyObject *__pyx_builtin_RuntimeError;
 static PyObject *__pyx_builtin_MemoryError;
 static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_Ellipsis;
 static PyObject *__pyx_builtin_id;
 static const char __pyx_k_O[] = "O";
@@ -2795,15 +2795,15 @@
 static const char __pyx_k_m[] = "m";
 static const char __pyx_k_t[] = "t";
 static const char __pyx_k_id[] = "id";
 static const char __pyx_k_np[] = "np";
 static const char __pyx_k_op[] = "op";
 static const char __pyx_k_qb[] = "qb";
 static const char __pyx_k_CCX[] = "CCX";
-static const char __pyx_k__32[] = "*";
+static const char __pyx_k__31[] = "*";
 static const char __pyx_k_all[] = "__all__";
 static const char __pyx_k_idx[] = "idx";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_obj[] = "obj";
 static const char __pyx_k_ops[] = "ops";
 static const char __pyx_k_rng[] = "rng";
 static const char __pyx_k_set[] = "set";
@@ -2851,15 +2851,14 @@
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_matrix[] = "matrix";
 static const char __pyx_k_name_2[] = "__name__";
 static const char __pyx_k_pickle[] = "pickle";
 static const char __pyx_k_qubits[] = "qubits";
 static const char __pyx_k_random[] = "random";
 static const char __pyx_k_reduce[] = "__reduce__";
-static const char __pyx_k_sample[] = "_sample";
 static const char __pyx_k_struct[] = "struct";
 static const char __pyx_k_target[] = "target";
 static const char __pyx_k_typing[] = "typing";
 static const char __pyx_k_unpack[] = "unpack";
 static const char __pyx_k_update[] = "update";
 static const char __pyx_k_Circuit[] = "Circuit";
 static const char __pyx_k_circuit[] = "circuit";
@@ -2885,14 +2884,15 @@
 static const char __pyx_k_simulate[] = "simulate";
 static const char __pyx_k_warnings[] = "warnings";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_conjugate[] = "conjugate";
 static const char __pyx_k_enumerate[] = "enumerate";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
+static const char __pyx_k_set_state[] = "set_state";
 static const char __pyx_k_IndexError[] = "IndexError";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_complex128[] = "complex128";
 static const char __pyx_k_is_blocked[] = "is_blocked";
 static const char __pyx_k_num_qubits[] = "num_qubits";
 static const char __pyx_k_parameters[] = "parameters";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
@@ -2903,14 +2903,15 @@
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_default_rng[] = "default_rng";
 static const char __pyx_k_mixed_state[] = "mixed_state";
 static const char __pyx_k_num_control[] = "num_control";
 static const char __pyx_k_CircuitError[] = "CircuitError";
 static const char __pyx_k_RuntimeError[] = "RuntimeError";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
+static const char __pyx_k_sample_qubit[] = "sample_qubit";
 static const char __pyx_k_stringsource[] = "stringsource";
 static const char __pyx_k_little_endian[] = "little_endian";
 static const char __pyx_k_pyx_getbuffer[] = "__pyx_getbuffer";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_collapse_state[] = "collapse_state";
 static const char __pyx_k_conjugate_gate[] = "conjugate_gate";
 static const char __pyx_k_density_matrix[] = "density_matrix";
@@ -2999,15 +3000,15 @@
 static PyObject *__pyx_n_s_PickleError;
 static PyObject *__pyx_n_s_RuntimeError;
 static PyObject *__pyx_n_s_SWAP;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_kp_s_Unable_to_convert_item_to_object;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_View_MemoryView;
-static PyObject *__pyx_n_s__32;
+static PyObject *__pyx_n_s__31;
 static PyObject *__pyx_n_s_all;
 static PyObject *__pyx_n_s_allocate_buffer;
 static PyObject *__pyx_n_s_append;
 static PyObject *__pyx_n_s_apply_instruction;
 static PyObject *__pyx_n_s_array;
 static PyObject *__pyx_n_s_ascontiguousarray;
 static PyObject *__pyx_n_s_base;
@@ -3103,16 +3104,18 @@
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
 static PyObject *__pyx_n_s_reshape;
 static PyObject *__pyx_n_s_rng;
 static PyObject *__pyx_n_s_rng_seed;
 static PyObject *__pyx_n_s_round;
-static PyObject *__pyx_n_s_sample;
+static PyObject *__pyx_n_s_sample_qubit;
+static PyObject *__pyx_n_u_sample_qubit;
 static PyObject *__pyx_n_s_set;
+static PyObject *__pyx_n_s_set_state;
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
 static PyObject *__pyx_n_s_shape;
 static PyObject *__pyx_n_s_simulate;
 static PyObject *__pyx_n_u_simulate;
 static PyObject *__pyx_n_s_simulate_circuit_density_matrix;
 static PyObject *__pyx_kp_u_simulator_encountered_unknown_mu;
@@ -3143,16 +3146,16 @@
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_n_s_virtual_targets;
 static PyObject *__pyx_n_s_warn;
 static PyObject *__pyx_n_s_warnings;
 static PyObject *__pyx_n_s_zeros;
 static PyObject *__pyx_pf_5dwave_4gate_9simulator_9simulator_apply_instruction(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_num_qubits, PyArrayObject *__pyx_v_state, PyObject *__pyx_v_op, PyObject *__pyx_v_targets, PyObject *__pyx_v_little_endian, PyObject *__pyx_v_rng, PyObject *__pyx_v_conjugate_gate); /* proto */
 static PyObject *__pyx_pf_5dwave_4gate_9simulator_9simulator_2simulate(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_circuit, PyObject *__pyx_v_mixed_state, PyObject *__pyx_v_little_endian, PyObject *__pyx_v_rng_seed); /* proto */
-static PyObject *__pyx_pf_5dwave_4gate_9simulator_9simulator_4_measure(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_op, PyObject *__pyx_v_state, PyObject *__pyx_v_targets, PyObject *__pyx_v_rng); /* proto */
-static PyObject *__pyx_pf_5dwave_4gate_9simulator_9simulator_6_sample(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_qubit, PyObject *__pyx_v_state, PyObject *__pyx_v_rng, PyObject *__pyx_v_collapse_state, PyObject *__pyx_v_little_endian); /* proto */
+static PyObject *__pyx_pf_5dwave_4gate_9simulator_9simulator_4sample_qubit(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_qubit, PyObject *__pyx_v_state, PyObject *__pyx_v_rng, PyObject *__pyx_v_collapse_state, PyObject *__pyx_v_little_endian); /* proto */
+static PyObject *__pyx_pf_5dwave_4gate_9simulator_9simulator_6_measure(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_op, PyObject *__pyx_v_state, PyObject *__pyx_v_targets, PyObject *__pyx_v_rng); /* proto */
 static PyObject *__pyx_pf_5dwave_4gate_9simulator_9simulator_8_simulate_circuit_density_matrix(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_circuit, PyObject *__pyx_v_rng, PyObject *__pyx_v_little_endian); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_8__getattr__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_attr); /* proto */
@@ -3202,18 +3205,18 @@
 static PyObject *__pyx_int_2;
 static PyObject *__pyx_int_112105877;
 static PyObject *__pyx_int_136983863;
 static PyObject *__pyx_int_184977713;
 static PyObject *__pyx_int_neg_1;
 static PyObject *__pyx_codeobj_;
 static PyObject *__pyx_tuple__2;
-static PyObject *__pyx_tuple__4;
+static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__8;
 static PyObject *__pyx_tuple__9;
-static PyObject *__pyx_slice__26;
+static PyObject *__pyx_slice__25;
 static PyObject *__pyx_tuple__10;
 static PyObject *__pyx_tuple__11;
 static PyObject *__pyx_tuple__12;
 static PyObject *__pyx_tuple__13;
 static PyObject *__pyx_tuple__14;
 static PyObject *__pyx_tuple__15;
 static PyObject *__pyx_tuple__16;
@@ -3221,38 +3224,37 @@
 static PyObject *__pyx_tuple__18;
 static PyObject *__pyx_tuple__19;
 static PyObject *__pyx_tuple__20;
 static PyObject *__pyx_tuple__21;
 static PyObject *__pyx_tuple__22;
 static PyObject *__pyx_tuple__23;
 static PyObject *__pyx_tuple__24;
-static PyObject *__pyx_tuple__25;
+static PyObject *__pyx_tuple__26;
 static PyObject *__pyx_tuple__27;
 static PyObject *__pyx_tuple__28;
-static PyObject *__pyx_tuple__29;
-static PyObject *__pyx_tuple__31;
+static PyObject *__pyx_tuple__30;
+static PyObject *__pyx_tuple__32;
 static PyObject *__pyx_tuple__33;
 static PyObject *__pyx_tuple__34;
 static PyObject *__pyx_tuple__35;
 static PyObject *__pyx_tuple__36;
 static PyObject *__pyx_tuple__37;
 static PyObject *__pyx_tuple__38;
 static PyObject *__pyx_tuple__39;
 static PyObject *__pyx_tuple__40;
 static PyObject *__pyx_tuple__41;
 static PyObject *__pyx_tuple__42;
-static PyObject *__pyx_tuple__43;
 static PyObject *__pyx_codeobj__3;
+static PyObject *__pyx_codeobj__4;
 static PyObject *__pyx_codeobj__5;
 static PyObject *__pyx_codeobj__6;
-static PyObject *__pyx_codeobj__7;
-static PyObject *__pyx_codeobj__30;
+static PyObject *__pyx_codeobj__29;
 /* Late includes */
 
-/* "dwave/gate/simulator/simulator.pyx":44
+/* "dwave/gate/simulator/simulator.pyx":45
  * 
  * 
  * def apply_instruction(             # <<<<<<<<<<<<<<
  *     num_qubits: int,
  *     state: np.ndarray,
  */
 
@@ -3273,15 +3275,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("apply_instruction (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_num_qubits,&__pyx_n_s_state,&__pyx_n_s_op,&__pyx_n_s_targets,&__pyx_n_s_little_endian,&__pyx_n_s_rng,&__pyx_n_s_conjugate_gate,0};
     PyObject* values[7] = {0,0,0,0,0,0,0};
 
-    /* "dwave/gate/simulator/simulator.pyx":51
+    /* "dwave/gate/simulator/simulator.pyx":52
  *     little_endian: bool,
  *     rng: np.random.Generator,
  *     conjugate_gate: bool = False,             # <<<<<<<<<<<<<<
  * ):
  *     if op.is_blocked:
  */
     values[6] = ((PyObject *)Py_False);
@@ -3311,49 +3313,49 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_num_qubits)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_state)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("apply_instruction", 0, 6, 7, 1); __PYX_ERR(0, 44, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("apply_instruction", 0, 6, 7, 1); __PYX_ERR(0, 45, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_op)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("apply_instruction", 0, 6, 7, 2); __PYX_ERR(0, 44, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("apply_instruction", 0, 6, 7, 2); __PYX_ERR(0, 45, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_targets)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("apply_instruction", 0, 6, 7, 3); __PYX_ERR(0, 44, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("apply_instruction", 0, 6, 7, 3); __PYX_ERR(0, 45, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_little_endian)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("apply_instruction", 0, 6, 7, 4); __PYX_ERR(0, 44, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("apply_instruction", 0, 6, 7, 4); __PYX_ERR(0, 45, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_rng)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("apply_instruction", 0, 6, 7, 5); __PYX_ERR(0, 44, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("apply_instruction", 0, 6, 7, 5); __PYX_ERR(0, 45, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_conjugate_gate);
           if (value) { values[6] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "apply_instruction") < 0)) __PYX_ERR(0, 44, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "apply_instruction") < 0)) __PYX_ERR(0, 45, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  7: values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
         CYTHON_FALLTHROUGH;
         case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
         values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
@@ -3371,24 +3373,24 @@
     __pyx_v_targets = values[3];
     __pyx_v_little_endian = values[4];
     __pyx_v_rng = values[5];
     __pyx_v_conjugate_gate = values[6];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("apply_instruction", 0, 6, 7, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 44, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("apply_instruction", 0, 6, 7, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 45, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("dwave.gate.simulator.simulator.apply_instruction", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_state), __pyx_ptype_5numpy_ndarray, 1, "state", 0))) __PYX_ERR(0, 46, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_state), __pyx_ptype_5numpy_ndarray, 1, "state", 0))) __PYX_ERR(0, 47, __pyx_L1_error)
   __pyx_r = __pyx_pf_5dwave_4gate_9simulator_9simulator_apply_instruction(__pyx_self, __pyx_v_num_qubits, __pyx_v_state, __pyx_v_op, __pyx_v_targets, __pyx_v_little_endian, __pyx_v_rng, __pyx_v_conjugate_gate);
 
-  /* "dwave/gate/simulator/simulator.pyx":44
+  /* "dwave/gate/simulator/simulator.pyx":45
  * 
  * 
  * def apply_instruction(             # <<<<<<<<<<<<<<
  *     num_qubits: int,
  *     state: np.ndarray,
  */
 
@@ -3432,127 +3434,127 @@
   struct __pyx_opt_args_5dwave_4gate_9simulator_3ops_apply_gate_control __pyx_t_18;
   struct __pyx_opt_args_5dwave_4gate_9simulator_3ops_single_qubit __pyx_t_19;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceFrameInit(__pyx_codeobj_)
   __Pyx_RefNannySetupContext("apply_instruction", 0);
-  __Pyx_TraceCall("apply_instruction", __pyx_f[0], 44, 0, __PYX_ERR(0, 44, __pyx_L1_error));
+  __Pyx_TraceCall("apply_instruction", __pyx_f[0], 45, 0, __PYX_ERR(0, 45, __pyx_L1_error));
 
-  /* "dwave/gate/simulator/simulator.pyx":53
+  /* "dwave/gate/simulator/simulator.pyx":54
  *     conjugate_gate: bool = False,
  * ):
  *     if op.is_blocked:             # <<<<<<<<<<<<<<
  *         return
  * 
  */
-  __Pyx_TraceLine(53,0,__PYX_ERR(0, 53, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_op, __pyx_n_s_is_blocked); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_TraceLine(54,0,__PYX_ERR(0, 54, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_op, __pyx_n_s_is_blocked); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
-    /* "dwave/gate/simulator/simulator.pyx":54
+    /* "dwave/gate/simulator/simulator.pyx":55
  * ):
  *     if op.is_blocked:
  *         return             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(op, ops.Measurement):
  */
-    __Pyx_TraceLine(54,0,__PYX_ERR(0, 54, __pyx_L1_error))
+    __Pyx_TraceLine(55,0,__PYX_ERR(0, 55, __pyx_L1_error))
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "dwave/gate/simulator/simulator.pyx":53
+    /* "dwave/gate/simulator/simulator.pyx":54
  *     conjugate_gate: bool = False,
  * ):
  *     if op.is_blocked:             # <<<<<<<<<<<<<<
  *         return
  * 
  */
   }
 
-  /* "dwave/gate/simulator/simulator.pyx":56
+  /* "dwave/gate/simulator/simulator.pyx":57
  *         return
  * 
  *     if isinstance(op, ops.Measurement):             # <<<<<<<<<<<<<<
  *         if little_endian:
  *             raise CircuitError("Measurements only supports big-endian qubit indexing.")
  */
-  __Pyx_TraceLine(56,0,__PYX_ERR(0, 56, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_ops); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __Pyx_TraceLine(57,0,__PYX_ERR(0, 57, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_ops); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Measurement); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Measurement); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_2 = PyObject_IsInstance(__pyx_v_op, __pyx_t_3); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_t_2 = PyObject_IsInstance(__pyx_v_op, __pyx_t_3); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_4 = (__pyx_t_2 != 0);
   if (__pyx_t_4) {
 
-    /* "dwave/gate/simulator/simulator.pyx":57
+    /* "dwave/gate/simulator/simulator.pyx":58
  * 
  *     if isinstance(op, ops.Measurement):
  *         if little_endian:             # <<<<<<<<<<<<<<
  *             raise CircuitError("Measurements only supports big-endian qubit indexing.")
  *         _measure(op, state, targets, rng)
  */
-    __Pyx_TraceLine(57,0,__PYX_ERR(0, 57, __pyx_L1_error))
-    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_little_endian); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 57, __pyx_L1_error)
+    __Pyx_TraceLine(58,0,__PYX_ERR(0, 58, __pyx_L1_error))
+    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_little_endian); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 58, __pyx_L1_error)
     if (unlikely(__pyx_t_4)) {
 
-      /* "dwave/gate/simulator/simulator.pyx":58
+      /* "dwave/gate/simulator/simulator.pyx":59
  *     if isinstance(op, ops.Measurement):
  *         if little_endian:
  *             raise CircuitError("Measurements only supports big-endian qubit indexing.")             # <<<<<<<<<<<<<<
  *         _measure(op, state, targets, rng)
  * 
  */
-      __Pyx_TraceLine(58,0,__PYX_ERR(0, 58, __pyx_L1_error))
-      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_CircuitError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
+      __Pyx_TraceLine(59,0,__PYX_ERR(0, 59, __pyx_L1_error))
+      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_CircuitError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 59, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_5 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
         __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
         if (likely(__pyx_t_5)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
           __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_1, function);
         }
       }
       __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_kp_u_Measurements_only_supports_big_e) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_kp_u_Measurements_only_supports_big_e);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 58, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 59, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(0, 58, __pyx_L1_error)
+      __PYX_ERR(0, 59, __pyx_L1_error)
 
-      /* "dwave/gate/simulator/simulator.pyx":57
+      /* "dwave/gate/simulator/simulator.pyx":58
  * 
  *     if isinstance(op, ops.Measurement):
  *         if little_endian:             # <<<<<<<<<<<<<<
  *             raise CircuitError("Measurements only supports big-endian qubit indexing.")
  *         _measure(op, state, targets, rng)
  */
     }
 
-    /* "dwave/gate/simulator/simulator.pyx":59
+    /* "dwave/gate/simulator/simulator.pyx":60
  *         if little_endian:
  *             raise CircuitError("Measurements only supports big-endian qubit indexing.")
  *         _measure(op, state, targets, rng)             # <<<<<<<<<<<<<<
  * 
  *     elif isinstance(op, ops.SWAP):
  */
-    __Pyx_TraceLine(59,0,__PYX_ERR(0, 59, __pyx_L1_error))
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_measure); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 59, __pyx_L1_error)
+    __Pyx_TraceLine(60,0,__PYX_ERR(0, 60, __pyx_L1_error))
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_measure); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_5 = NULL;
     __pyx_t_6 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
@@ -3561,29 +3563,29 @@
         __Pyx_DECREF_SET(__pyx_t_1, function);
         __pyx_t_6 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_1)) {
       PyObject *__pyx_temp[5] = {__pyx_t_5, __pyx_v_op, ((PyObject *)__pyx_v_state), __pyx_v_targets, __pyx_v_rng};
-      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_6, 4+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 59, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_6, 4+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 60, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_3);
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
       PyObject *__pyx_temp[5] = {__pyx_t_5, __pyx_v_op, ((PyObject *)__pyx_v_state), __pyx_v_targets, __pyx_v_rng};
-      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_6, 4+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 59, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_6, 4+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 60, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_3);
     } else
     #endif
     {
-      __pyx_t_7 = PyTuple_New(4+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 59, __pyx_L1_error)
+      __pyx_t_7 = PyTuple_New(4+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 60, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       if (__pyx_t_5) {
         __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
       }
       __Pyx_INCREF(__pyx_v_op);
       __Pyx_GIVEREF(__pyx_v_op);
       PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_v_op);
@@ -3592,581 +3594,581 @@
       PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, ((PyObject *)__pyx_v_state));
       __Pyx_INCREF(__pyx_v_targets);
       __Pyx_GIVEREF(__pyx_v_targets);
       PyTuple_SET_ITEM(__pyx_t_7, 2+__pyx_t_6, __pyx_v_targets);
       __Pyx_INCREF(__pyx_v_rng);
       __Pyx_GIVEREF(__pyx_v_rng);
       PyTuple_SET_ITEM(__pyx_t_7, 3+__pyx_t_6, __pyx_v_rng);
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 59, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 60, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "dwave/gate/simulator/simulator.pyx":56
+    /* "dwave/gate/simulator/simulator.pyx":57
  *         return
  * 
  *     if isinstance(op, ops.Measurement):             # <<<<<<<<<<<<<<
  *         if little_endian:
  *             raise CircuitError("Measurements only supports big-endian qubit indexing.")
  */
     goto __pyx_L4;
   }
 
-  /* "dwave/gate/simulator/simulator.pyx":61
+  /* "dwave/gate/simulator/simulator.pyx":62
  *         _measure(op, state, targets, rng)
  * 
  *     elif isinstance(op, ops.SWAP):             # <<<<<<<<<<<<<<
  *         gate = op.matrix
  *         target0 = targets[1]
  */
-  __Pyx_TraceLine(61,0,__PYX_ERR(0, 61, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_ops); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 61, __pyx_L1_error)
+  __Pyx_TraceLine(62,0,__PYX_ERR(0, 62, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_ops); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_SWAP); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 61, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_SWAP); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_4 = PyObject_IsInstance(__pyx_v_op, __pyx_t_1); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 61, __pyx_L1_error)
+  __pyx_t_4 = PyObject_IsInstance(__pyx_v_op, __pyx_t_1); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_2 = (__pyx_t_4 != 0);
   if (__pyx_t_2) {
 
-    /* "dwave/gate/simulator/simulator.pyx":62
+    /* "dwave/gate/simulator/simulator.pyx":63
  * 
  *     elif isinstance(op, ops.SWAP):
  *         gate = op.matrix             # <<<<<<<<<<<<<<
  *         target0 = targets[1]
  *         target1 = targets[0]
  */
-    __Pyx_TraceLine(62,0,__PYX_ERR(0, 62, __pyx_L1_error))
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_op, __pyx_n_s_matrix); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
+    __Pyx_TraceLine(63,0,__PYX_ERR(0, 63, __pyx_L1_error))
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_op, __pyx_n_s_matrix); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_gate = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "dwave/gate/simulator/simulator.pyx":63
+    /* "dwave/gate/simulator/simulator.pyx":64
  *     elif isinstance(op, ops.SWAP):
  *         gate = op.matrix
  *         target0 = targets[1]             # <<<<<<<<<<<<<<
  *         target1 = targets[0]
  *         apply_swap(
  */
-    __Pyx_TraceLine(63,0,__PYX_ERR(0, 63, __pyx_L1_error))
-    __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_targets, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
+    __Pyx_TraceLine(64,0,__PYX_ERR(0, 64, __pyx_L1_error))
+    __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_targets, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_target0 = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "dwave/gate/simulator/simulator.pyx":64
+    /* "dwave/gate/simulator/simulator.pyx":65
  *         gate = op.matrix
  *         target0 = targets[1]
  *         target1 = targets[0]             # <<<<<<<<<<<<<<
  *         apply_swap(
  *             num_qubits, state, gate, target0, target1,
  */
-    __Pyx_TraceLine(64,0,__PYX_ERR(0, 64, __pyx_L1_error))
-    __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_targets, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
+    __Pyx_TraceLine(65,0,__PYX_ERR(0, 65, __pyx_L1_error))
+    __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_targets, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_target1 = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "dwave/gate/simulator/simulator.pyx":66
+    /* "dwave/gate/simulator/simulator.pyx":67
  *         target1 = targets[0]
  *         apply_swap(
  *             num_qubits, state, gate, target0, target1,             # <<<<<<<<<<<<<<
  *             little_endian=little_endian,
  *         )
  */
-    __Pyx_TraceLine(66,0,__PYX_ERR(0, 66, __pyx_L1_error))
-    __pyx_t_8 = __Pyx_PyInt_As_uint64_t(__pyx_v_num_qubits); if (unlikely((__pyx_t_8 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 66, __pyx_L1_error)
-    __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dc___pyx_t_double_complex(((PyObject *)__pyx_v_state), PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 66, __pyx_L1_error)
-    __pyx_t_10 = __Pyx_PyObject_to_MemoryviewSlice_dsds___pyx_t_double_complex(__pyx_v_gate, PyBUF_WRITABLE); if (unlikely(!__pyx_t_10.memview)) __PYX_ERR(0, 66, __pyx_L1_error)
-    __pyx_t_11 = __Pyx_PyInt_As_uint64_t(__pyx_v_target0); if (unlikely((__pyx_t_11 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 66, __pyx_L1_error)
-    __pyx_t_12 = __Pyx_PyInt_As_uint64_t(__pyx_v_target1); if (unlikely((__pyx_t_12 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 66, __pyx_L1_error)
+    __Pyx_TraceLine(67,0,__PYX_ERR(0, 67, __pyx_L1_error))
+    __pyx_t_8 = __Pyx_PyInt_As_uint64_t(__pyx_v_num_qubits); if (unlikely((__pyx_t_8 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 67, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dc___pyx_t_double_complex(((PyObject *)__pyx_v_state), PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 67, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_to_MemoryviewSlice_dsds___pyx_t_double_complex(__pyx_v_gate, PyBUF_WRITABLE); if (unlikely(!__pyx_t_10.memview)) __PYX_ERR(0, 67, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyInt_As_uint64_t(__pyx_v_target0); if (unlikely((__pyx_t_11 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 67, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyInt_As_uint64_t(__pyx_v_target1); if (unlikely((__pyx_t_12 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 67, __pyx_L1_error)
 
-    /* "dwave/gate/simulator/simulator.pyx":65
+    /* "dwave/gate/simulator/simulator.pyx":66
  *         target0 = targets[1]
  *         target1 = targets[0]
  *         apply_swap(             # <<<<<<<<<<<<<<
  *             num_qubits, state, gate, target0, target1,
  *             little_endian=little_endian,
  */
-    __Pyx_TraceLine(65,0,__PYX_ERR(0, 65, __pyx_L1_error))
+    __Pyx_TraceLine(66,0,__PYX_ERR(0, 66, __pyx_L1_error))
     __pyx_t_13.__pyx_n = 1;
     __pyx_t_13.little_endian = __pyx_v_little_endian;
-    __pyx_t_1 = __pyx_f_5dwave_4gate_9simulator_3ops_apply_swap(__pyx_t_8, __pyx_t_9, __pyx_t_10, __pyx_t_11, __pyx_t_12, &__pyx_t_13); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_5dwave_4gate_9simulator_3ops_apply_swap(__pyx_t_8, __pyx_t_9, __pyx_t_10, __pyx_t_11, __pyx_t_12, &__pyx_t_13); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __PYX_XDEC_MEMVIEW(&__pyx_t_9, 1);
     __pyx_t_9.memview = NULL;
     __pyx_t_9.data = NULL;
     __PYX_XDEC_MEMVIEW(&__pyx_t_10, 1);
     __pyx_t_10.memview = NULL;
     __pyx_t_10.data = NULL;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "dwave/gate/simulator/simulator.pyx":61
+    /* "dwave/gate/simulator/simulator.pyx":62
  *         _measure(op, state, targets, rng)
  * 
  *     elif isinstance(op, ops.SWAP):             # <<<<<<<<<<<<<<
  *         gate = op.matrix
  *         target0 = targets[1]
  */
     goto __pyx_L4;
   }
 
-  /* "dwave/gate/simulator/simulator.pyx":70
+  /* "dwave/gate/simulator/simulator.pyx":71
  *         )
  * 
  *     elif isinstance(op, ops.CSWAP):             # <<<<<<<<<<<<<<
  *         gate = op.matrix
  *         target0 = targets[1]
  */
-  __Pyx_TraceLine(70,0,__PYX_ERR(0, 70, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_ops); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __Pyx_TraceLine(71,0,__PYX_ERR(0, 71, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_ops); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_CSWAP); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_CSWAP); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_2 = PyObject_IsInstance(__pyx_v_op, __pyx_t_3); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_2 = PyObject_IsInstance(__pyx_v_op, __pyx_t_3); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_4 = (__pyx_t_2 != 0);
   if (__pyx_t_4) {
 
-    /* "dwave/gate/simulator/simulator.pyx":71
+    /* "dwave/gate/simulator/simulator.pyx":72
  * 
  *     elif isinstance(op, ops.CSWAP):
  *         gate = op.matrix             # <<<<<<<<<<<<<<
  *         target0 = targets[1]
  *         target1 = targets[2]
  */
-    __Pyx_TraceLine(71,0,__PYX_ERR(0, 71, __pyx_L1_error))
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_op, __pyx_n_s_matrix); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 71, __pyx_L1_error)
+    __Pyx_TraceLine(72,0,__PYX_ERR(0, 72, __pyx_L1_error))
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_op, __pyx_n_s_matrix); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 72, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_v_gate = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "dwave/gate/simulator/simulator.pyx":72
+    /* "dwave/gate/simulator/simulator.pyx":73
  *     elif isinstance(op, ops.CSWAP):
  *         gate = op.matrix
  *         target0 = targets[1]             # <<<<<<<<<<<<<<
  *         target1 = targets[2]
  *         control = targets[0]
  */
-    __Pyx_TraceLine(72,0,__PYX_ERR(0, 72, __pyx_L1_error))
-    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_targets, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 72, __pyx_L1_error)
+    __Pyx_TraceLine(73,0,__PYX_ERR(0, 73, __pyx_L1_error))
+    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_targets, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_v_target0 = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "dwave/gate/simulator/simulator.pyx":73
+    /* "dwave/gate/simulator/simulator.pyx":74
  *         gate = op.matrix
  *         target0 = targets[1]
  *         target1 = targets[2]             # <<<<<<<<<<<<<<
  *         control = targets[0]
  *         apply_cswap(
  */
-    __Pyx_TraceLine(73,0,__PYX_ERR(0, 73, __pyx_L1_error))
-    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_targets, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
+    __Pyx_TraceLine(74,0,__PYX_ERR(0, 74, __pyx_L1_error))
+    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_targets, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 74, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_v_target1 = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "dwave/gate/simulator/simulator.pyx":74
+    /* "dwave/gate/simulator/simulator.pyx":75
  *         target0 = targets[1]
  *         target1 = targets[2]
  *         control = targets[0]             # <<<<<<<<<<<<<<
  *         apply_cswap(
  *             num_qubits, state, gate, target0, target1, control,
  */
-    __Pyx_TraceLine(74,0,__PYX_ERR(0, 74, __pyx_L1_error))
-    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_targets, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 74, __pyx_L1_error)
+    __Pyx_TraceLine(75,0,__PYX_ERR(0, 75, __pyx_L1_error))
+    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_targets, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 75, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_v_control = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "dwave/gate/simulator/simulator.pyx":76
+    /* "dwave/gate/simulator/simulator.pyx":77
  *         control = targets[0]
  *         apply_cswap(
  *             num_qubits, state, gate, target0, target1, control,             # <<<<<<<<<<<<<<
  *             little_endian=little_endian,
  *         )
  */
-    __Pyx_TraceLine(76,0,__PYX_ERR(0, 76, __pyx_L1_error))
-    __pyx_t_12 = __Pyx_PyInt_As_uint64_t(__pyx_v_num_qubits); if (unlikely((__pyx_t_12 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 76, __pyx_L1_error)
-    __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dc___pyx_t_double_complex(((PyObject *)__pyx_v_state), PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 76, __pyx_L1_error)
-    __pyx_t_10 = __Pyx_PyObject_to_MemoryviewSlice_dsds___pyx_t_double_complex(__pyx_v_gate, PyBUF_WRITABLE); if (unlikely(!__pyx_t_10.memview)) __PYX_ERR(0, 76, __pyx_L1_error)
-    __pyx_t_11 = __Pyx_PyInt_As_uint64_t(__pyx_v_target0); if (unlikely((__pyx_t_11 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 76, __pyx_L1_error)
-    __pyx_t_8 = __Pyx_PyInt_As_uint64_t(__pyx_v_target1); if (unlikely((__pyx_t_8 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 76, __pyx_L1_error)
-    __pyx_t_14 = __Pyx_PyInt_As_uint64_t(__pyx_v_control); if (unlikely((__pyx_t_14 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 76, __pyx_L1_error)
+    __Pyx_TraceLine(77,0,__PYX_ERR(0, 77, __pyx_L1_error))
+    __pyx_t_12 = __Pyx_PyInt_As_uint64_t(__pyx_v_num_qubits); if (unlikely((__pyx_t_12 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 77, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dc___pyx_t_double_complex(((PyObject *)__pyx_v_state), PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 77, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_to_MemoryviewSlice_dsds___pyx_t_double_complex(__pyx_v_gate, PyBUF_WRITABLE); if (unlikely(!__pyx_t_10.memview)) __PYX_ERR(0, 77, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyInt_As_uint64_t(__pyx_v_target0); if (unlikely((__pyx_t_11 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 77, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_As_uint64_t(__pyx_v_target1); if (unlikely((__pyx_t_8 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 77, __pyx_L1_error)
+    __pyx_t_14 = __Pyx_PyInt_As_uint64_t(__pyx_v_control); if (unlikely((__pyx_t_14 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 77, __pyx_L1_error)
 
-    /* "dwave/gate/simulator/simulator.pyx":75
+    /* "dwave/gate/simulator/simulator.pyx":76
  *         target1 = targets[2]
  *         control = targets[0]
  *         apply_cswap(             # <<<<<<<<<<<<<<
  *             num_qubits, state, gate, target0, target1, control,
  *             little_endian=little_endian,
  */
-    __Pyx_TraceLine(75,0,__PYX_ERR(0, 75, __pyx_L1_error))
+    __Pyx_TraceLine(76,0,__PYX_ERR(0, 76, __pyx_L1_error))
     __pyx_t_15.__pyx_n = 1;
     __pyx_t_15.little_endian = __pyx_v_little_endian;
-    __pyx_t_3 = __pyx_f_5dwave_4gate_9simulator_3ops_apply_cswap(__pyx_t_12, __pyx_t_9, __pyx_t_10, __pyx_t_11, __pyx_t_8, __pyx_t_14, &__pyx_t_15); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 75, __pyx_L1_error)
+    __pyx_t_3 = __pyx_f_5dwave_4gate_9simulator_3ops_apply_cswap(__pyx_t_12, __pyx_t_9, __pyx_t_10, __pyx_t_11, __pyx_t_8, __pyx_t_14, &__pyx_t_15); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 76, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __PYX_XDEC_MEMVIEW(&__pyx_t_9, 1);
     __pyx_t_9.memview = NULL;
     __pyx_t_9.data = NULL;
     __PYX_XDEC_MEMVIEW(&__pyx_t_10, 1);
     __pyx_t_10.memview = NULL;
     __pyx_t_10.data = NULL;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "dwave/gate/simulator/simulator.pyx":70
+    /* "dwave/gate/simulator/simulator.pyx":71
  *         )
  * 
  *     elif isinstance(op, ops.CSWAP):             # <<<<<<<<<<<<<<
  *         gate = op.matrix
  *         target0 = targets[1]
  */
     goto __pyx_L4;
   }
 
-  /* "dwave/gate/simulator/simulator.pyx":80
+  /* "dwave/gate/simulator/simulator.pyx":81
  *         )
  * 
  *     elif isinstance(op, ops.CCX):             # <<<<<<<<<<<<<<
  *         # this one has to hardcoded for now because ops.ControlledOperation
  *         # doesn't support more than one control yet
  */
-  __Pyx_TraceLine(80,0,__PYX_ERR(0, 80, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_ops); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __Pyx_TraceLine(81,0,__PYX_ERR(0, 81, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_ops); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_CCX); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_CCX); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_4 = PyObject_IsInstance(__pyx_v_op, __pyx_t_1); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 80, __pyx_L1_error)
+  __pyx_t_4 = PyObject_IsInstance(__pyx_v_op, __pyx_t_1); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_2 = (__pyx_t_4 != 0);
   if (__pyx_t_2) {
 
-    /* "dwave/gate/simulator/simulator.pyx":83
+    /* "dwave/gate/simulator/simulator.pyx":84
  *         # this one has to hardcoded for now because ops.ControlledOperation
  *         # doesn't support more than one control yet
  *         gate = np.array([[0, 1], [1, 0]], dtype=np.complex128)             # <<<<<<<<<<<<<<
  *         target = targets[2]
  *         control0 = targets[0]
  */
-    __Pyx_TraceLine(83,0,__PYX_ERR(0, 83, __pyx_L1_error))
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 83, __pyx_L1_error)
+    __Pyx_TraceLine(84,0,__PYX_ERR(0, 84, __pyx_L1_error))
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 84, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_array); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 83, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_array); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 84, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 83, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 84, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_int_0);
     __Pyx_GIVEREF(__pyx_int_0);
     PyList_SET_ITEM(__pyx_t_1, 0, __pyx_int_0);
     __Pyx_INCREF(__pyx_int_1);
     __Pyx_GIVEREF(__pyx_int_1);
     PyList_SET_ITEM(__pyx_t_1, 1, __pyx_int_1);
-    __pyx_t_7 = PyList_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 83, __pyx_L1_error)
+    __pyx_t_7 = PyList_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 84, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_INCREF(__pyx_int_1);
     __Pyx_GIVEREF(__pyx_int_1);
     PyList_SET_ITEM(__pyx_t_7, 0, __pyx_int_1);
     __Pyx_INCREF(__pyx_int_0);
     __Pyx_GIVEREF(__pyx_int_0);
     PyList_SET_ITEM(__pyx_t_7, 1, __pyx_int_0);
-    __pyx_t_5 = PyList_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 83, __pyx_L1_error)
+    __pyx_t_5 = PyList_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 84, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_1);
     PyList_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_7);
     PyList_SET_ITEM(__pyx_t_5, 1, __pyx_t_7);
     __pyx_t_1 = 0;
     __pyx_t_7 = 0;
-    __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 83, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 84, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5);
     __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 83, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 84, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 83, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 84, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_complex128); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 83, __pyx_L1_error)
+    __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_complex128); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 84, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_16);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_16) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_16) < 0) __PYX_ERR(0, 84, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-    __pyx_t_16 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, __pyx_t_5); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 83, __pyx_L1_error)
+    __pyx_t_16 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, __pyx_t_5); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 84, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_16);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_v_gate = __pyx_t_16;
     __pyx_t_16 = 0;
 
-    /* "dwave/gate/simulator/simulator.pyx":84
+    /* "dwave/gate/simulator/simulator.pyx":85
  *         # doesn't support more than one control yet
  *         gate = np.array([[0, 1], [1, 0]], dtype=np.complex128)
  *         target = targets[2]             # <<<<<<<<<<<<<<
  *         control0 = targets[0]
  *         control1 = targets[1]
  */
-    __Pyx_TraceLine(84,0,__PYX_ERR(0, 84, __pyx_L1_error))
-    __pyx_t_16 = __Pyx_GetItemInt(__pyx_v_targets, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 84, __pyx_L1_error)
+    __Pyx_TraceLine(85,0,__PYX_ERR(0, 85, __pyx_L1_error))
+    __pyx_t_16 = __Pyx_GetItemInt(__pyx_v_targets, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 85, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_16);
     __pyx_v_target = __pyx_t_16;
     __pyx_t_16 = 0;
 
-    /* "dwave/gate/simulator/simulator.pyx":85
+    /* "dwave/gate/simulator/simulator.pyx":86
  *         gate = np.array([[0, 1], [1, 0]], dtype=np.complex128)
  *         target = targets[2]
  *         control0 = targets[0]             # <<<<<<<<<<<<<<
  *         control1 = targets[1]
  *         apply_gate_two_control(
  */
-    __Pyx_TraceLine(85,0,__PYX_ERR(0, 85, __pyx_L1_error))
-    __pyx_t_16 = __Pyx_GetItemInt(__pyx_v_targets, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 85, __pyx_L1_error)
+    __Pyx_TraceLine(86,0,__PYX_ERR(0, 86, __pyx_L1_error))
+    __pyx_t_16 = __Pyx_GetItemInt(__pyx_v_targets, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 86, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_16);
     __pyx_v_control0 = __pyx_t_16;
     __pyx_t_16 = 0;
 
-    /* "dwave/gate/simulator/simulator.pyx":86
+    /* "dwave/gate/simulator/simulator.pyx":87
  *         target = targets[2]
  *         control0 = targets[0]
  *         control1 = targets[1]             # <<<<<<<<<<<<<<
  *         apply_gate_two_control(
  *             num_qubits, state, gate, target, control0, control1,
  */
-    __Pyx_TraceLine(86,0,__PYX_ERR(0, 86, __pyx_L1_error))
-    __pyx_t_16 = __Pyx_GetItemInt(__pyx_v_targets, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 86, __pyx_L1_error)
+    __Pyx_TraceLine(87,0,__PYX_ERR(0, 87, __pyx_L1_error))
+    __pyx_t_16 = __Pyx_GetItemInt(__pyx_v_targets, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 87, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_16);
     __pyx_v_control1 = __pyx_t_16;
     __pyx_t_16 = 0;
 
-    /* "dwave/gate/simulator/simulator.pyx":88
+    /* "dwave/gate/simulator/simulator.pyx":89
  *         control1 = targets[1]
  *         apply_gate_two_control(
  *             num_qubits, state, gate, target, control0, control1,             # <<<<<<<<<<<<<<
  *             little_endian=little_endian,
  *         )
  */
-    __Pyx_TraceLine(88,0,__PYX_ERR(0, 88, __pyx_L1_error))
-    __pyx_t_14 = __Pyx_PyInt_As_uint64_t(__pyx_v_num_qubits); if (unlikely((__pyx_t_14 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 88, __pyx_L1_error)
-    __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dc___pyx_t_double_complex(((PyObject *)__pyx_v_state), PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 88, __pyx_L1_error)
-    __pyx_t_10 = __Pyx_PyObject_to_MemoryviewSlice_dsds___pyx_t_double_complex(__pyx_v_gate, PyBUF_WRITABLE); if (unlikely(!__pyx_t_10.memview)) __PYX_ERR(0, 88, __pyx_L1_error)
-    __pyx_t_8 = __Pyx_PyInt_As_uint64_t(__pyx_v_target); if (unlikely((__pyx_t_8 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 88, __pyx_L1_error)
-    __pyx_t_11 = __Pyx_PyInt_As_uint64_t(__pyx_v_control0); if (unlikely((__pyx_t_11 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 88, __pyx_L1_error)
-    __pyx_t_12 = __Pyx_PyInt_As_uint64_t(__pyx_v_control1); if (unlikely((__pyx_t_12 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 88, __pyx_L1_error)
+    __Pyx_TraceLine(89,0,__PYX_ERR(0, 89, __pyx_L1_error))
+    __pyx_t_14 = __Pyx_PyInt_As_uint64_t(__pyx_v_num_qubits); if (unlikely((__pyx_t_14 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 89, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dc___pyx_t_double_complex(((PyObject *)__pyx_v_state), PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 89, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_to_MemoryviewSlice_dsds___pyx_t_double_complex(__pyx_v_gate, PyBUF_WRITABLE); if (unlikely(!__pyx_t_10.memview)) __PYX_ERR(0, 89, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_As_uint64_t(__pyx_v_target); if (unlikely((__pyx_t_8 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 89, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyInt_As_uint64_t(__pyx_v_control0); if (unlikely((__pyx_t_11 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 89, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyInt_As_uint64_t(__pyx_v_control1); if (unlikely((__pyx_t_12 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 89, __pyx_L1_error)
 
-    /* "dwave/gate/simulator/simulator.pyx":87
+    /* "dwave/gate/simulator/simulator.pyx":88
  *         control0 = targets[0]
  *         control1 = targets[1]
  *         apply_gate_two_control(             # <<<<<<<<<<<<<<
  *             num_qubits, state, gate, target, control0, control1,
  *             little_endian=little_endian,
  */
-    __Pyx_TraceLine(87,0,__PYX_ERR(0, 87, __pyx_L1_error))
+    __Pyx_TraceLine(88,0,__PYX_ERR(0, 88, __pyx_L1_error))
     __pyx_t_17.__pyx_n = 1;
     __pyx_t_17.little_endian = __pyx_v_little_endian;
-    __pyx_t_16 = __pyx_f_5dwave_4gate_9simulator_3ops_apply_gate_two_control(__pyx_t_14, __pyx_t_9, __pyx_t_10, __pyx_t_8, __pyx_t_11, __pyx_t_12, &__pyx_t_17); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 87, __pyx_L1_error)
+    __pyx_t_16 = __pyx_f_5dwave_4gate_9simulator_3ops_apply_gate_two_control(__pyx_t_14, __pyx_t_9, __pyx_t_10, __pyx_t_8, __pyx_t_11, __pyx_t_12, &__pyx_t_17); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 88, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_16);
     __PYX_XDEC_MEMVIEW(&__pyx_t_9, 1);
     __pyx_t_9.memview = NULL;
     __pyx_t_9.data = NULL;
     __PYX_XDEC_MEMVIEW(&__pyx_t_10, 1);
     __pyx_t_10.memview = NULL;
     __pyx_t_10.data = NULL;
     __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
 
-    /* "dwave/gate/simulator/simulator.pyx":80
+    /* "dwave/gate/simulator/simulator.pyx":81
  *         )
  * 
  *     elif isinstance(op, ops.CCX):             # <<<<<<<<<<<<<<
  *         # this one has to hardcoded for now because ops.ControlledOperation
  *         # doesn't support more than one control yet
  */
     goto __pyx_L4;
   }
 
-  /* "dwave/gate/simulator/simulator.pyx":92
+  /* "dwave/gate/simulator/simulator.pyx":93
  *         )
  * 
  *     elif isinstance(op, ops.ControlledOperation):             # <<<<<<<<<<<<<<
  *         # should be single qubit gate with controls
  *         if isinstance(op, ops.ParametricOperation):
  */
-  __Pyx_TraceLine(92,0,__PYX_ERR(0, 92, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_16, __pyx_n_s_ops); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __Pyx_TraceLine(93,0,__PYX_ERR(0, 93, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_16, __pyx_n_s_ops); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_16);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_16, __pyx_n_s_ControlledOperation); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_16, __pyx_n_s_ControlledOperation); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-  __pyx_t_2 = PyObject_IsInstance(__pyx_v_op, __pyx_t_5); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 92, __pyx_L1_error)
+  __pyx_t_2 = PyObject_IsInstance(__pyx_v_op, __pyx_t_5); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_4 = (__pyx_t_2 != 0);
   if (__pyx_t_4) {
 
-    /* "dwave/gate/simulator/simulator.pyx":94
+    /* "dwave/gate/simulator/simulator.pyx":95
  *     elif isinstance(op, ops.ControlledOperation):
  *         # should be single qubit gate with controls
  *         if isinstance(op, ops.ParametricOperation):             # <<<<<<<<<<<<<<
  *             gate = op.target_operation(op.parameters).matrix
  *         else:
  */
-    __Pyx_TraceLine(94,0,__PYX_ERR(0, 94, __pyx_L1_error))
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_ops); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 94, __pyx_L1_error)
+    __Pyx_TraceLine(95,0,__PYX_ERR(0, 95, __pyx_L1_error))
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_ops); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 95, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ParametricOperation); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 94, __pyx_L1_error)
+    __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ParametricOperation); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 95, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_16);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_4 = PyObject_IsInstance(__pyx_v_op, __pyx_t_16); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 94, __pyx_L1_error)
+    __pyx_t_4 = PyObject_IsInstance(__pyx_v_op, __pyx_t_16); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 95, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
     __pyx_t_2 = (__pyx_t_4 != 0);
     if (__pyx_t_2) {
 
-      /* "dwave/gate/simulator/simulator.pyx":95
+      /* "dwave/gate/simulator/simulator.pyx":96
  *         # should be single qubit gate with controls
  *         if isinstance(op, ops.ParametricOperation):
  *             gate = op.target_operation(op.parameters).matrix             # <<<<<<<<<<<<<<
  *         else:
  *             gate = op.target_operation.matrix
  */
-      __Pyx_TraceLine(95,0,__PYX_ERR(0, 95, __pyx_L1_error))
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_op, __pyx_n_s_target_operation); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 95, __pyx_L1_error)
+      __Pyx_TraceLine(96,0,__PYX_ERR(0, 96, __pyx_L1_error))
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_op, __pyx_n_s_target_operation); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 96, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_op, __pyx_n_s_parameters); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 95, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_op, __pyx_n_s_parameters); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 96, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_t_3 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
         __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
         if (likely(__pyx_t_3)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
           __Pyx_INCREF(__pyx_t_3);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_5, function);
         }
       }
       __pyx_t_16 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_t_7) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_7);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 95, __pyx_L1_error)
+      if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 96, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_16);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_16, __pyx_n_s_matrix); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 95, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_16, __pyx_n_s_matrix); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 96, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
       __pyx_v_gate = __pyx_t_5;
       __pyx_t_5 = 0;
 
-      /* "dwave/gate/simulator/simulator.pyx":94
+      /* "dwave/gate/simulator/simulator.pyx":95
  *     elif isinstance(op, ops.ControlledOperation):
  *         # should be single qubit gate with controls
  *         if isinstance(op, ops.ParametricOperation):             # <<<<<<<<<<<<<<
  *             gate = op.target_operation(op.parameters).matrix
  *         else:
  */
       goto __pyx_L6;
     }
 
-    /* "dwave/gate/simulator/simulator.pyx":97
+    /* "dwave/gate/simulator/simulator.pyx":98
  *             gate = op.target_operation(op.parameters).matrix
  *         else:
  *             gate = op.target_operation.matrix             # <<<<<<<<<<<<<<
  *         assert gate.shape == (2, 2), (op, gate)
  *         if conjugate_gate:
  */
-    __Pyx_TraceLine(97,0,__PYX_ERR(0, 97, __pyx_L1_error))
+    __Pyx_TraceLine(98,0,__PYX_ERR(0, 98, __pyx_L1_error))
     /*else*/ {
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_op, __pyx_n_s_target_operation); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 97, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_op, __pyx_n_s_target_operation); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 98, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_matrix); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 97, __pyx_L1_error)
+      __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_matrix); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 98, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_16);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_v_gate = __pyx_t_16;
       __pyx_t_16 = 0;
     }
     __pyx_L6:;
 
-    /* "dwave/gate/simulator/simulator.pyx":98
+    /* "dwave/gate/simulator/simulator.pyx":99
  *         else:
  *             gate = op.target_operation.matrix
  *         assert gate.shape == (2, 2), (op, gate)             # <<<<<<<<<<<<<<
  *         if conjugate_gate:
  *             gate = np.ascontiguousarray(gate.conjugate())
  */
-    __Pyx_TraceLine(98,0,__PYX_ERR(0, 98, __pyx_L1_error))
+    __Pyx_TraceLine(99,0,__PYX_ERR(0, 99, __pyx_L1_error))
     #ifndef CYTHON_WITHOUT_ASSERTIONS
     if (unlikely(!Py_OptimizeFlag)) {
-      __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_v_gate, __pyx_n_s_shape); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 98, __pyx_L1_error)
+      __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_v_gate, __pyx_n_s_shape); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 99, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_16);
-      __pyx_t_5 = PyObject_RichCompare(__pyx_t_16, __pyx_tuple__2, Py_EQ); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 98, __pyx_L1_error)
+      __pyx_t_5 = PyObject_RichCompare(__pyx_t_16, __pyx_tuple__2, Py_EQ); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 99, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-      __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 98, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 99, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       if (unlikely(!__pyx_t_2)) {
-        __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 98, __pyx_L1_error)
+        __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 99, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_INCREF(__pyx_v_op);
         __Pyx_GIVEREF(__pyx_v_op);
         PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_op);
         __Pyx_INCREF(__pyx_v_gate);
         __Pyx_GIVEREF(__pyx_v_gate);
         PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_v_gate);
-        __pyx_t_16 = PyTuple_Pack(1, __pyx_t_5); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 98, __pyx_L1_error)
+        __pyx_t_16 = PyTuple_Pack(1, __pyx_t_5); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 99, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_16);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         PyErr_SetObject(PyExc_AssertionError, __pyx_t_16);
         __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-        __PYX_ERR(0, 98, __pyx_L1_error)
+        __PYX_ERR(0, 99, __pyx_L1_error)
       }
     }
     #endif
 
-    /* "dwave/gate/simulator/simulator.pyx":99
+    /* "dwave/gate/simulator/simulator.pyx":100
  *             gate = op.target_operation.matrix
  *         assert gate.shape == (2, 2), (op, gate)
  *         if conjugate_gate:             # <<<<<<<<<<<<<<
  *             gate = np.ascontiguousarray(gate.conjugate())
  * 
  */
-    __Pyx_TraceLine(99,0,__PYX_ERR(0, 99, __pyx_L1_error))
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_conjugate_gate); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 99, __pyx_L1_error)
+    __Pyx_TraceLine(100,0,__PYX_ERR(0, 100, __pyx_L1_error))
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_conjugate_gate); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 100, __pyx_L1_error)
     if (__pyx_t_2) {
 
-      /* "dwave/gate/simulator/simulator.pyx":100
+      /* "dwave/gate/simulator/simulator.pyx":101
  *         assert gate.shape == (2, 2), (op, gate)
  *         if conjugate_gate:
  *             gate = np.ascontiguousarray(gate.conjugate())             # <<<<<<<<<<<<<<
  * 
  *         if op.num_control == 1:
  */
-      __Pyx_TraceLine(100,0,__PYX_ERR(0, 100, __pyx_L1_error))
-      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 100, __pyx_L1_error)
+      __Pyx_TraceLine(101,0,__PYX_ERR(0, 101, __pyx_L1_error))
+      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 101, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 100, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 101, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_gate, __pyx_n_s_conjugate); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 100, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_gate, __pyx_n_s_conjugate); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 101, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_1 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_1)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
           __Pyx_INCREF(__pyx_t_1);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_3, function);
         }
       }
       __pyx_t_5 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 100, __pyx_L1_error)
+      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 101, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_3 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
         __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_7);
         if (likely(__pyx_t_3)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
@@ -4174,338 +4176,338 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_7, function);
         }
       }
       __pyx_t_16 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_3, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_5);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 100, __pyx_L1_error)
+      if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 101, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_16);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF_SET(__pyx_v_gate, __pyx_t_16);
       __pyx_t_16 = 0;
 
-      /* "dwave/gate/simulator/simulator.pyx":99
+      /* "dwave/gate/simulator/simulator.pyx":100
  *             gate = op.target_operation.matrix
  *         assert gate.shape == (2, 2), (op, gate)
  *         if conjugate_gate:             # <<<<<<<<<<<<<<
  *             gate = np.ascontiguousarray(gate.conjugate())
  * 
  */
     }
 
-    /* "dwave/gate/simulator/simulator.pyx":102
+    /* "dwave/gate/simulator/simulator.pyx":103
  *             gate = np.ascontiguousarray(gate.conjugate())
  * 
  *         if op.num_control == 1:             # <<<<<<<<<<<<<<
  *             target = targets[1]
  *             control = targets[0]
  */
-    __Pyx_TraceLine(102,0,__PYX_ERR(0, 102, __pyx_L1_error))
-    __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_v_op, __pyx_n_s_num_control); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 102, __pyx_L1_error)
+    __Pyx_TraceLine(103,0,__PYX_ERR(0, 103, __pyx_L1_error))
+    __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_v_op, __pyx_n_s_num_control); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 103, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_16);
-    __pyx_t_7 = __Pyx_PyInt_EqObjC(__pyx_t_16, __pyx_int_1, 1, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 102, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_EqObjC(__pyx_t_16, __pyx_int_1, 1, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 103, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 102, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 103, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     if (__pyx_t_2) {
 
-      /* "dwave/gate/simulator/simulator.pyx":103
+      /* "dwave/gate/simulator/simulator.pyx":104
  * 
  *         if op.num_control == 1:
  *             target = targets[1]             # <<<<<<<<<<<<<<
  *             control = targets[0]
  *             apply_gate_control(
  */
-      __Pyx_TraceLine(103,0,__PYX_ERR(0, 103, __pyx_L1_error))
-      __pyx_t_7 = __Pyx_GetItemInt(__pyx_v_targets, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 103, __pyx_L1_error)
+      __Pyx_TraceLine(104,0,__PYX_ERR(0, 104, __pyx_L1_error))
+      __pyx_t_7 = __Pyx_GetItemInt(__pyx_v_targets, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 104, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_v_target = __pyx_t_7;
       __pyx_t_7 = 0;
 
-      /* "dwave/gate/simulator/simulator.pyx":104
+      /* "dwave/gate/simulator/simulator.pyx":105
  *         if op.num_control == 1:
  *             target = targets[1]
  *             control = targets[0]             # <<<<<<<<<<<<<<
  *             apply_gate_control(
  *                 num_qubits, state, gate, target, control,
  */
-      __Pyx_TraceLine(104,0,__PYX_ERR(0, 104, __pyx_L1_error))
-      __pyx_t_7 = __Pyx_GetItemInt(__pyx_v_targets, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 104, __pyx_L1_error)
+      __Pyx_TraceLine(105,0,__PYX_ERR(0, 105, __pyx_L1_error))
+      __pyx_t_7 = __Pyx_GetItemInt(__pyx_v_targets, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 105, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_v_control = __pyx_t_7;
       __pyx_t_7 = 0;
 
-      /* "dwave/gate/simulator/simulator.pyx":106
+      /* "dwave/gate/simulator/simulator.pyx":107
  *             control = targets[0]
  *             apply_gate_control(
  *                 num_qubits, state, gate, target, control,             # <<<<<<<<<<<<<<
  *                 little_endian=little_endian,
  *             )
  */
-      __Pyx_TraceLine(106,0,__PYX_ERR(0, 106, __pyx_L1_error))
-      __pyx_t_12 = __Pyx_PyInt_As_uint64_t(__pyx_v_num_qubits); if (unlikely((__pyx_t_12 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 106, __pyx_L1_error)
-      __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dc___pyx_t_double_complex(((PyObject *)__pyx_v_state), PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 106, __pyx_L1_error)
-      __pyx_t_10 = __Pyx_PyObject_to_MemoryviewSlice_dsds___pyx_t_double_complex(__pyx_v_gate, PyBUF_WRITABLE); if (unlikely(!__pyx_t_10.memview)) __PYX_ERR(0, 106, __pyx_L1_error)
-      __pyx_t_11 = __Pyx_PyInt_As_uint64_t(__pyx_v_target); if (unlikely((__pyx_t_11 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 106, __pyx_L1_error)
-      __pyx_t_8 = __Pyx_PyInt_As_uint64_t(__pyx_v_control); if (unlikely((__pyx_t_8 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 106, __pyx_L1_error)
+      __Pyx_TraceLine(107,0,__PYX_ERR(0, 107, __pyx_L1_error))
+      __pyx_t_12 = __Pyx_PyInt_As_uint64_t(__pyx_v_num_qubits); if (unlikely((__pyx_t_12 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 107, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dc___pyx_t_double_complex(((PyObject *)__pyx_v_state), PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 107, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_to_MemoryviewSlice_dsds___pyx_t_double_complex(__pyx_v_gate, PyBUF_WRITABLE); if (unlikely(!__pyx_t_10.memview)) __PYX_ERR(0, 107, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyInt_As_uint64_t(__pyx_v_target); if (unlikely((__pyx_t_11 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 107, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyInt_As_uint64_t(__pyx_v_control); if (unlikely((__pyx_t_8 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 107, __pyx_L1_error)
 
-      /* "dwave/gate/simulator/simulator.pyx":105
+      /* "dwave/gate/simulator/simulator.pyx":106
  *             target = targets[1]
  *             control = targets[0]
  *             apply_gate_control(             # <<<<<<<<<<<<<<
  *                 num_qubits, state, gate, target, control,
  *                 little_endian=little_endian,
  */
-      __Pyx_TraceLine(105,0,__PYX_ERR(0, 105, __pyx_L1_error))
+      __Pyx_TraceLine(106,0,__PYX_ERR(0, 106, __pyx_L1_error))
       __pyx_t_18.__pyx_n = 1;
       __pyx_t_18.little_endian = __pyx_v_little_endian;
-      __pyx_t_7 = __pyx_f_5dwave_4gate_9simulator_3ops_apply_gate_control(__pyx_t_12, __pyx_t_9, __pyx_t_10, __pyx_t_11, __pyx_t_8, &__pyx_t_18); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 105, __pyx_L1_error)
+      __pyx_t_7 = __pyx_f_5dwave_4gate_9simulator_3ops_apply_gate_control(__pyx_t_12, __pyx_t_9, __pyx_t_10, __pyx_t_11, __pyx_t_8, &__pyx_t_18); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 106, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __PYX_XDEC_MEMVIEW(&__pyx_t_9, 1);
       __pyx_t_9.memview = NULL;
       __pyx_t_9.data = NULL;
       __PYX_XDEC_MEMVIEW(&__pyx_t_10, 1);
       __pyx_t_10.memview = NULL;
       __pyx_t_10.data = NULL;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "dwave/gate/simulator/simulator.pyx":102
+      /* "dwave/gate/simulator/simulator.pyx":103
  *             gate = np.ascontiguousarray(gate.conjugate())
  * 
  *         if op.num_control == 1:             # <<<<<<<<<<<<<<
  *             target = targets[1]
  *             control = targets[0]
  */
       goto __pyx_L8;
     }
 
-    /* "dwave/gate/simulator/simulator.pyx":110
+    /* "dwave/gate/simulator/simulator.pyx":111
  *             )
  * 
  *         elif op.num_control == 2:             # <<<<<<<<<<<<<<
  *             target = targets[2]
  *             control0 = targets[0]
  */
-    __Pyx_TraceLine(110,0,__PYX_ERR(0, 110, __pyx_L1_error))
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_op, __pyx_n_s_num_control); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 110, __pyx_L1_error)
+    __Pyx_TraceLine(111,0,__PYX_ERR(0, 111, __pyx_L1_error))
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_op, __pyx_n_s_num_control); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 111, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_16 = __Pyx_PyInt_EqObjC(__pyx_t_7, __pyx_int_2, 2, 0); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 110, __pyx_L1_error)
+    __pyx_t_16 = __Pyx_PyInt_EqObjC(__pyx_t_7, __pyx_int_2, 2, 0); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 111, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_16);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_16); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 110, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_16); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 111, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
     if (__pyx_t_2) {
 
-      /* "dwave/gate/simulator/simulator.pyx":111
+      /* "dwave/gate/simulator/simulator.pyx":112
  * 
  *         elif op.num_control == 2:
  *             target = targets[2]             # <<<<<<<<<<<<<<
  *             control0 = targets[0]
  *             control1 = targets[1]
  */
-      __Pyx_TraceLine(111,0,__PYX_ERR(0, 111, __pyx_L1_error))
-      __pyx_t_16 = __Pyx_GetItemInt(__pyx_v_targets, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 111, __pyx_L1_error)
+      __Pyx_TraceLine(112,0,__PYX_ERR(0, 112, __pyx_L1_error))
+      __pyx_t_16 = __Pyx_GetItemInt(__pyx_v_targets, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 112, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_16);
       __pyx_v_target = __pyx_t_16;
       __pyx_t_16 = 0;
 
-      /* "dwave/gate/simulator/simulator.pyx":112
+      /* "dwave/gate/simulator/simulator.pyx":113
  *         elif op.num_control == 2:
  *             target = targets[2]
  *             control0 = targets[0]             # <<<<<<<<<<<<<<
  *             control1 = targets[1]
  * 
  */
-      __Pyx_TraceLine(112,0,__PYX_ERR(0, 112, __pyx_L1_error))
-      __pyx_t_16 = __Pyx_GetItemInt(__pyx_v_targets, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 112, __pyx_L1_error)
+      __Pyx_TraceLine(113,0,__PYX_ERR(0, 113, __pyx_L1_error))
+      __pyx_t_16 = __Pyx_GetItemInt(__pyx_v_targets, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 113, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_16);
       __pyx_v_control0 = __pyx_t_16;
       __pyx_t_16 = 0;
 
-      /* "dwave/gate/simulator/simulator.pyx":113
+      /* "dwave/gate/simulator/simulator.pyx":114
  *             target = targets[2]
  *             control0 = targets[0]
  *             control1 = targets[1]             # <<<<<<<<<<<<<<
  * 
  *             apply_gate_two_control(
  */
-      __Pyx_TraceLine(113,0,__PYX_ERR(0, 113, __pyx_L1_error))
-      __pyx_t_16 = __Pyx_GetItemInt(__pyx_v_targets, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 113, __pyx_L1_error)
+      __Pyx_TraceLine(114,0,__PYX_ERR(0, 114, __pyx_L1_error))
+      __pyx_t_16 = __Pyx_GetItemInt(__pyx_v_targets, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 114, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_16);
       __pyx_v_control1 = __pyx_t_16;
       __pyx_t_16 = 0;
 
-      /* "dwave/gate/simulator/simulator.pyx":116
+      /* "dwave/gate/simulator/simulator.pyx":117
  * 
  *             apply_gate_two_control(
  *                 num_qubits, state, gate, target, control0, control1,             # <<<<<<<<<<<<<<
  *                 little_endian=little_endian,
  *             )
  */
-      __Pyx_TraceLine(116,0,__PYX_ERR(0, 116, __pyx_L1_error))
-      __pyx_t_8 = __Pyx_PyInt_As_uint64_t(__pyx_v_num_qubits); if (unlikely((__pyx_t_8 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 116, __pyx_L1_error)
-      __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dc___pyx_t_double_complex(((PyObject *)__pyx_v_state), PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 116, __pyx_L1_error)
-      __pyx_t_10 = __Pyx_PyObject_to_MemoryviewSlice_dsds___pyx_t_double_complex(__pyx_v_gate, PyBUF_WRITABLE); if (unlikely(!__pyx_t_10.memview)) __PYX_ERR(0, 116, __pyx_L1_error)
-      __pyx_t_11 = __Pyx_PyInt_As_uint64_t(__pyx_v_target); if (unlikely((__pyx_t_11 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 116, __pyx_L1_error)
-      __pyx_t_12 = __Pyx_PyInt_As_uint64_t(__pyx_v_control0); if (unlikely((__pyx_t_12 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 116, __pyx_L1_error)
-      __pyx_t_14 = __Pyx_PyInt_As_uint64_t(__pyx_v_control1); if (unlikely((__pyx_t_14 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 116, __pyx_L1_error)
+      __Pyx_TraceLine(117,0,__PYX_ERR(0, 117, __pyx_L1_error))
+      __pyx_t_8 = __Pyx_PyInt_As_uint64_t(__pyx_v_num_qubits); if (unlikely((__pyx_t_8 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 117, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dc___pyx_t_double_complex(((PyObject *)__pyx_v_state), PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 117, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_to_MemoryviewSlice_dsds___pyx_t_double_complex(__pyx_v_gate, PyBUF_WRITABLE); if (unlikely(!__pyx_t_10.memview)) __PYX_ERR(0, 117, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyInt_As_uint64_t(__pyx_v_target); if (unlikely((__pyx_t_11 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 117, __pyx_L1_error)
+      __pyx_t_12 = __Pyx_PyInt_As_uint64_t(__pyx_v_control0); if (unlikely((__pyx_t_12 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 117, __pyx_L1_error)
+      __pyx_t_14 = __Pyx_PyInt_As_uint64_t(__pyx_v_control1); if (unlikely((__pyx_t_14 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 117, __pyx_L1_error)
 
-      /* "dwave/gate/simulator/simulator.pyx":115
+      /* "dwave/gate/simulator/simulator.pyx":116
  *             control1 = targets[1]
  * 
  *             apply_gate_two_control(             # <<<<<<<<<<<<<<
  *                 num_qubits, state, gate, target, control0, control1,
  *                 little_endian=little_endian,
  */
-      __Pyx_TraceLine(115,0,__PYX_ERR(0, 115, __pyx_L1_error))
+      __Pyx_TraceLine(116,0,__PYX_ERR(0, 116, __pyx_L1_error))
       __pyx_t_17.__pyx_n = 1;
       __pyx_t_17.little_endian = __pyx_v_little_endian;
-      __pyx_t_16 = __pyx_f_5dwave_4gate_9simulator_3ops_apply_gate_two_control(__pyx_t_8, __pyx_t_9, __pyx_t_10, __pyx_t_11, __pyx_t_12, __pyx_t_14, &__pyx_t_17); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 115, __pyx_L1_error)
+      __pyx_t_16 = __pyx_f_5dwave_4gate_9simulator_3ops_apply_gate_two_control(__pyx_t_8, __pyx_t_9, __pyx_t_10, __pyx_t_11, __pyx_t_12, __pyx_t_14, &__pyx_t_17); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 116, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_16);
       __PYX_XDEC_MEMVIEW(&__pyx_t_9, 1);
       __pyx_t_9.memview = NULL;
       __pyx_t_9.data = NULL;
       __PYX_XDEC_MEMVIEW(&__pyx_t_10, 1);
       __pyx_t_10.memview = NULL;
       __pyx_t_10.data = NULL;
       __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
 
-      /* "dwave/gate/simulator/simulator.pyx":110
+      /* "dwave/gate/simulator/simulator.pyx":111
  *             )
  * 
  *         elif op.num_control == 2:             # <<<<<<<<<<<<<<
  *             target = targets[2]
  *             control0 = targets[0]
  */
     }
     __pyx_L8:;
 
-    /* "dwave/gate/simulator/simulator.pyx":92
+    /* "dwave/gate/simulator/simulator.pyx":93
  *         )
  * 
  *     elif isinstance(op, ops.ControlledOperation):             # <<<<<<<<<<<<<<
  *         # should be single qubit gate with controls
  *         if isinstance(op, ops.ParametricOperation):
  */
     goto __pyx_L4;
   }
 
-  /* "dwave/gate/simulator/simulator.pyx":121
+  /* "dwave/gate/simulator/simulator.pyx":122
  *     else:
  *         # apply single qubit gate
  *         if op.num_qubits != 1:             # <<<<<<<<<<<<<<
  *             raise ValueError(
  *                 f"simulator encountered unknown multi-qubit operation: {op.label}"
  */
-  __Pyx_TraceLine(121,0,__PYX_ERR(0, 121, __pyx_L1_error))
+  __Pyx_TraceLine(122,0,__PYX_ERR(0, 122, __pyx_L1_error))
   /*else*/ {
-    __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_v_op, __pyx_n_s_num_qubits); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 121, __pyx_L1_error)
+    __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_v_op, __pyx_n_s_num_qubits); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 122, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_16);
-    __pyx_t_7 = __Pyx_PyInt_NeObjC(__pyx_t_16, __pyx_int_1, 1, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 121, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_NeObjC(__pyx_t_16, __pyx_int_1, 1, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 122, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 121, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 122, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     if (unlikely(__pyx_t_2)) {
 
-      /* "dwave/gate/simulator/simulator.pyx":123
+      /* "dwave/gate/simulator/simulator.pyx":124
  *         if op.num_qubits != 1:
  *             raise ValueError(
  *                 f"simulator encountered unknown multi-qubit operation: {op.label}"             # <<<<<<<<<<<<<<
  *             )
  *         gate = op.matrix
  */
-      __Pyx_TraceLine(123,0,__PYX_ERR(0, 123, __pyx_L1_error))
-      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_op, __pyx_n_s_label); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 123, __pyx_L1_error)
+      __Pyx_TraceLine(124,0,__PYX_ERR(0, 124, __pyx_L1_error))
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_op, __pyx_n_s_label); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 124, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_16 = __Pyx_PyObject_FormatSimple(__pyx_t_7, __pyx_empty_unicode); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 123, __pyx_L1_error)
+      __pyx_t_16 = __Pyx_PyObject_FormatSimple(__pyx_t_7, __pyx_empty_unicode); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 124, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_16);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __pyx_t_7 = __Pyx_PyUnicode_Concat(__pyx_kp_u_simulator_encountered_unknown_mu, __pyx_t_16); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 123, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyUnicode_Concat(__pyx_kp_u_simulator_encountered_unknown_mu, __pyx_t_16); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 124, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
 
-      /* "dwave/gate/simulator/simulator.pyx":122
+      /* "dwave/gate/simulator/simulator.pyx":123
  *         # apply single qubit gate
  *         if op.num_qubits != 1:
  *             raise ValueError(             # <<<<<<<<<<<<<<
  *                 f"simulator encountered unknown multi-qubit operation: {op.label}"
  *             )
  */
-      __Pyx_TraceLine(122,0,__PYX_ERR(0, 122, __pyx_L1_error))
-      __pyx_t_16 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_7); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 122, __pyx_L1_error)
+      __Pyx_TraceLine(123,0,__PYX_ERR(0, 123, __pyx_L1_error))
+      __pyx_t_16 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_7); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 123, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_16);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_Raise(__pyx_t_16, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-      __PYX_ERR(0, 122, __pyx_L1_error)
+      __PYX_ERR(0, 123, __pyx_L1_error)
 
-      /* "dwave/gate/simulator/simulator.pyx":121
+      /* "dwave/gate/simulator/simulator.pyx":122
  *     else:
  *         # apply single qubit gate
  *         if op.num_qubits != 1:             # <<<<<<<<<<<<<<
  *             raise ValueError(
  *                 f"simulator encountered unknown multi-qubit operation: {op.label}"
  */
     }
 
-    /* "dwave/gate/simulator/simulator.pyx":125
+    /* "dwave/gate/simulator/simulator.pyx":126
  *                 f"simulator encountered unknown multi-qubit operation: {op.label}"
  *             )
  *         gate = op.matrix             # <<<<<<<<<<<<<<
  *         if conjugate_gate:
  *             gate = np.ascontiguousarray(gate.conjugate())
  */
-    __Pyx_TraceLine(125,0,__PYX_ERR(0, 125, __pyx_L1_error))
-    __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_v_op, __pyx_n_s_matrix); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 125, __pyx_L1_error)
+    __Pyx_TraceLine(126,0,__PYX_ERR(0, 126, __pyx_L1_error))
+    __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_v_op, __pyx_n_s_matrix); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 126, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_16);
     __pyx_v_gate = __pyx_t_16;
     __pyx_t_16 = 0;
 
-    /* "dwave/gate/simulator/simulator.pyx":126
+    /* "dwave/gate/simulator/simulator.pyx":127
  *             )
  *         gate = op.matrix
  *         if conjugate_gate:             # <<<<<<<<<<<<<<
  *             gate = np.ascontiguousarray(gate.conjugate())
  * 
  */
-    __Pyx_TraceLine(126,0,__PYX_ERR(0, 126, __pyx_L1_error))
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_conjugate_gate); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 126, __pyx_L1_error)
+    __Pyx_TraceLine(127,0,__PYX_ERR(0, 127, __pyx_L1_error))
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_conjugate_gate); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 127, __pyx_L1_error)
     if (__pyx_t_2) {
 
-      /* "dwave/gate/simulator/simulator.pyx":127
+      /* "dwave/gate/simulator/simulator.pyx":128
  *         gate = op.matrix
  *         if conjugate_gate:
  *             gate = np.ascontiguousarray(gate.conjugate())             # <<<<<<<<<<<<<<
  * 
  *         target = targets[0]
  */
-      __Pyx_TraceLine(127,0,__PYX_ERR(0, 127, __pyx_L1_error))
-      __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 127, __pyx_L1_error)
+      __Pyx_TraceLine(128,0,__PYX_ERR(0, 128, __pyx_L1_error))
+      __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 128, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 127, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 128, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_gate, __pyx_n_s_conjugate); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 127, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_gate, __pyx_n_s_conjugate); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 128, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_1 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_1)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
           __Pyx_INCREF(__pyx_t_1);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_3, function);
         }
       }
       __pyx_t_7 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 127, __pyx_L1_error)
+      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 128, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_3 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
         __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
         if (likely(__pyx_t_3)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -4513,69 +4515,69 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_5, function);
         }
       }
       __pyx_t_16 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_t_7) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_7);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 127, __pyx_L1_error)
+      if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 128, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_16);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF_SET(__pyx_v_gate, __pyx_t_16);
       __pyx_t_16 = 0;
 
-      /* "dwave/gate/simulator/simulator.pyx":126
+      /* "dwave/gate/simulator/simulator.pyx":127
  *             )
  *         gate = op.matrix
  *         if conjugate_gate:             # <<<<<<<<<<<<<<
  *             gate = np.ascontiguousarray(gate.conjugate())
  * 
  */
     }
 
-    /* "dwave/gate/simulator/simulator.pyx":129
+    /* "dwave/gate/simulator/simulator.pyx":130
  *             gate = np.ascontiguousarray(gate.conjugate())
  * 
  *         target = targets[0]             # <<<<<<<<<<<<<<
  *         single_qubit(num_qubits, state, gate, target, little_endian=little_endian)
  * 
  */
-    __Pyx_TraceLine(129,0,__PYX_ERR(0, 129, __pyx_L1_error))
-    __pyx_t_16 = __Pyx_GetItemInt(__pyx_v_targets, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 129, __pyx_L1_error)
+    __Pyx_TraceLine(130,0,__PYX_ERR(0, 130, __pyx_L1_error))
+    __pyx_t_16 = __Pyx_GetItemInt(__pyx_v_targets, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 130, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_16);
     __pyx_v_target = __pyx_t_16;
     __pyx_t_16 = 0;
 
-    /* "dwave/gate/simulator/simulator.pyx":130
+    /* "dwave/gate/simulator/simulator.pyx":131
  * 
  *         target = targets[0]
  *         single_qubit(num_qubits, state, gate, target, little_endian=little_endian)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __Pyx_TraceLine(130,0,__PYX_ERR(0, 130, __pyx_L1_error))
-    __pyx_t_14 = __Pyx_PyInt_As_uint64_t(__pyx_v_num_qubits); if (unlikely((__pyx_t_14 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 130, __pyx_L1_error)
-    __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dc___pyx_t_double_complex(((PyObject *)__pyx_v_state), PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 130, __pyx_L1_error)
-    __pyx_t_10 = __Pyx_PyObject_to_MemoryviewSlice_dsds___pyx_t_double_complex(__pyx_v_gate, PyBUF_WRITABLE); if (unlikely(!__pyx_t_10.memview)) __PYX_ERR(0, 130, __pyx_L1_error)
-    __pyx_t_12 = __Pyx_PyInt_As_uint64_t(__pyx_v_target); if (unlikely((__pyx_t_12 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 130, __pyx_L1_error)
+    __Pyx_TraceLine(131,0,__PYX_ERR(0, 131, __pyx_L1_error))
+    __pyx_t_14 = __Pyx_PyInt_As_uint64_t(__pyx_v_num_qubits); if (unlikely((__pyx_t_14 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 131, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dc___pyx_t_double_complex(((PyObject *)__pyx_v_state), PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_to_MemoryviewSlice_dsds___pyx_t_double_complex(__pyx_v_gate, PyBUF_WRITABLE); if (unlikely(!__pyx_t_10.memview)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyInt_As_uint64_t(__pyx_v_target); if (unlikely((__pyx_t_12 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 131, __pyx_L1_error)
     __pyx_t_19.__pyx_n = 1;
     __pyx_t_19.little_endian = __pyx_v_little_endian;
-    __pyx_t_16 = __pyx_f_5dwave_4gate_9simulator_3ops_single_qubit(__pyx_t_14, __pyx_t_9, __pyx_t_10, __pyx_t_12, &__pyx_t_19); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 130, __pyx_L1_error)
+    __pyx_t_16 = __pyx_f_5dwave_4gate_9simulator_3ops_single_qubit(__pyx_t_14, __pyx_t_9, __pyx_t_10, __pyx_t_12, &__pyx_t_19); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 131, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_16);
     __PYX_XDEC_MEMVIEW(&__pyx_t_9, 1);
     __pyx_t_9.memview = NULL;
     __pyx_t_9.data = NULL;
     __PYX_XDEC_MEMVIEW(&__pyx_t_10, 1);
     __pyx_t_10.memview = NULL;
     __pyx_t_10.data = NULL;
     __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
   }
   __pyx_L4:;
 
-  /* "dwave/gate/simulator/simulator.pyx":44
+  /* "dwave/gate/simulator/simulator.pyx":45
  * 
  * 
  * def apply_instruction(             # <<<<<<<<<<<<<<
  *     num_qubits: int,
  *     state: np.ndarray,
  */
 
@@ -4602,25 +4604,25 @@
   __Pyx_XDECREF(__pyx_v_control1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "dwave/gate/simulator/simulator.pyx":133
+/* "dwave/gate/simulator/simulator.pyx":134
  * 
  * 
  * def simulate(             # <<<<<<<<<<<<<<
  *     circuit: Circuit,
  *     mixed_state: bool = False,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_5dwave_4gate_9simulator_9simulator_3simulate(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_5dwave_4gate_9simulator_9simulator_2simulate[] = "Simulate the given circuit with either a state vector or density matrix\n    simulation.\n\n    Args:\n        circuit: The circuit to simulate.\n\n        mixed_state:\n            If true, use the full density matrix method to simulate the circuit.\n            Otherwise, simulate using the state vector method.\n\n        little_endian:\n            If true, return the state vector using little-endian indexing for\n            the qubits. Otherwise use big-endian.\n\n    Returns:\n        The resulting state vector or density matrix.\n\n    ";
+static char __pyx_doc_5dwave_4gate_9simulator_9simulator_2simulate[] = "Simulate the given circuit with either a state vector or density matrix simulation.\n\n    The resulting state is stored in the circuit object, together with the measured value in the\n    classical register.\n\n    Args:\n        circuit: The circuit to simulate.\n\n        mixed_state:\n            If true, use the full density matrix method to simulate the circuit.\n            Otherwise, simulate using the state vector method.\n\n        little_endian:\n            If true, return the state vector using little-endian indexing for\n            the qubits. Otherwise use big-endian.\n\n    ";
 static PyMethodDef __pyx_mdef_5dwave_4gate_9simulator_9simulator_3simulate = {"simulate", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5dwave_4gate_9simulator_9simulator_3simulate, METH_VARARGS|METH_KEYWORDS, __pyx_doc_5dwave_4gate_9simulator_9simulator_2simulate};
 static PyObject *__pyx_pw_5dwave_4gate_9simulator_9simulator_3simulate(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_circuit = 0;
   PyObject *__pyx_v_mixed_state = 0;
   PyObject *__pyx_v_little_endian = 0;
   PyObject *__pyx_v_rng_seed = 0;
   int __pyx_lineno = 0;
@@ -4629,38 +4631,38 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("simulate (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_circuit,&__pyx_n_s_mixed_state,&__pyx_n_s_little_endian,&__pyx_n_s_rng_seed,0};
     PyObject* values[4] = {0,0,0,0};
 
-    /* "dwave/gate/simulator/simulator.pyx":135
+    /* "dwave/gate/simulator/simulator.pyx":136
  * def simulate(
  *     circuit: Circuit,
  *     mixed_state: bool = False,             # <<<<<<<<<<<<<<
  *     little_endian: bool = False,
  *     rng_seed: Optional[int] = None,
  */
     values[1] = ((PyObject *)Py_False);
 
-    /* "dwave/gate/simulator/simulator.pyx":136
+    /* "dwave/gate/simulator/simulator.pyx":137
  *     circuit: Circuit,
  *     mixed_state: bool = False,
  *     little_endian: bool = False,             # <<<<<<<<<<<<<<
  *     rng_seed: Optional[int] = None,
- * ) -> np.typing.NDArray:
+ * ) -> None:
  */
     values[2] = ((PyObject *)Py_False);
 
-    /* "dwave/gate/simulator/simulator.pyx":137
+    /* "dwave/gate/simulator/simulator.pyx":138
  *     mixed_state: bool = False,
  *     little_endian: bool = False,
  *     rng_seed: Optional[int] = None,             # <<<<<<<<<<<<<<
- * ) -> np.typing.NDArray:
- *     """Simulate the given circuit with either a state vector or density matrix
+ * ) -> None:
+ *     """Simulate the given circuit with either a state vector or density matrix simulation.
  */
     values[3] = ((PyObject *)Py_None);
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
@@ -4695,15 +4697,15 @@
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_rng_seed);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "simulate") < 0)) __PYX_ERR(0, 133, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "simulate") < 0)) __PYX_ERR(0, 134, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
@@ -4717,23 +4719,23 @@
     __pyx_v_circuit = values[0];
     __pyx_v_mixed_state = values[1];
     __pyx_v_little_endian = values[2];
     __pyx_v_rng_seed = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("simulate", 0, 1, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 133, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("simulate", 0, 1, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 134, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("dwave.gate.simulator.simulator.simulate", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5dwave_4gate_9simulator_9simulator_2simulate(__pyx_self, __pyx_v_circuit, __pyx_v_mixed_state, __pyx_v_little_endian, __pyx_v_rng_seed);
 
-  /* "dwave/gate/simulator/simulator.pyx":133
+  /* "dwave/gate/simulator/simulator.pyx":134
  * 
  * 
  * def simulate(             # <<<<<<<<<<<<<<
  *     circuit: Circuit,
  *     mixed_state: bool = False,
  */
 
@@ -4752,506 +4754,503 @@
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
-  PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  int __pyx_t_5;
+  PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   Py_ssize_t __pyx_t_8;
   PyObject *(*__pyx_t_9)(PyObject *);
   Py_ssize_t __pyx_t_10;
   PyObject *(*__pyx_t_11)(PyObject *);
   PyObject *__pyx_t_12 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceFrameInit(__pyx_codeobj__3)
   __Pyx_RefNannySetupContext("simulate", 0);
-  __Pyx_TraceCall("simulate", __pyx_f[0], 133, 0, __PYX_ERR(0, 133, __pyx_L1_error));
+  __Pyx_TraceCall("simulate", __pyx_f[0], 134, 0, __PYX_ERR(0, 134, __pyx_L1_error));
 
   /* "dwave/gate/simulator/simulator.pyx":158
  *     """
  * 
  *     num_qubits = circuit.num_qubits             # <<<<<<<<<<<<<<
  *     if num_qubits == 0:
- *         return np.empty(0, dtype=np.complex128)
+ *         return
  */
   __Pyx_TraceLine(158,0,__PYX_ERR(0, 158, __pyx_L1_error))
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_circuit, __pyx_n_s_num_qubits); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 158, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_num_qubits = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "dwave/gate/simulator/simulator.pyx":159
  * 
  *     num_qubits = circuit.num_qubits
  *     if num_qubits == 0:             # <<<<<<<<<<<<<<
- *         return np.empty(0, dtype=np.complex128)
+ *         return
  * 
  */
   __Pyx_TraceLine(159,0,__PYX_ERR(0, 159, __pyx_L1_error))
   __pyx_t_1 = __Pyx_PyInt_EqObjC(__pyx_v_num_qubits, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 159, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 159, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
     /* "dwave/gate/simulator/simulator.pyx":160
  *     num_qubits = circuit.num_qubits
  *     if num_qubits == 0:
- *         return np.empty(0, dtype=np.complex128)             # <<<<<<<<<<<<<<
+ *         return             # <<<<<<<<<<<<<<
  * 
  *     rng = np.random.default_rng(rng_seed)
  */
     __Pyx_TraceLine(160,0,__PYX_ERR(0, 160, __pyx_L1_error))
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 160, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 160, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 160, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 160, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_complex128); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 160, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__4, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 160, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_r = __pyx_t_5;
-    __pyx_t_5 = 0;
+    __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
     /* "dwave/gate/simulator/simulator.pyx":159
  * 
  *     num_qubits = circuit.num_qubits
  *     if num_qubits == 0:             # <<<<<<<<<<<<<<
- *         return np.empty(0, dtype=np.complex128)
+ *         return
  * 
  */
   }
 
   /* "dwave/gate/simulator/simulator.pyx":162
- *         return np.empty(0, dtype=np.complex128)
+ *         return
  * 
  *     rng = np.random.default_rng(rng_seed)             # <<<<<<<<<<<<<<
  * 
  *     if mixed_state:
  */
   __Pyx_TraceLine(162,0,__PYX_ERR(0, 162, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_random); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 162, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 162, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_default_rng); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_random); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 162, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-      __Pyx_INCREF(__pyx_t_3);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_default_rng); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 162, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_4)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_1, function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
-  __pyx_t_5 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_v_rng_seed) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v_rng_seed);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 162, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v_rng = __pyx_t_5;
-  __pyx_t_5 = 0;
+  __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_rng_seed) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_rng_seed);
+  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_v_rng = __pyx_t_1;
+  __pyx_t_1 = 0;
 
   /* "dwave/gate/simulator/simulator.pyx":164
  *     rng = np.random.default_rng(rng_seed)
  * 
  *     if mixed_state:             # <<<<<<<<<<<<<<
- *         return _simulate_circuit_density_matrix(circuit, rng)
- * 
+ *         state = _simulate_circuit_density_matrix(circuit, rng)
+ *     else:
  */
   __Pyx_TraceLine(164,0,__PYX_ERR(0, 164, __pyx_L1_error))
   __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_mixed_state); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 164, __pyx_L1_error)
   if (__pyx_t_2) {
 
     /* "dwave/gate/simulator/simulator.pyx":165
  * 
  *     if mixed_state:
- *         return _simulate_circuit_density_matrix(circuit, rng)             # <<<<<<<<<<<<<<
- * 
- *     state = np.zeros(1 << num_qubits, dtype=np.complex128)
+ *         state = _simulate_circuit_density_matrix(circuit, rng)             # <<<<<<<<<<<<<<
+ *     else:
+ *         state = np.zeros(1 << num_qubits, dtype=np.complex128)
  */
     __Pyx_TraceLine(165,0,__PYX_ERR(0, 165, __pyx_L1_error))
-    __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_simulate_circuit_density_matrix); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 165, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = NULL;
-    __pyx_t_6 = 0;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
-      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
-      if (likely(__pyx_t_3)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-        __Pyx_INCREF(__pyx_t_3);
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_simulate_circuit_density_matrix); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 165, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_4 = NULL;
+    __pyx_t_5 = 0;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
+      if (likely(__pyx_t_4)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+        __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_1, function);
-        __pyx_t_6 = 1;
+        __Pyx_DECREF_SET(__pyx_t_3, function);
+        __pyx_t_5 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(__pyx_t_1)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_circuit, __pyx_v_rng};
-      __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 165, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __Pyx_GOTREF(__pyx_t_5);
+    if (PyFunction_Check(__pyx_t_3)) {
+      PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_circuit, __pyx_v_rng};
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 165, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __Pyx_GOTREF(__pyx_t_1);
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_circuit, __pyx_v_rng};
-      __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 165, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __Pyx_GOTREF(__pyx_t_5);
+    if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
+      PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_circuit, __pyx_v_rng};
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 165, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __Pyx_GOTREF(__pyx_t_1);
     } else
     #endif
     {
-      __pyx_t_4 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 165, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      if (__pyx_t_3) {
-        __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3); __pyx_t_3 = NULL;
+      __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 165, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      if (__pyx_t_4) {
+        __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
       }
       __Pyx_INCREF(__pyx_v_circuit);
       __Pyx_GIVEREF(__pyx_v_circuit);
-      PyTuple_SET_ITEM(__pyx_t_4, 0+__pyx_t_6, __pyx_v_circuit);
+      PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, __pyx_v_circuit);
       __Pyx_INCREF(__pyx_v_rng);
       __Pyx_GIVEREF(__pyx_v_rng);
-      PyTuple_SET_ITEM(__pyx_t_4, 1+__pyx_t_6, __pyx_v_rng);
-      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 165, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, __pyx_v_rng);
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 165, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_r = __pyx_t_5;
-    __pyx_t_5 = 0;
-    goto __pyx_L0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_v_state = __pyx_t_1;
+    __pyx_t_1 = 0;
 
     /* "dwave/gate/simulator/simulator.pyx":164
  *     rng = np.random.default_rng(rng_seed)
  * 
  *     if mixed_state:             # <<<<<<<<<<<<<<
- *         return _simulate_circuit_density_matrix(circuit, rng)
- * 
+ *         state = _simulate_circuit_density_matrix(circuit, rng)
+ *     else:
  */
+    goto __pyx_L4;
   }
 
   /* "dwave/gate/simulator/simulator.pyx":167
- *         return _simulate_circuit_density_matrix(circuit, rng)
- * 
- *     state = np.zeros(1 << num_qubits, dtype=np.complex128)             # <<<<<<<<<<<<<<
- *     state[0] = 1
+ *         state = _simulate_circuit_density_matrix(circuit, rng)
+ *     else:
+ *         state = np.zeros(1 << num_qubits, dtype=np.complex128)             # <<<<<<<<<<<<<<
+ *         state[0] = 1
  * 
  */
   __Pyx_TraceLine(167,0,__PYX_ERR(0, 167, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 167, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyNumber_Lshift(__pyx_int_1, __pyx_v_num_qubits); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 167, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 167, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GIVEREF(__pyx_t_5);
-  PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
-  __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 167, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 167, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_complex128); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 167, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 167, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 167, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_v_state = __pyx_t_7;
-  __pyx_t_7 = 0;
+  /*else*/ {
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 167, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = PyNumber_Lshift(__pyx_int_1, __pyx_v_num_qubits); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 167, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_1);
+    __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 167, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_complex128); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 167, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 167, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, __pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 167, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_v_state = __pyx_t_7;
+    __pyx_t_7 = 0;
 
-  /* "dwave/gate/simulator/simulator.pyx":168
- * 
- *     state = np.zeros(1 << num_qubits, dtype=np.complex128)
- *     state[0] = 1             # <<<<<<<<<<<<<<
+    /* "dwave/gate/simulator/simulator.pyx":168
+ *     else:
+ *         state = np.zeros(1 << num_qubits, dtype=np.complex128)
+ *         state[0] = 1             # <<<<<<<<<<<<<<
  * 
- *     for op in circuit.circuit:
+ *         for op in circuit.circuit:
  */
-  __Pyx_TraceLine(168,0,__PYX_ERR(0, 168, __pyx_L1_error))
-  if (unlikely(__Pyx_SetItemInt(__pyx_v_state, 0, __pyx_int_1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1) < 0)) __PYX_ERR(0, 168, __pyx_L1_error)
+    __Pyx_TraceLine(168,0,__PYX_ERR(0, 168, __pyx_L1_error))
+    if (unlikely(__Pyx_SetItemInt(__pyx_v_state, 0, __pyx_int_1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1) < 0)) __PYX_ERR(0, 168, __pyx_L1_error)
 
-  /* "dwave/gate/simulator/simulator.pyx":170
- *     state[0] = 1
+    /* "dwave/gate/simulator/simulator.pyx":170
+ *         state[0] = 1
  * 
- *     for op in circuit.circuit:             # <<<<<<<<<<<<<<
- *         targets = [circuit.qubits.index(qb) for qb in op.qubits]
- *         apply_instruction(num_qubits, state, op, targets, little_endian, rng)
+ *         for op in circuit.circuit:             # <<<<<<<<<<<<<<
+ *             targets = [circuit.qubits.index(qb) for qb in op.qubits]
+ *             apply_instruction(num_qubits, state, op, targets, little_endian, rng)
  */
-  __Pyx_TraceLine(170,0,__PYX_ERR(0, 170, __pyx_L1_error))
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_circuit, __pyx_n_s_circuit); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 170, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  if (likely(PyList_CheckExact(__pyx_t_7)) || PyTuple_CheckExact(__pyx_t_7)) {
-    __pyx_t_5 = __pyx_t_7; __Pyx_INCREF(__pyx_t_5); __pyx_t_8 = 0;
-    __pyx_t_9 = NULL;
-  } else {
-    __pyx_t_8 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 170, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_9 = Py_TYPE(__pyx_t_5)->tp_iternext; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 170, __pyx_L1_error)
-  }
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  for (;;) {
-    if (likely(!__pyx_t_9)) {
-      if (likely(PyList_CheckExact(__pyx_t_5))) {
-        if (__pyx_t_8 >= PyList_GET_SIZE(__pyx_t_5)) break;
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_7 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_8); __Pyx_INCREF(__pyx_t_7); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 170, __pyx_L1_error)
-        #else
-        __pyx_t_7 = PySequence_ITEM(__pyx_t_5, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 170, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_7);
-        #endif
-      } else {
-        if (__pyx_t_8 >= PyTuple_GET_SIZE(__pyx_t_5)) break;
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_8); __Pyx_INCREF(__pyx_t_7); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 170, __pyx_L1_error)
-        #else
-        __pyx_t_7 = PySequence_ITEM(__pyx_t_5, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 170, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_7);
-        #endif
-      }
+    __Pyx_TraceLine(170,0,__PYX_ERR(0, 170, __pyx_L1_error))
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_circuit, __pyx_n_s_circuit); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 170, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    if (likely(PyList_CheckExact(__pyx_t_7)) || PyTuple_CheckExact(__pyx_t_7)) {
+      __pyx_t_1 = __pyx_t_7; __Pyx_INCREF(__pyx_t_1); __pyx_t_8 = 0;
+      __pyx_t_9 = NULL;
     } else {
-      __pyx_t_7 = __pyx_t_9(__pyx_t_5);
-      if (unlikely(!__pyx_t_7)) {
-        PyObject* exc_type = PyErr_Occurred();
-        if (exc_type) {
-          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 170, __pyx_L1_error)
+      __pyx_t_8 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 170, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_9 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 170, __pyx_L1_error)
+    }
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    for (;;) {
+      if (likely(!__pyx_t_9)) {
+        if (likely(PyList_CheckExact(__pyx_t_1))) {
+          if (__pyx_t_8 >= PyList_GET_SIZE(__pyx_t_1)) break;
+          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_8); __Pyx_INCREF(__pyx_t_7); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 170, __pyx_L1_error)
+          #else
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_1, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 170, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_7);
+          #endif
+        } else {
+          if (__pyx_t_8 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
+          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_8); __Pyx_INCREF(__pyx_t_7); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 170, __pyx_L1_error)
+          #else
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_1, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 170, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_7);
+          #endif
         }
-        break;
+      } else {
+        __pyx_t_7 = __pyx_t_9(__pyx_t_1);
+        if (unlikely(!__pyx_t_7)) {
+          PyObject* exc_type = PyErr_Occurred();
+          if (exc_type) {
+            if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+            else __PYX_ERR(0, 170, __pyx_L1_error)
+          }
+          break;
+        }
+        __Pyx_GOTREF(__pyx_t_7);
       }
-      __Pyx_GOTREF(__pyx_t_7);
-    }
-    __Pyx_XDECREF_SET(__pyx_v_op, __pyx_t_7);
-    __pyx_t_7 = 0;
+      __Pyx_XDECREF_SET(__pyx_v_op, __pyx_t_7);
+      __pyx_t_7 = 0;
 
-    /* "dwave/gate/simulator/simulator.pyx":171
+      /* "dwave/gate/simulator/simulator.pyx":171
  * 
- *     for op in circuit.circuit:
- *         targets = [circuit.qubits.index(qb) for qb in op.qubits]             # <<<<<<<<<<<<<<
- *         apply_instruction(num_qubits, state, op, targets, little_endian, rng)
+ *         for op in circuit.circuit:
+ *             targets = [circuit.qubits.index(qb) for qb in op.qubits]             # <<<<<<<<<<<<<<
+ *             apply_instruction(num_qubits, state, op, targets, little_endian, rng)
  * 
  */
-    __Pyx_TraceLine(171,0,__PYX_ERR(0, 171, __pyx_L1_error))
-    { /* enter inner scope */
-      __pyx_t_7 = PyList_New(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 171, __pyx_L9_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_op, __pyx_n_s_qubits); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 171, __pyx_L9_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      if (likely(PyList_CheckExact(__pyx_t_4)) || PyTuple_CheckExact(__pyx_t_4)) {
-        __pyx_t_1 = __pyx_t_4; __Pyx_INCREF(__pyx_t_1); __pyx_t_10 = 0;
-        __pyx_t_11 = NULL;
-      } else {
-        __pyx_t_10 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 171, __pyx_L9_error)
-        __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_11 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 171, __pyx_L9_error)
-      }
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      for (;;) {
-        if (likely(!__pyx_t_11)) {
-          if (likely(PyList_CheckExact(__pyx_t_1))) {
-            if (__pyx_t_10 >= PyList_GET_SIZE(__pyx_t_1)) break;
-            #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_10); __Pyx_INCREF(__pyx_t_4); __pyx_t_10++; if (unlikely(0 < 0)) __PYX_ERR(0, 171, __pyx_L9_error)
-            #else
-            __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 171, __pyx_L9_error)
-            __Pyx_GOTREF(__pyx_t_4);
-            #endif
-          } else {
-            if (__pyx_t_10 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
-            #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_10); __Pyx_INCREF(__pyx_t_4); __pyx_t_10++; if (unlikely(0 < 0)) __PYX_ERR(0, 171, __pyx_L9_error)
-            #else
-            __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 171, __pyx_L9_error)
-            __Pyx_GOTREF(__pyx_t_4);
-            #endif
-          }
+      __Pyx_TraceLine(171,0,__PYX_ERR(0, 171, __pyx_L1_error))
+      { /* enter inner scope */
+        __pyx_t_7 = PyList_New(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 171, __pyx_L9_error)
+        __Pyx_GOTREF(__pyx_t_7);
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_op, __pyx_n_s_qubits); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 171, __pyx_L9_error)
+        __Pyx_GOTREF(__pyx_t_6);
+        if (likely(PyList_CheckExact(__pyx_t_6)) || PyTuple_CheckExact(__pyx_t_6)) {
+          __pyx_t_3 = __pyx_t_6; __Pyx_INCREF(__pyx_t_3); __pyx_t_10 = 0;
+          __pyx_t_11 = NULL;
         } else {
-          __pyx_t_4 = __pyx_t_11(__pyx_t_1);
-          if (unlikely(!__pyx_t_4)) {
-            PyObject* exc_type = PyErr_Occurred();
-            if (exc_type) {
-              if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-              else __PYX_ERR(0, 171, __pyx_L9_error)
+          __pyx_t_10 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 171, __pyx_L9_error)
+          __Pyx_GOTREF(__pyx_t_3);
+          __pyx_t_11 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 171, __pyx_L9_error)
+        }
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        for (;;) {
+          if (likely(!__pyx_t_11)) {
+            if (likely(PyList_CheckExact(__pyx_t_3))) {
+              if (__pyx_t_10 >= PyList_GET_SIZE(__pyx_t_3)) break;
+              #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+              __pyx_t_6 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_10); __Pyx_INCREF(__pyx_t_6); __pyx_t_10++; if (unlikely(0 < 0)) __PYX_ERR(0, 171, __pyx_L9_error)
+              #else
+              __pyx_t_6 = PySequence_ITEM(__pyx_t_3, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 171, __pyx_L9_error)
+              __Pyx_GOTREF(__pyx_t_6);
+              #endif
+            } else {
+              if (__pyx_t_10 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
+              #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+              __pyx_t_6 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_10); __Pyx_INCREF(__pyx_t_6); __pyx_t_10++; if (unlikely(0 < 0)) __PYX_ERR(0, 171, __pyx_L9_error)
+              #else
+              __pyx_t_6 = PySequence_ITEM(__pyx_t_3, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 171, __pyx_L9_error)
+              __Pyx_GOTREF(__pyx_t_6);
+              #endif
             }
-            break;
+          } else {
+            __pyx_t_6 = __pyx_t_11(__pyx_t_3);
+            if (unlikely(!__pyx_t_6)) {
+              PyObject* exc_type = PyErr_Occurred();
+              if (exc_type) {
+                if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+                else __PYX_ERR(0, 171, __pyx_L9_error)
+              }
+              break;
+            }
+            __Pyx_GOTREF(__pyx_t_6);
           }
+          __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_qb, __pyx_t_6);
+          __pyx_t_6 = 0;
+          __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_circuit, __pyx_n_s_qubits); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 171, __pyx_L9_error)
           __Pyx_GOTREF(__pyx_t_4);
-        }
-        __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_qb, __pyx_t_4);
-        __pyx_t_4 = 0;
-        __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_circuit, __pyx_n_s_qubits); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 171, __pyx_L9_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_index); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 171, __pyx_L9_error)
-        __Pyx_GOTREF(__pyx_t_12);
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __pyx_t_3 = NULL;
-        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_12))) {
-          __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_12);
-          if (likely(__pyx_t_3)) {
-            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
-            __Pyx_INCREF(__pyx_t_3);
-            __Pyx_INCREF(function);
-            __Pyx_DECREF_SET(__pyx_t_12, function);
+          __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_index); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 171, __pyx_L9_error)
+          __Pyx_GOTREF(__pyx_t_12);
+          __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+          __pyx_t_4 = NULL;
+          if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_12))) {
+            __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_12);
+            if (likely(__pyx_t_4)) {
+              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
+              __Pyx_INCREF(__pyx_t_4);
+              __Pyx_INCREF(function);
+              __Pyx_DECREF_SET(__pyx_t_12, function);
+            }
           }
+          __pyx_t_6 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_12, __pyx_t_4, __pyx_7genexpr__pyx_v_qb) : __Pyx_PyObject_CallOneArg(__pyx_t_12, __pyx_7genexpr__pyx_v_qb);
+          __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+          if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 171, __pyx_L9_error)
+          __Pyx_GOTREF(__pyx_t_6);
+          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+          if (unlikely(__Pyx_ListComp_Append(__pyx_t_7, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 171, __pyx_L9_error)
+          __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         }
-        __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_12, __pyx_t_3, __pyx_7genexpr__pyx_v_qb) : __Pyx_PyObject_CallOneArg(__pyx_t_12, __pyx_7genexpr__pyx_v_qb);
-        __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 171, __pyx_L9_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-        if (unlikely(__Pyx_ListComp_Append(__pyx_t_7, (PyObject*)__pyx_t_4))) __PYX_ERR(0, 171, __pyx_L9_error)
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      }
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __Pyx_XDECREF(__pyx_7genexpr__pyx_v_qb); __pyx_7genexpr__pyx_v_qb = 0;
-      goto __pyx_L12_exit_scope;
-      __pyx_L9_error:;
-      __Pyx_XDECREF(__pyx_7genexpr__pyx_v_qb); __pyx_7genexpr__pyx_v_qb = 0;
-      goto __pyx_L1_error;
-      __pyx_L12_exit_scope:;
-    } /* exit inner scope */
-    __Pyx_XDECREF_SET(__pyx_v_targets, ((PyObject*)__pyx_t_7));
-    __pyx_t_7 = 0;
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __Pyx_XDECREF(__pyx_7genexpr__pyx_v_qb); __pyx_7genexpr__pyx_v_qb = 0;
+        goto __pyx_L12_exit_scope;
+        __pyx_L9_error:;
+        __Pyx_XDECREF(__pyx_7genexpr__pyx_v_qb); __pyx_7genexpr__pyx_v_qb = 0;
+        goto __pyx_L1_error;
+        __pyx_L12_exit_scope:;
+      } /* exit inner scope */
+      __Pyx_XDECREF_SET(__pyx_v_targets, ((PyObject*)__pyx_t_7));
+      __pyx_t_7 = 0;
 
-    /* "dwave/gate/simulator/simulator.pyx":172
- *     for op in circuit.circuit:
- *         targets = [circuit.qubits.index(qb) for qb in op.qubits]
- *         apply_instruction(num_qubits, state, op, targets, little_endian, rng)             # <<<<<<<<<<<<<<
+      /* "dwave/gate/simulator/simulator.pyx":172
+ *         for op in circuit.circuit:
+ *             targets = [circuit.qubits.index(qb) for qb in op.qubits]
+ *             apply_instruction(num_qubits, state, op, targets, little_endian, rng)             # <<<<<<<<<<<<<<
  * 
- *     return state
+ *     circuit.set_state(state, force=True)
  */
-    __Pyx_TraceLine(172,0,__PYX_ERR(0, 172, __pyx_L1_error))
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_apply_instruction); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = NULL;
-    __pyx_t_6 = 0;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
-      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
-      if (likely(__pyx_t_4)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-        __Pyx_INCREF(__pyx_t_4);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_1, function);
-        __pyx_t_6 = 1;
+      __Pyx_TraceLine(172,0,__PYX_ERR(0, 172, __pyx_L1_error))
+      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_apply_instruction); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 172, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_6 = NULL;
+      __pyx_t_5 = 0;
+      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+        __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
+        if (likely(__pyx_t_6)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+          __Pyx_INCREF(__pyx_t_6);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_3, function);
+          __pyx_t_5 = 1;
+        }
       }
-    }
-    #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(__pyx_t_1)) {
-      PyObject *__pyx_temp[7] = {__pyx_t_4, __pyx_v_num_qubits, __pyx_v_state, __pyx_v_op, __pyx_v_targets, __pyx_v_little_endian, __pyx_v_rng};
-      __pyx_t_7 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_6, 6+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 172, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_GOTREF(__pyx_t_7);
-    } else
-    #endif
-    #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
-      PyObject *__pyx_temp[7] = {__pyx_t_4, __pyx_v_num_qubits, __pyx_v_state, __pyx_v_op, __pyx_v_targets, __pyx_v_little_endian, __pyx_v_rng};
-      __pyx_t_7 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_6, 6+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 172, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_GOTREF(__pyx_t_7);
-    } else
-    #endif
-    {
-      __pyx_t_12 = PyTuple_New(6+__pyx_t_6); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 172, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_12);
-      if (__pyx_t_4) {
-        __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_4); __pyx_t_4 = NULL;
+      #if CYTHON_FAST_PYCALL
+      if (PyFunction_Check(__pyx_t_3)) {
+        PyObject *__pyx_temp[7] = {__pyx_t_6, __pyx_v_num_qubits, __pyx_v_state, __pyx_v_op, __pyx_v_targets, __pyx_v_little_endian, __pyx_v_rng};
+        __pyx_t_7 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 6+__pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 172, __pyx_L1_error)
+        __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+        __Pyx_GOTREF(__pyx_t_7);
+      } else
+      #endif
+      #if CYTHON_FAST_PYCCALL
+      if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
+        PyObject *__pyx_temp[7] = {__pyx_t_6, __pyx_v_num_qubits, __pyx_v_state, __pyx_v_op, __pyx_v_targets, __pyx_v_little_endian, __pyx_v_rng};
+        __pyx_t_7 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 6+__pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 172, __pyx_L1_error)
+        __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+        __Pyx_GOTREF(__pyx_t_7);
+      } else
+      #endif
+      {
+        __pyx_t_12 = PyTuple_New(6+__pyx_t_5); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 172, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_12);
+        if (__pyx_t_6) {
+          __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_6); __pyx_t_6 = NULL;
+        }
+        __Pyx_INCREF(__pyx_v_num_qubits);
+        __Pyx_GIVEREF(__pyx_v_num_qubits);
+        PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_5, __pyx_v_num_qubits);
+        __Pyx_INCREF(__pyx_v_state);
+        __Pyx_GIVEREF(__pyx_v_state);
+        PyTuple_SET_ITEM(__pyx_t_12, 1+__pyx_t_5, __pyx_v_state);
+        __Pyx_INCREF(__pyx_v_op);
+        __Pyx_GIVEREF(__pyx_v_op);
+        PyTuple_SET_ITEM(__pyx_t_12, 2+__pyx_t_5, __pyx_v_op);
+        __Pyx_INCREF(__pyx_v_targets);
+        __Pyx_GIVEREF(__pyx_v_targets);
+        PyTuple_SET_ITEM(__pyx_t_12, 3+__pyx_t_5, __pyx_v_targets);
+        __Pyx_INCREF(__pyx_v_little_endian);
+        __Pyx_GIVEREF(__pyx_v_little_endian);
+        PyTuple_SET_ITEM(__pyx_t_12, 4+__pyx_t_5, __pyx_v_little_endian);
+        __Pyx_INCREF(__pyx_v_rng);
+        __Pyx_GIVEREF(__pyx_v_rng);
+        PyTuple_SET_ITEM(__pyx_t_12, 5+__pyx_t_5, __pyx_v_rng);
+        __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_12, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 172, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_7);
+        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       }
-      __Pyx_INCREF(__pyx_v_num_qubits);
-      __Pyx_GIVEREF(__pyx_v_num_qubits);
-      PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_6, __pyx_v_num_qubits);
-      __Pyx_INCREF(__pyx_v_state);
-      __Pyx_GIVEREF(__pyx_v_state);
-      PyTuple_SET_ITEM(__pyx_t_12, 1+__pyx_t_6, __pyx_v_state);
-      __Pyx_INCREF(__pyx_v_op);
-      __Pyx_GIVEREF(__pyx_v_op);
-      PyTuple_SET_ITEM(__pyx_t_12, 2+__pyx_t_6, __pyx_v_op);
-      __Pyx_INCREF(__pyx_v_targets);
-      __Pyx_GIVEREF(__pyx_v_targets);
-      PyTuple_SET_ITEM(__pyx_t_12, 3+__pyx_t_6, __pyx_v_targets);
-      __Pyx_INCREF(__pyx_v_little_endian);
-      __Pyx_GIVEREF(__pyx_v_little_endian);
-      PyTuple_SET_ITEM(__pyx_t_12, 4+__pyx_t_6, __pyx_v_little_endian);
-      __Pyx_INCREF(__pyx_v_rng);
-      __Pyx_GIVEREF(__pyx_v_rng);
-      PyTuple_SET_ITEM(__pyx_t_12, 5+__pyx_t_6, __pyx_v_rng);
-      __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_12, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 172, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-    }
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "dwave/gate/simulator/simulator.pyx":170
- *     state[0] = 1
+      /* "dwave/gate/simulator/simulator.pyx":170
+ *         state[0] = 1
  * 
- *     for op in circuit.circuit:             # <<<<<<<<<<<<<<
- *         targets = [circuit.qubits.index(qb) for qb in op.qubits]
- *         apply_instruction(num_qubits, state, op, targets, little_endian, rng)
+ *         for op in circuit.circuit:             # <<<<<<<<<<<<<<
+ *             targets = [circuit.qubits.index(qb) for qb in op.qubits]
+ *             apply_instruction(num_qubits, state, op, targets, little_endian, rng)
  */
-    __Pyx_TraceLine(170,0,__PYX_ERR(0, 170, __pyx_L1_error))
+      __Pyx_TraceLine(170,0,__PYX_ERR(0, 170, __pyx_L1_error))
+    }
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_L4:;
 
   /* "dwave/gate/simulator/simulator.pyx":174
- *         apply_instruction(num_qubits, state, op, targets, little_endian, rng)
+ *             apply_instruction(num_qubits, state, op, targets, little_endian, rng)
  * 
- *     return state             # <<<<<<<<<<<<<<
+ *     circuit.set_state(state, force=True)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_TraceLine(174,0,__PYX_ERR(0, 174, __pyx_L1_error))
-  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_circuit, __pyx_n_s_set_state); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 174, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 174, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
   __Pyx_INCREF(__pyx_v_state);
-  __pyx_r = __pyx_v_state;
-  goto __pyx_L0;
+  __Pyx_GIVEREF(__pyx_v_state);
+  PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_v_state);
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 174, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_force, Py_True) < 0) __PYX_ERR(0, 174, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_7, __pyx_t_3); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 174, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_12);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
 
-  /* "dwave/gate/simulator/simulator.pyx":133
+  /* "dwave/gate/simulator/simulator.pyx":134
  * 
  * 
  * def simulate(             # <<<<<<<<<<<<<<
  *     circuit: Circuit,
  *     mixed_state: bool = False,
  */
 
   /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_12);
   __Pyx_AddTraceback("dwave.gate.simulator.simulator.simulate", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_num_qubits);
   __Pyx_XDECREF(__pyx_v_rng);
@@ -5264,23 +5263,295 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "dwave/gate/simulator/simulator.pyx":177
  * 
  * 
+ * def sample_qubit(             # <<<<<<<<<<<<<<
+ *     qubit: int,
+ *     state: np.typing.NDArray,
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_5dwave_4gate_9simulator_9simulator_5sample_qubit(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_5dwave_4gate_9simulator_9simulator_4sample_qubit[] = "Sample a single qubit.\n\n    Args:\n        qubit: The qubit index that is measured.\n        state: The state to sample from.\n        rng: Random number generator to use for measuring in the computational basis.\n        collapse_state: Whether to collapse the state after measuring.\n        little_endian: If true, return the state vector using little-endian indexing for\n            the qubits. Otherwise use big-endian.\n\n    Returns:\n        int: The measurement sample (0 or 1).\n    ";
+static PyMethodDef __pyx_mdef_5dwave_4gate_9simulator_9simulator_5sample_qubit = {"sample_qubit", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5dwave_4gate_9simulator_9simulator_5sample_qubit, METH_VARARGS|METH_KEYWORDS, __pyx_doc_5dwave_4gate_9simulator_9simulator_4sample_qubit};
+static PyObject *__pyx_pw_5dwave_4gate_9simulator_9simulator_5sample_qubit(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_qubit = 0;
+  PyObject *__pyx_v_state = 0;
+  PyObject *__pyx_v_rng = 0;
+  PyObject *__pyx_v_collapse_state = 0;
+  PyObject *__pyx_v_little_endian = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("sample_qubit (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_qubit,&__pyx_n_s_state,&__pyx_n_s_rng,&__pyx_n_s_collapse_state,&__pyx_n_s_little_endian,0};
+    PyObject* values[5] = {0,0,0,0,0};
+
+    /* "dwave/gate/simulator/simulator.pyx":181
+ *     state: np.typing.NDArray,
+ *     rng: np.random.Generator,
+ *     collapse_state: bool = True,             # <<<<<<<<<<<<<<
+ *     little_endian: bool = False,
+ * ) -> int:
+ */
+    values[3] = ((PyObject *)Py_True);
+
+    /* "dwave/gate/simulator/simulator.pyx":182
+ *     rng: np.random.Generator,
+ *     collapse_state: bool = True,
+ *     little_endian: bool = False,             # <<<<<<<<<<<<<<
+ * ) -> int:
+ *     """Sample a single qubit.
+ */
+    values[4] = ((PyObject *)Py_False);
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+        CYTHON_FALLTHROUGH;
+        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_qubit)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_state)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("sample_qubit", 0, 3, 5, 1); __PYX_ERR(0, 177, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_rng)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("sample_qubit", 0, 3, 5, 2); __PYX_ERR(0, 177, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  3:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_collapse_state);
+          if (value) { values[3] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case  4:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_little_endian);
+          if (value) { values[4] = value; kw_args--; }
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "sample_qubit") < 0)) __PYX_ERR(0, 177, __pyx_L3_error)
+      }
+    } else {
+      switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+        CYTHON_FALLTHROUGH;
+        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+    }
+    __pyx_v_qubit = values[0];
+    __pyx_v_state = values[1];
+    __pyx_v_rng = values[2];
+    __pyx_v_collapse_state = values[3];
+    __pyx_v_little_endian = values[4];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("sample_qubit", 0, 3, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 177, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("dwave.gate.simulator.simulator.sample_qubit", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_5dwave_4gate_9simulator_9simulator_4sample_qubit(__pyx_self, __pyx_v_qubit, __pyx_v_state, __pyx_v_rng, __pyx_v_collapse_state, __pyx_v_little_endian);
+
+  /* "dwave/gate/simulator/simulator.pyx":177
+ * 
+ * 
+ * def sample_qubit(             # <<<<<<<<<<<<<<
+ *     qubit: int,
+ *     state: np.typing.NDArray,
+ */
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_5dwave_4gate_9simulator_9simulator_4sample_qubit(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_qubit, PyObject *__pyx_v_state, PyObject *__pyx_v_rng, PyObject *__pyx_v_collapse_state, PyObject *__pyx_v_little_endian) {
+  int __pyx_v_num_qubits;
+  PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  int __pyx_t_5;
+  __Pyx_memviewslice __pyx_t_6 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  uint64_t __pyx_t_7;
+  struct __pyx_opt_args_5dwave_4gate_9simulator_3ops_measurement_computational_basis __pyx_t_8;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_TraceFrameInit(__pyx_codeobj__4)
+  __Pyx_RefNannySetupContext("sample_qubit", 0);
+  __Pyx_TraceCall("sample_qubit", __pyx_f[0], 177, 0, __PYX_ERR(0, 177, __pyx_L1_error));
+
+  /* "dwave/gate/simulator/simulator.pyx":197
+ *         int: The measurement sample (0 or 1).
+ *     """
+ *     cdef int num_qubits = round(np.log2(state.shape[0]))             # <<<<<<<<<<<<<<
+ * 
+ *     return measurement_computational_basis(
+ */
+  __Pyx_TraceLine(197,0,__PYX_ERR(0, 197, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_log2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_shape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_2, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_2)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_2);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
+    }
+  }
+  __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_round, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_v_num_qubits = __pyx_t_5;
+
+  /* "dwave/gate/simulator/simulator.pyx":199
+ *     cdef int num_qubits = round(np.log2(state.shape[0]))
+ * 
+ *     return measurement_computational_basis(             # <<<<<<<<<<<<<<
+ *         num_qubits,
+ *         state,
+ */
+  __Pyx_TraceLine(199,0,__PYX_ERR(0, 199, __pyx_L1_error))
+  __Pyx_XDECREF(__pyx_r);
+
+  /* "dwave/gate/simulator/simulator.pyx":201
+ *     return measurement_computational_basis(
+ *         num_qubits,
+ *         state,             # <<<<<<<<<<<<<<
+ *         qubit,
+ *         rng,
+ */
+  __Pyx_TraceLine(201,0,__PYX_ERR(0, 201, __pyx_L1_error))
+  __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_dc___pyx_t_double_complex(__pyx_v_state, PyBUF_WRITABLE); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 201, __pyx_L1_error)
+
+  /* "dwave/gate/simulator/simulator.pyx":202
+ *         num_qubits,
+ *         state,
+ *         qubit,             # <<<<<<<<<<<<<<
+ *         rng,
+ *         little_endian=little_endian,
+ */
+  __Pyx_TraceLine(202,0,__PYX_ERR(0, 202, __pyx_L1_error))
+  __pyx_t_7 = __Pyx_PyInt_As_uint64_t(__pyx_v_qubit); if (unlikely((__pyx_t_7 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 202, __pyx_L1_error)
+
+  /* "dwave/gate/simulator/simulator.pyx":199
+ *     cdef int num_qubits = round(np.log2(state.shape[0]))
+ * 
+ *     return measurement_computational_basis(             # <<<<<<<<<<<<<<
+ *         num_qubits,
+ *         state,
+ */
+  __Pyx_TraceLine(199,0,__PYX_ERR(0, 199, __pyx_L1_error))
+  __pyx_t_8.__pyx_n = 2;
+  __pyx_t_8.little_endian = __pyx_v_little_endian;
+  __pyx_t_8.apply_operator = __pyx_v_collapse_state;
+  __pyx_t_3 = __pyx_f_5dwave_4gate_9simulator_3ops_measurement_computational_basis(__pyx_v_num_qubits, __pyx_t_6, __pyx_t_7, __pyx_v_rng, &__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __PYX_XDEC_MEMVIEW(&__pyx_t_6, 1);
+  __pyx_t_6.memview = NULL;
+  __pyx_t_6.data = NULL;
+  __pyx_r = __pyx_t_3;
+  __pyx_t_3 = 0;
+  goto __pyx_L0;
+
+  /* "dwave/gate/simulator/simulator.pyx":177
+ * 
+ * 
+ * def sample_qubit(             # <<<<<<<<<<<<<<
+ *     qubit: int,
+ *     state: np.typing.NDArray,
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __PYX_XDEC_MEMVIEW(&__pyx_t_6, 1);
+  __Pyx_AddTraceback("dwave.gate.simulator.simulator.sample_qubit", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "dwave/gate/simulator/simulator.pyx":209
+ * 
+ * 
  * def _measure(op, state, targets, rng):             # <<<<<<<<<<<<<<
  *     op._measured_state = state.copy()
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_5dwave_4gate_9simulator_9simulator_5_measure(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_5dwave_4gate_9simulator_9simulator_5_measure = {"_measure", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5dwave_4gate_9simulator_9simulator_5_measure, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_5dwave_4gate_9simulator_9simulator_5_measure(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_5dwave_4gate_9simulator_9simulator_7_measure(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_5dwave_4gate_9simulator_9simulator_7_measure = {"_measure", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5dwave_4gate_9simulator_9simulator_7_measure, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_5dwave_4gate_9simulator_9simulator_7_measure(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_op = 0;
   PyObject *__pyx_v_state = 0;
   PyObject *__pyx_v_targets = 0;
   PyObject *__pyx_v_rng = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -5310,31 +5581,31 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_op)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_state)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_measure", 1, 4, 4, 1); __PYX_ERR(0, 177, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_measure", 1, 4, 4, 1); __PYX_ERR(0, 209, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_targets)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_measure", 1, 4, 4, 2); __PYX_ERR(0, 177, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_measure", 1, 4, 4, 2); __PYX_ERR(0, 209, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_rng)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_measure", 1, 4, 4, 3); __PYX_ERR(0, 177, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_measure", 1, 4, 4, 3); __PYX_ERR(0, 209, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_measure") < 0)) __PYX_ERR(0, 177, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_measure") < 0)) __PYX_ERR(0, 209, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -5343,28 +5614,28 @@
     __pyx_v_op = values[0];
     __pyx_v_state = values[1];
     __pyx_v_targets = values[2];
     __pyx_v_rng = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_measure", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 177, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_measure", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 209, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("dwave.gate.simulator.simulator._measure", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_5dwave_4gate_9simulator_9simulator_4_measure(__pyx_self, __pyx_v_op, __pyx_v_state, __pyx_v_targets, __pyx_v_rng);
+  __pyx_r = __pyx_pf_5dwave_4gate_9simulator_9simulator_6_measure(__pyx_self, __pyx_v_op, __pyx_v_state, __pyx_v_targets, __pyx_v_rng);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_5dwave_4gate_9simulator_9simulator_4_measure(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_op, PyObject *__pyx_v_state, PyObject *__pyx_v_targets, PyObject *__pyx_v_rng) {
+static PyObject *__pyx_pf_5dwave_4gate_9simulator_9simulator_6_measure(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_op, PyObject *__pyx_v_state, PyObject *__pyx_v_targets, PyObject *__pyx_v_rng) {
   PyObject *__pyx_v_idx = NULL;
   PyObject *__pyx_v_t = NULL;
   PyObject *__pyx_v_m = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
@@ -5383,112 +5654,112 @@
   PyObject *__pyx_t_14 = NULL;
   int __pyx_t_15;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceFrameInit(__pyx_codeobj__5)
   __Pyx_RefNannySetupContext("_measure", 0);
-  __Pyx_TraceCall("_measure", __pyx_f[0], 177, 0, __PYX_ERR(0, 177, __pyx_L1_error));
+  __Pyx_TraceCall("_measure", __pyx_f[0], 209, 0, __PYX_ERR(0, 209, __pyx_L1_error));
 
-  /* "dwave/gate/simulator/simulator.pyx":178
+  /* "dwave/gate/simulator/simulator.pyx":210
  * 
  * def _measure(op, state, targets, rng):
  *     op._measured_state = state.copy()             # <<<<<<<<<<<<<<
  * 
  *     for idx, t in enumerate(targets):
  */
-  __Pyx_TraceLine(178,0,__PYX_ERR(0, 178, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_copy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 178, __pyx_L1_error)
+  __Pyx_TraceLine(210,0,__PYX_ERR(0, 210, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_copy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 178, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_op, __pyx_n_s_measured_state, __pyx_t_1) < 0) __PYX_ERR(0, 178, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_op, __pyx_n_s_measured_state, __pyx_t_1) < 0) __PYX_ERR(0, 210, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "dwave/gate/simulator/simulator.pyx":180
+  /* "dwave/gate/simulator/simulator.pyx":212
  *     op._measured_state = state.copy()
  * 
  *     for idx, t in enumerate(targets):             # <<<<<<<<<<<<<<
- *         m = _sample(t, state, rng)
+ *         m = sample_qubit(t, state, rng)
  * 
  */
-  __Pyx_TraceLine(180,0,__PYX_ERR(0, 180, __pyx_L1_error))
+  __Pyx_TraceLine(212,0,__PYX_ERR(0, 212, __pyx_L1_error))
   __Pyx_INCREF(__pyx_int_0);
   __pyx_t_1 = __pyx_int_0;
   if (likely(PyList_CheckExact(__pyx_v_targets)) || PyTuple_CheckExact(__pyx_v_targets)) {
     __pyx_t_2 = __pyx_v_targets; __Pyx_INCREF(__pyx_t_2); __pyx_t_4 = 0;
     __pyx_t_5 = NULL;
   } else {
-    __pyx_t_4 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_targets); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 180, __pyx_L1_error)
+    __pyx_t_4 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_targets); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 212, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_5 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 180, __pyx_L1_error)
+    __pyx_t_5 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 212, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_5)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 180, __pyx_L1_error)
+        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 212, __pyx_L1_error)
         #else
-        __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 180, __pyx_L1_error)
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 212, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         #endif
       } else {
         if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 180, __pyx_L1_error)
+        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 212, __pyx_L1_error)
         #else
-        __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 180, __pyx_L1_error)
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 212, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         #endif
       }
     } else {
       __pyx_t_3 = __pyx_t_5(__pyx_t_2);
       if (unlikely(!__pyx_t_3)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 180, __pyx_L1_error)
+          else __PYX_ERR(0, 212, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_3);
     }
     __Pyx_XDECREF_SET(__pyx_v_t, __pyx_t_3);
     __pyx_t_3 = 0;
     __Pyx_INCREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_idx, __pyx_t_1);
-    __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_t_1, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 180, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_t_1, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 212, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1);
     __pyx_t_1 = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "dwave/gate/simulator/simulator.pyx":181
+    /* "dwave/gate/simulator/simulator.pyx":213
  * 
  *     for idx, t in enumerate(targets):
- *         m = _sample(t, state, rng)             # <<<<<<<<<<<<<<
+ *         m = sample_qubit(t, state, rng)             # <<<<<<<<<<<<<<
  * 
  *         try:
  */
-    __Pyx_TraceLine(181,0,__PYX_ERR(0, 181, __pyx_L1_error))
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_sample); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 181, __pyx_L1_error)
+    __Pyx_TraceLine(213,0,__PYX_ERR(0, 213, __pyx_L1_error))
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_sample_qubit); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 213, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_7 = NULL;
     __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -5497,100 +5768,100 @@
         __Pyx_DECREF_SET(__pyx_t_6, function);
         __pyx_t_8 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_6)) {
       PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_v_t, __pyx_v_state, __pyx_v_rng};
-      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 181, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 213, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_GOTREF(__pyx_t_3);
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
       PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_v_t, __pyx_v_state, __pyx_v_rng};
-      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 181, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 213, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_GOTREF(__pyx_t_3);
     } else
     #endif
     {
-      __pyx_t_9 = PyTuple_New(3+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 181, __pyx_L1_error)
+      __pyx_t_9 = PyTuple_New(3+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 213, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       if (__pyx_t_7) {
         __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_7); __pyx_t_7 = NULL;
       }
       __Pyx_INCREF(__pyx_v_t);
       __Pyx_GIVEREF(__pyx_v_t);
       PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_v_t);
       __Pyx_INCREF(__pyx_v_state);
       __Pyx_GIVEREF(__pyx_v_state);
       PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_8, __pyx_v_state);
       __Pyx_INCREF(__pyx_v_rng);
       __Pyx_GIVEREF(__pyx_v_rng);
       PyTuple_SET_ITEM(__pyx_t_9, 2+__pyx_t_8, __pyx_v_rng);
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 181, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 213, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF_SET(__pyx_v_m, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "dwave/gate/simulator/simulator.pyx":183
- *         m = _sample(t, state, rng)
+    /* "dwave/gate/simulator/simulator.pyx":215
+ *         m = sample_qubit(t, state, rng)
  * 
  *         try:             # <<<<<<<<<<<<<<
  *             op.bits[idx].set(m, force=True)
  *         except (IndexError, TypeError):
  */
-    __Pyx_TraceLine(183,0,__PYX_ERR(0, 183, __pyx_L1_error))
+    __Pyx_TraceLine(215,0,__PYX_ERR(0, 215, __pyx_L1_error))
     {
       __Pyx_PyThreadState_declare
       __Pyx_PyThreadState_assign
       __Pyx_ExceptionSave(&__pyx_t_10, &__pyx_t_11, &__pyx_t_12);
       __Pyx_XGOTREF(__pyx_t_10);
       __Pyx_XGOTREF(__pyx_t_11);
       __Pyx_XGOTREF(__pyx_t_12);
       /*try:*/ {
 
-        /* "dwave/gate/simulator/simulator.pyx":184
+        /* "dwave/gate/simulator/simulator.pyx":216
  * 
  *         try:
  *             op.bits[idx].set(m, force=True)             # <<<<<<<<<<<<<<
  *         except (IndexError, TypeError):
  *             warnings.warn("Measurements not stored in the classical register.")
  */
-        __Pyx_TraceLine(184,0,__PYX_ERR(0, 184, __pyx_L5_error))
-        __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_op, __pyx_n_s_bits); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 184, __pyx_L5_error)
+        __Pyx_TraceLine(216,0,__PYX_ERR(0, 216, __pyx_L5_error))
+        __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_op, __pyx_n_s_bits); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 216, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_t_3, __pyx_v_idx); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 184, __pyx_L5_error)
+        __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_t_3, __pyx_v_idx); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 216, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_set); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 184, __pyx_L5_error)
+        __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_set); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 216, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-        __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 184, __pyx_L5_error)
+        __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 216, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_INCREF(__pyx_v_m);
         __Pyx_GIVEREF(__pyx_v_m);
         PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_v_m);
-        __pyx_t_9 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 184, __pyx_L5_error)
+        __pyx_t_9 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 216, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_9);
-        if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_force, Py_True) < 0) __PYX_ERR(0, 184, __pyx_L5_error)
-        __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, __pyx_t_9); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 184, __pyx_L5_error)
+        if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_force, Py_True) < 0) __PYX_ERR(0, 216, __pyx_L5_error)
+        __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, __pyx_t_9); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 216, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-        /* "dwave/gate/simulator/simulator.pyx":183
- *         m = _sample(t, state, rng)
+        /* "dwave/gate/simulator/simulator.pyx":215
+ *         m = sample_qubit(t, state, rng)
  * 
  *         try:             # <<<<<<<<<<<<<<
  *             op.bits[idx].set(m, force=True)
  *         except (IndexError, TypeError):
  */
       }
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
@@ -5599,69 +5870,69 @@
       goto __pyx_L12_try_end;
       __pyx_L5_error:;
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-      /* "dwave/gate/simulator/simulator.pyx":185
+      /* "dwave/gate/simulator/simulator.pyx":217
  *         try:
  *             op.bits[idx].set(m, force=True)
  *         except (IndexError, TypeError):             # <<<<<<<<<<<<<<
  *             warnings.warn("Measurements not stored in the classical register.")
  * 
  */
-      __Pyx_TraceLine(185,0,__PYX_ERR(0, 185, __pyx_L7_except_error))
+      __Pyx_TraceLine(217,0,__PYX_ERR(0, 217, __pyx_L7_except_error))
       __pyx_t_8 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_IndexError) || __Pyx_PyErr_ExceptionMatches(__pyx_builtin_TypeError);
       if (__pyx_t_8) {
         __Pyx_AddTraceback("dwave.gate.simulator.simulator._measure", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_9, &__pyx_t_6) < 0) __PYX_ERR(0, 185, __pyx_L7_except_error)
+        if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_9, &__pyx_t_6) < 0) __PYX_ERR(0, 217, __pyx_L7_except_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_GOTREF(__pyx_t_9);
         __Pyx_GOTREF(__pyx_t_6);
 
-        /* "dwave/gate/simulator/simulator.pyx":186
+        /* "dwave/gate/simulator/simulator.pyx":218
  *             op.bits[idx].set(m, force=True)
  *         except (IndexError, TypeError):
  *             warnings.warn("Measurements not stored in the classical register.")             # <<<<<<<<<<<<<<
  * 
  *         op._measured_qubit_indices.append(t)
  */
-        __Pyx_TraceLine(186,0,__PYX_ERR(0, 186, __pyx_L7_except_error))
-        __Pyx_GetModuleGlobalName(__pyx_t_13, __pyx_n_s_warnings); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 186, __pyx_L7_except_error)
+        __Pyx_TraceLine(218,0,__PYX_ERR(0, 218, __pyx_L7_except_error))
+        __Pyx_GetModuleGlobalName(__pyx_t_13, __pyx_n_s_warnings); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 218, __pyx_L7_except_error)
         __Pyx_GOTREF(__pyx_t_13);
-        __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_13, __pyx_n_s_warn); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 186, __pyx_L7_except_error)
+        __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_13, __pyx_n_s_warn); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 218, __pyx_L7_except_error)
         __Pyx_GOTREF(__pyx_t_14);
         __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
         __pyx_t_13 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_14))) {
           __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_14);
           if (likely(__pyx_t_13)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_14);
             __Pyx_INCREF(__pyx_t_13);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_14, function);
           }
         }
         __pyx_t_3 = (__pyx_t_13) ? __Pyx_PyObject_Call2Args(__pyx_t_14, __pyx_t_13, __pyx_kp_u_Measurements_not_stored_in_the_c) : __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_kp_u_Measurements_not_stored_in_the_c);
         __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 186, __pyx_L7_except_error)
+        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 218, __pyx_L7_except_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
         __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
         goto __pyx_L6_exception_handled;
       }
       goto __pyx_L7_except_error;
       __pyx_L7_except_error:;
 
-      /* "dwave/gate/simulator/simulator.pyx":183
- *         m = _sample(t, state, rng)
+      /* "dwave/gate/simulator/simulator.pyx":215
+ *         m = sample_qubit(t, state, rng)
  * 
  *         try:             # <<<<<<<<<<<<<<
  *             op.bits[idx].set(m, force=True)
  *         except (IndexError, TypeError):
  */
       __Pyx_XGIVEREF(__pyx_t_10);
       __Pyx_XGIVEREF(__pyx_t_11);
@@ -5672,40 +5943,40 @@
       __Pyx_XGIVEREF(__pyx_t_10);
       __Pyx_XGIVEREF(__pyx_t_11);
       __Pyx_XGIVEREF(__pyx_t_12);
       __Pyx_ExceptionReset(__pyx_t_10, __pyx_t_11, __pyx_t_12);
       __pyx_L12_try_end:;
     }
 
-    /* "dwave/gate/simulator/simulator.pyx":188
+    /* "dwave/gate/simulator/simulator.pyx":220
  *             warnings.warn("Measurements not stored in the classical register.")
  * 
  *         op._measured_qubit_indices.append(t)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __Pyx_TraceLine(188,0,__PYX_ERR(0, 188, __pyx_L1_error))
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_op, __pyx_n_s_measured_qubit_indices); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 188, __pyx_L1_error)
+    __Pyx_TraceLine(220,0,__PYX_ERR(0, 220, __pyx_L1_error))
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_op, __pyx_n_s_measured_qubit_indices); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 220, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_15 = __Pyx_PyObject_Append(__pyx_t_6, __pyx_v_t); if (unlikely(__pyx_t_15 == ((int)-1))) __PYX_ERR(0, 188, __pyx_L1_error)
+    __pyx_t_15 = __Pyx_PyObject_Append(__pyx_t_6, __pyx_v_t); if (unlikely(__pyx_t_15 == ((int)-1))) __PYX_ERR(0, 220, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "dwave/gate/simulator/simulator.pyx":180
+    /* "dwave/gate/simulator/simulator.pyx":212
  *     op._measured_state = state.copy()
  * 
  *     for idx, t in enumerate(targets):             # <<<<<<<<<<<<<<
- *         m = _sample(t, state, rng)
+ *         m = sample_qubit(t, state, rng)
  * 
  */
-    __Pyx_TraceLine(180,0,__PYX_ERR(0, 180, __pyx_L1_error))
+    __Pyx_TraceLine(212,0,__PYX_ERR(0, 212, __pyx_L1_error))
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "dwave/gate/simulator/simulator.pyx":177
+  /* "dwave/gate/simulator/simulator.pyx":209
  * 
  * 
  * def _measure(op, state, targets, rng):             # <<<<<<<<<<<<<<
  *     op._measured_state = state.copy()
  * 
  */
 
@@ -5729,286 +6000,15 @@
   __Pyx_XDECREF(__pyx_v_m);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "dwave/gate/simulator/simulator.pyx":191
- * 
- * 
- * def _sample(             # <<<<<<<<<<<<<<
- *     qubit: int,
- *     state: np.typing.NDArray,
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_5dwave_4gate_9simulator_9simulator_7_sample(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_5dwave_4gate_9simulator_9simulator_7_sample = {"_sample", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5dwave_4gate_9simulator_9simulator_7_sample, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_5dwave_4gate_9simulator_9simulator_7_sample(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  PyObject *__pyx_v_qubit = 0;
-  PyObject *__pyx_v_state = 0;
-  PyObject *__pyx_v_rng = 0;
-  PyObject *__pyx_v_collapse_state = 0;
-  PyObject *__pyx_v_little_endian = 0;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("_sample (wrapper)", 0);
-  {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_qubit,&__pyx_n_s_state,&__pyx_n_s_rng,&__pyx_n_s_collapse_state,&__pyx_n_s_little_endian,0};
-    PyObject* values[5] = {0,0,0,0,0};
-
-    /* "dwave/gate/simulator/simulator.pyx":195
- *     state: np.typing.NDArray,
- *     rng: np.random.Generator,
- *     collapse_state: bool = True,             # <<<<<<<<<<<<<<
- *     little_endian: bool = False,
- * ) -> int:
- */
-    values[3] = ((PyObject *)Py_True);
-
-    /* "dwave/gate/simulator/simulator.pyx":196
- *     rng: np.random.Generator,
- *     collapse_state: bool = True,
- *     little_endian: bool = False,             # <<<<<<<<<<<<<<
- * ) -> int:
- *     cdef int num_qubits = round(np.log2(state.shape[0]))
- */
-    values[4] = ((PyObject *)Py_False);
-    if (unlikely(__pyx_kwds)) {
-      Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
-        CYTHON_FALLTHROUGH;
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
-        CYTHON_FALLTHROUGH;
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-        CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
-        case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_qubit)) != 0)) kw_args--;
-        else goto __pyx_L5_argtuple_error;
-        CYTHON_FALLTHROUGH;
-        case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_state)) != 0)) kw_args--;
-        else {
-          __Pyx_RaiseArgtupleInvalid("_sample", 0, 3, 5, 1); __PYX_ERR(0, 191, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  2:
-        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_rng)) != 0)) kw_args--;
-        else {
-          __Pyx_RaiseArgtupleInvalid("_sample", 0, 3, 5, 2); __PYX_ERR(0, 191, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  3:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_collapse_state);
-          if (value) { values[3] = value; kw_args--; }
-        }
-        CYTHON_FALLTHROUGH;
-        case  4:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_little_endian);
-          if (value) { values[4] = value; kw_args--; }
-        }
-      }
-      if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_sample") < 0)) __PYX_ERR(0, 191, __pyx_L3_error)
-      }
-    } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
-        CYTHON_FALLTHROUGH;
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
-        CYTHON_FALLTHROUGH;
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-        values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-    }
-    __pyx_v_qubit = values[0];
-    __pyx_v_state = values[1];
-    __pyx_v_rng = values[2];
-    __pyx_v_collapse_state = values[3];
-    __pyx_v_little_endian = values[4];
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_sample", 0, 3, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 191, __pyx_L3_error)
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("dwave.gate.simulator.simulator._sample", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_5dwave_4gate_9simulator_9simulator_6_sample(__pyx_self, __pyx_v_qubit, __pyx_v_state, __pyx_v_rng, __pyx_v_collapse_state, __pyx_v_little_endian);
-
-  /* "dwave/gate/simulator/simulator.pyx":191
- * 
- * 
- * def _sample(             # <<<<<<<<<<<<<<
- *     qubit: int,
- *     state: np.typing.NDArray,
- */
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_5dwave_4gate_9simulator_9simulator_6_sample(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_qubit, PyObject *__pyx_v_state, PyObject *__pyx_v_rng, PyObject *__pyx_v_collapse_state, PyObject *__pyx_v_little_endian) {
-  int __pyx_v_num_qubits;
-  PyObject *__pyx_r = NULL;
-  __Pyx_TraceDeclarations
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
-  int __pyx_t_5;
-  __Pyx_memviewslice __pyx_t_6 = { 0, 0, { 0 }, { 0 }, { 0 } };
-  uint64_t __pyx_t_7;
-  struct __pyx_opt_args_5dwave_4gate_9simulator_3ops_measurement_computational_basis __pyx_t_8;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_TraceFrameInit(__pyx_codeobj__6)
-  __Pyx_RefNannySetupContext("_sample", 0);
-  __Pyx_TraceCall("_sample", __pyx_f[0], 191, 0, __PYX_ERR(0, 191, __pyx_L1_error));
-
-  /* "dwave/gate/simulator/simulator.pyx":198
- *     little_endian: bool = False,
- * ) -> int:
- *     cdef int num_qubits = round(np.log2(state.shape[0]))             # <<<<<<<<<<<<<<
- * 
- *     return measurement_computational_basis(
- */
-  __Pyx_TraceLine(198,0,__PYX_ERR(0, 198, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_log2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 198, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_shape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_2, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_2)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_2);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-    }
-  }
-  __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 198, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_round, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 198, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 198, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_v_num_qubits = __pyx_t_5;
-
-  /* "dwave/gate/simulator/simulator.pyx":200
- *     cdef int num_qubits = round(np.log2(state.shape[0]))
- * 
- *     return measurement_computational_basis(             # <<<<<<<<<<<<<<
- *         num_qubits,
- *         state,
- */
-  __Pyx_TraceLine(200,0,__PYX_ERR(0, 200, __pyx_L1_error))
-  __Pyx_XDECREF(__pyx_r);
-
-  /* "dwave/gate/simulator/simulator.pyx":202
- *     return measurement_computational_basis(
- *         num_qubits,
- *         state,             # <<<<<<<<<<<<<<
- *         qubit,
- *         rng,
- */
-  __Pyx_TraceLine(202,0,__PYX_ERR(0, 202, __pyx_L1_error))
-  __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_dc___pyx_t_double_complex(__pyx_v_state, PyBUF_WRITABLE); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 202, __pyx_L1_error)
-
-  /* "dwave/gate/simulator/simulator.pyx":203
- *         num_qubits,
- *         state,
- *         qubit,             # <<<<<<<<<<<<<<
- *         rng,
- *         little_endian=little_endian,
- */
-  __Pyx_TraceLine(203,0,__PYX_ERR(0, 203, __pyx_L1_error))
-  __pyx_t_7 = __Pyx_PyInt_As_uint64_t(__pyx_v_qubit); if (unlikely((__pyx_t_7 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 203, __pyx_L1_error)
-
-  /* "dwave/gate/simulator/simulator.pyx":200
- *     cdef int num_qubits = round(np.log2(state.shape[0]))
- * 
- *     return measurement_computational_basis(             # <<<<<<<<<<<<<<
- *         num_qubits,
- *         state,
- */
-  __Pyx_TraceLine(200,0,__PYX_ERR(0, 200, __pyx_L1_error))
-  __pyx_t_8.__pyx_n = 2;
-  __pyx_t_8.little_endian = __pyx_v_little_endian;
-  __pyx_t_8.apply_operator = __pyx_v_collapse_state;
-  __pyx_t_3 = __pyx_f_5dwave_4gate_9simulator_3ops_measurement_computational_basis(__pyx_v_num_qubits, __pyx_t_6, __pyx_t_7, __pyx_v_rng, &__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 200, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __PYX_XDEC_MEMVIEW(&__pyx_t_6, 1);
-  __pyx_t_6.memview = NULL;
-  __pyx_t_6.data = NULL;
-  __pyx_r = __pyx_t_3;
-  __pyx_t_3 = 0;
-  goto __pyx_L0;
-
-  /* "dwave/gate/simulator/simulator.pyx":191
- * 
- * 
- * def _sample(             # <<<<<<<<<<<<<<
- *     qubit: int,
- *     state: np.typing.NDArray,
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4);
-  __PYX_XDEC_MEMVIEW(&__pyx_t_6, 1);
-  __Pyx_AddTraceback("dwave.gate.simulator.simulator._sample", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_TraceReturn(__pyx_r, 0);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "dwave/gate/simulator/simulator.pyx":210
+/* "dwave/gate/simulator/simulator.pyx":223
  * 
  * 
  * def _simulate_circuit_density_matrix(             # <<<<<<<<<<<<<<
  *     circuit: Circuit,
  *     rng: np.random.Generator,
  */
 
@@ -6025,15 +6025,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_simulate_circuit_density_matrix (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_circuit,&__pyx_n_s_rng,&__pyx_n_s_little_endian,0};
     PyObject* values[3] = {0,0,0};
 
-    /* "dwave/gate/simulator/simulator.pyx":213
+    /* "dwave/gate/simulator/simulator.pyx":226
  *     circuit: Circuit,
  *     rng: np.random.Generator,
  *     little_endian: bool = False,             # <<<<<<<<<<<<<<
  * ) -> np.typing.NDArray:
  * 
  */
     values[2] = ((PyObject *)Py_False);
@@ -6055,25 +6055,25 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_circuit)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_rng)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_simulate_circuit_density_matrix", 0, 2, 3, 1); __PYX_ERR(0, 210, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_simulate_circuit_density_matrix", 0, 2, 3, 1); __PYX_ERR(0, 223, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_little_endian);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_simulate_circuit_density_matrix") < 0)) __PYX_ERR(0, 210, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_simulate_circuit_density_matrix") < 0)) __PYX_ERR(0, 223, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
@@ -6083,23 +6083,23 @@
     }
     __pyx_v_circuit = values[0];
     __pyx_v_rng = values[1];
     __pyx_v_little_endian = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_simulate_circuit_density_matrix", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 210, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_simulate_circuit_density_matrix", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 223, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("dwave.gate.simulator.simulator._simulate_circuit_density_matrix", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5dwave_4gate_9simulator_9simulator_8_simulate_circuit_density_matrix(__pyx_self, __pyx_v_circuit, __pyx_v_rng, __pyx_v_little_endian);
 
-  /* "dwave/gate/simulator/simulator.pyx":210
+  /* "dwave/gate/simulator/simulator.pyx":223
  * 
  * 
  * def _simulate_circuit_density_matrix(             # <<<<<<<<<<<<<<
  *     circuit: Circuit,
  *     rng: np.random.Generator,
  */
 
@@ -6133,171 +6133,171 @@
   int __pyx_t_10;
   Py_ssize_t __pyx_t_11;
   PyObject *(*__pyx_t_12)(PyObject *);
   PyObject *__pyx_t_13 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceFrameInit(__pyx_codeobj__7)
+  __Pyx_TraceFrameInit(__pyx_codeobj__6)
   __Pyx_RefNannySetupContext("_simulate_circuit_density_matrix", 0);
-  __Pyx_TraceCall("_simulate_circuit_density_matrix", __pyx_f[0], 210, 0, __PYX_ERR(0, 210, __pyx_L1_error));
+  __Pyx_TraceCall("_simulate_circuit_density_matrix", __pyx_f[0], 223, 0, __PYX_ERR(0, 223, __pyx_L1_error));
 
-  /* "dwave/gate/simulator/simulator.pyx":216
+  /* "dwave/gate/simulator/simulator.pyx":229
  * ) -> np.typing.NDArray:
  * 
  *     num_qubits = circuit.num_qubits             # <<<<<<<<<<<<<<
  *     num_virtual_qubits = 2 * num_qubits
  *     state = np.zeros(1 << num_virtual_qubits, dtype=np.complex128)
  */
-  __Pyx_TraceLine(216,0,__PYX_ERR(0, 216, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_circuit, __pyx_n_s_num_qubits); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
+  __Pyx_TraceLine(229,0,__PYX_ERR(0, 229, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_circuit, __pyx_n_s_num_qubits); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_num_qubits = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "dwave/gate/simulator/simulator.pyx":217
+  /* "dwave/gate/simulator/simulator.pyx":230
  * 
  *     num_qubits = circuit.num_qubits
  *     num_virtual_qubits = 2 * num_qubits             # <<<<<<<<<<<<<<
  *     state = np.zeros(1 << num_virtual_qubits, dtype=np.complex128)
  *     state[0] = 1
  */
-  __Pyx_TraceLine(217,0,__PYX_ERR(0, 217, __pyx_L1_error))
-  __pyx_t_1 = PyNumber_Multiply(__pyx_int_2, __pyx_v_num_qubits); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 217, __pyx_L1_error)
+  __Pyx_TraceLine(230,0,__PYX_ERR(0, 230, __pyx_L1_error))
+  __pyx_t_1 = PyNumber_Multiply(__pyx_int_2, __pyx_v_num_qubits); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 230, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_num_virtual_qubits = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "dwave/gate/simulator/simulator.pyx":218
+  /* "dwave/gate/simulator/simulator.pyx":231
  *     num_qubits = circuit.num_qubits
  *     num_virtual_qubits = 2 * num_qubits
  *     state = np.zeros(1 << num_virtual_qubits, dtype=np.complex128)             # <<<<<<<<<<<<<<
  *     state[0] = 1
  * 
  */
-  __Pyx_TraceLine(218,0,__PYX_ERR(0, 218, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 218, __pyx_L1_error)
+  __Pyx_TraceLine(231,0,__PYX_ERR(0, 231, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 231, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 218, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 231, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Lshift(__pyx_int_1, __pyx_v_num_virtual_qubits); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 218, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Lshift(__pyx_int_1, __pyx_v_num_virtual_qubits); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 231, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 218, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 231, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 218, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 231, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 218, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 231, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_complex128); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 218, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_complex128); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 231, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 218, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 231, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 218, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 231, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_state = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "dwave/gate/simulator/simulator.pyx":219
+  /* "dwave/gate/simulator/simulator.pyx":232
  *     num_virtual_qubits = 2 * num_qubits
  *     state = np.zeros(1 << num_virtual_qubits, dtype=np.complex128)
  *     state[0] = 1             # <<<<<<<<<<<<<<
  * 
  *     for op in circuit.circuit:
  */
-  __Pyx_TraceLine(219,0,__PYX_ERR(0, 219, __pyx_L1_error))
-  if (unlikely(__Pyx_SetItemInt(__pyx_v_state, 0, __pyx_int_1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1) < 0)) __PYX_ERR(0, 219, __pyx_L1_error)
+  __Pyx_TraceLine(232,0,__PYX_ERR(0, 232, __pyx_L1_error))
+  if (unlikely(__Pyx_SetItemInt(__pyx_v_state, 0, __pyx_int_1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1) < 0)) __PYX_ERR(0, 232, __pyx_L1_error)
 
-  /* "dwave/gate/simulator/simulator.pyx":221
+  /* "dwave/gate/simulator/simulator.pyx":234
  *     state[0] = 1
  * 
  *     for op in circuit.circuit:             # <<<<<<<<<<<<<<
  *         if isinstance(op, ops.Measurement):
  *             _measure(op, state, circuit, rng)
  */
-  __Pyx_TraceLine(221,0,__PYX_ERR(0, 221, __pyx_L1_error))
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_circuit, __pyx_n_s_circuit); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 221, __pyx_L1_error)
+  __Pyx_TraceLine(234,0,__PYX_ERR(0, 234, __pyx_L1_error))
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_circuit, __pyx_n_s_circuit); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 234, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (likely(PyList_CheckExact(__pyx_t_5)) || PyTuple_CheckExact(__pyx_t_5)) {
     __pyx_t_1 = __pyx_t_5; __Pyx_INCREF(__pyx_t_1); __pyx_t_6 = 0;
     __pyx_t_7 = NULL;
   } else {
-    __pyx_t_6 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 221, __pyx_L1_error)
+    __pyx_t_6 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 234, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_7 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 221, __pyx_L1_error)
+    __pyx_t_7 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 234, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   for (;;) {
     if (likely(!__pyx_t_7)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_6); __Pyx_INCREF(__pyx_t_5); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 221, __pyx_L1_error)
+        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_6); __Pyx_INCREF(__pyx_t_5); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 234, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_1, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 221, __pyx_L1_error)
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_1, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 234, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       } else {
         if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_6); __Pyx_INCREF(__pyx_t_5); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 221, __pyx_L1_error)
+        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_6); __Pyx_INCREF(__pyx_t_5); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 234, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_1, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 221, __pyx_L1_error)
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_1, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 234, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       }
     } else {
       __pyx_t_5 = __pyx_t_7(__pyx_t_1);
       if (unlikely(!__pyx_t_5)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 221, __pyx_L1_error)
+          else __PYX_ERR(0, 234, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_5);
     }
     __Pyx_XDECREF_SET(__pyx_v_op, __pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "dwave/gate/simulator/simulator.pyx":222
+    /* "dwave/gate/simulator/simulator.pyx":235
  * 
  *     for op in circuit.circuit:
  *         if isinstance(op, ops.Measurement):             # <<<<<<<<<<<<<<
  *             _measure(op, state, circuit, rng)
  *         else:
  */
-    __Pyx_TraceLine(222,0,__PYX_ERR(0, 222, __pyx_L1_error))
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_ops); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 222, __pyx_L1_error)
+    __Pyx_TraceLine(235,0,__PYX_ERR(0, 235, __pyx_L1_error))
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_ops); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 235, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_Measurement); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 222, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_Measurement); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 235, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_8 = PyObject_IsInstance(__pyx_v_op, __pyx_t_3); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 222, __pyx_L1_error)
+    __pyx_t_8 = PyObject_IsInstance(__pyx_v_op, __pyx_t_3); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 235, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_9 = (__pyx_t_8 != 0);
     if (__pyx_t_9) {
 
-      /* "dwave/gate/simulator/simulator.pyx":223
+      /* "dwave/gate/simulator/simulator.pyx":236
  *     for op in circuit.circuit:
  *         if isinstance(op, ops.Measurement):
  *             _measure(op, state, circuit, rng)             # <<<<<<<<<<<<<<
  *         else:
  *             # first apply the gate normally
  */
-      __Pyx_TraceLine(223,0,__PYX_ERR(0, 223, __pyx_L1_error))
-      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_measure); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 223, __pyx_L1_error)
+      __Pyx_TraceLine(236,0,__PYX_ERR(0, 236, __pyx_L1_error))
+      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_measure); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 236, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_2 = NULL;
       __pyx_t_10 = 0;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
         __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
         if (likely(__pyx_t_2)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -6306,29 +6306,29 @@
           __Pyx_DECREF_SET(__pyx_t_5, function);
           __pyx_t_10 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_5)) {
         PyObject *__pyx_temp[5] = {__pyx_t_2, __pyx_v_op, __pyx_v_state, __pyx_v_circuit, __pyx_v_rng};
-        __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_10, 4+__pyx_t_10); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 223, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_10, 4+__pyx_t_10); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 236, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_GOTREF(__pyx_t_3);
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
         PyObject *__pyx_temp[5] = {__pyx_t_2, __pyx_v_op, __pyx_v_state, __pyx_v_circuit, __pyx_v_rng};
-        __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_10, 4+__pyx_t_10); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 223, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_10, 4+__pyx_t_10); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 236, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_GOTREF(__pyx_t_3);
       } else
       #endif
       {
-        __pyx_t_4 = PyTuple_New(4+__pyx_t_10); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 223, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_New(4+__pyx_t_10); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 236, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         if (__pyx_t_2) {
           __Pyx_GIVEREF(__pyx_t_2); PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2); __pyx_t_2 = NULL;
         }
         __Pyx_INCREF(__pyx_v_op);
         __Pyx_GIVEREF(__pyx_v_op);
         PyTuple_SET_ITEM(__pyx_t_4, 0+__pyx_t_10, __pyx_v_op);
@@ -6337,140 +6337,140 @@
         PyTuple_SET_ITEM(__pyx_t_4, 1+__pyx_t_10, __pyx_v_state);
         __Pyx_INCREF(__pyx_v_circuit);
         __Pyx_GIVEREF(__pyx_v_circuit);
         PyTuple_SET_ITEM(__pyx_t_4, 2+__pyx_t_10, __pyx_v_circuit);
         __Pyx_INCREF(__pyx_v_rng);
         __Pyx_GIVEREF(__pyx_v_rng);
         PyTuple_SET_ITEM(__pyx_t_4, 3+__pyx_t_10, __pyx_v_rng);
-        __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 223, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 236, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       }
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "dwave/gate/simulator/simulator.pyx":222
+      /* "dwave/gate/simulator/simulator.pyx":235
  * 
  *     for op in circuit.circuit:
  *         if isinstance(op, ops.Measurement):             # <<<<<<<<<<<<<<
  *             _measure(op, state, circuit, rng)
  *         else:
  */
       goto __pyx_L5;
     }
 
-    /* "dwave/gate/simulator/simulator.pyx":226
+    /* "dwave/gate/simulator/simulator.pyx":239
  *         else:
  *             # first apply the gate normally
  *             targets = [circuit.qubits.index(qb) for qb in op.qubits]             # <<<<<<<<<<<<<<
  *             apply_instruction(
  *                 num_virtual_qubits, state, op, targets, little_endian, rng
  */
-    __Pyx_TraceLine(226,0,__PYX_ERR(0, 226, __pyx_L1_error))
+    __Pyx_TraceLine(239,0,__PYX_ERR(0, 239, __pyx_L1_error))
     /*else*/ {
       { /* enter inner scope */
-        __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 226, __pyx_L8_error)
+        __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 239, __pyx_L8_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_op, __pyx_n_s_qubits); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 226, __pyx_L8_error)
+        __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_op, __pyx_n_s_qubits); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 239, __pyx_L8_error)
         __Pyx_GOTREF(__pyx_t_5);
         if (likely(PyList_CheckExact(__pyx_t_5)) || PyTuple_CheckExact(__pyx_t_5)) {
           __pyx_t_4 = __pyx_t_5; __Pyx_INCREF(__pyx_t_4); __pyx_t_11 = 0;
           __pyx_t_12 = NULL;
         } else {
-          __pyx_t_11 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 226, __pyx_L8_error)
+          __pyx_t_11 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 239, __pyx_L8_error)
           __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_12 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 226, __pyx_L8_error)
+          __pyx_t_12 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 239, __pyx_L8_error)
         }
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         for (;;) {
           if (likely(!__pyx_t_12)) {
             if (likely(PyList_CheckExact(__pyx_t_4))) {
               if (__pyx_t_11 >= PyList_GET_SIZE(__pyx_t_4)) break;
               #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-              __pyx_t_5 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_11); __Pyx_INCREF(__pyx_t_5); __pyx_t_11++; if (unlikely(0 < 0)) __PYX_ERR(0, 226, __pyx_L8_error)
+              __pyx_t_5 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_11); __Pyx_INCREF(__pyx_t_5); __pyx_t_11++; if (unlikely(0 < 0)) __PYX_ERR(0, 239, __pyx_L8_error)
               #else
-              __pyx_t_5 = PySequence_ITEM(__pyx_t_4, __pyx_t_11); __pyx_t_11++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 226, __pyx_L8_error)
+              __pyx_t_5 = PySequence_ITEM(__pyx_t_4, __pyx_t_11); __pyx_t_11++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 239, __pyx_L8_error)
               __Pyx_GOTREF(__pyx_t_5);
               #endif
             } else {
               if (__pyx_t_11 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
               #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-              __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_11); __Pyx_INCREF(__pyx_t_5); __pyx_t_11++; if (unlikely(0 < 0)) __PYX_ERR(0, 226, __pyx_L8_error)
+              __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_11); __Pyx_INCREF(__pyx_t_5); __pyx_t_11++; if (unlikely(0 < 0)) __PYX_ERR(0, 239, __pyx_L8_error)
               #else
-              __pyx_t_5 = PySequence_ITEM(__pyx_t_4, __pyx_t_11); __pyx_t_11++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 226, __pyx_L8_error)
+              __pyx_t_5 = PySequence_ITEM(__pyx_t_4, __pyx_t_11); __pyx_t_11++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 239, __pyx_L8_error)
               __Pyx_GOTREF(__pyx_t_5);
               #endif
             }
           } else {
             __pyx_t_5 = __pyx_t_12(__pyx_t_4);
             if (unlikely(!__pyx_t_5)) {
               PyObject* exc_type = PyErr_Occurred();
               if (exc_type) {
                 if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-                else __PYX_ERR(0, 226, __pyx_L8_error)
+                else __PYX_ERR(0, 239, __pyx_L8_error)
               }
               break;
             }
             __Pyx_GOTREF(__pyx_t_5);
           }
           __Pyx_XDECREF_SET(__pyx_8genexpr1__pyx_v_qb, __pyx_t_5);
           __pyx_t_5 = 0;
-          __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_circuit, __pyx_n_s_qubits); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 226, __pyx_L8_error)
+          __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_circuit, __pyx_n_s_qubits); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 239, __pyx_L8_error)
           __Pyx_GOTREF(__pyx_t_2);
-          __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_index); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 226, __pyx_L8_error)
+          __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_index); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 239, __pyx_L8_error)
           __Pyx_GOTREF(__pyx_t_13);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __pyx_t_2 = NULL;
           if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_13))) {
             __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_13);
             if (likely(__pyx_t_2)) {
               PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_13);
               __Pyx_INCREF(__pyx_t_2);
               __Pyx_INCREF(function);
               __Pyx_DECREF_SET(__pyx_t_13, function);
             }
           }
           __pyx_t_5 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_13, __pyx_t_2, __pyx_8genexpr1__pyx_v_qb) : __Pyx_PyObject_CallOneArg(__pyx_t_13, __pyx_8genexpr1__pyx_v_qb);
           __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-          if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 226, __pyx_L8_error)
+          if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 239, __pyx_L8_error)
           __Pyx_GOTREF(__pyx_t_5);
           __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-          if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 226, __pyx_L8_error)
+          if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 239, __pyx_L8_error)
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         }
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_qb); __pyx_8genexpr1__pyx_v_qb = 0;
         goto __pyx_L11_exit_scope;
         __pyx_L8_error:;
         __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_qb); __pyx_8genexpr1__pyx_v_qb = 0;
         goto __pyx_L1_error;
         __pyx_L11_exit_scope:;
       } /* exit inner scope */
       __Pyx_XDECREF_SET(__pyx_v_targets, ((PyObject*)__pyx_t_3));
       __pyx_t_3 = 0;
 
-      /* "dwave/gate/simulator/simulator.pyx":227
+      /* "dwave/gate/simulator/simulator.pyx":240
  *             # first apply the gate normally
  *             targets = [circuit.qubits.index(qb) for qb in op.qubits]
  *             apply_instruction(             # <<<<<<<<<<<<<<
  *                 num_virtual_qubits, state, op, targets, little_endian, rng
  *             )
  */
-      __Pyx_TraceLine(227,0,__PYX_ERR(0, 227, __pyx_L1_error))
-      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_apply_instruction); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 227, __pyx_L1_error)
+      __Pyx_TraceLine(240,0,__PYX_ERR(0, 240, __pyx_L1_error))
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_apply_instruction); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 240, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
 
-      /* "dwave/gate/simulator/simulator.pyx":228
+      /* "dwave/gate/simulator/simulator.pyx":241
  *             targets = [circuit.qubits.index(qb) for qb in op.qubits]
  *             apply_instruction(
  *                 num_virtual_qubits, state, op, targets, little_endian, rng             # <<<<<<<<<<<<<<
  *             )
  *             # then apply conjugate transpose to corresponding virtual qubit
  */
-      __Pyx_TraceLine(228,0,__PYX_ERR(0, 228, __pyx_L1_error))
+      __Pyx_TraceLine(241,0,__PYX_ERR(0, 241, __pyx_L1_error))
       __pyx_t_5 = NULL;
       __pyx_t_10 = 0;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_5)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_5);
@@ -6478,29 +6478,29 @@
           __Pyx_DECREF_SET(__pyx_t_4, function);
           __pyx_t_10 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_4)) {
         PyObject *__pyx_temp[7] = {__pyx_t_5, __pyx_v_num_virtual_qubits, __pyx_v_state, __pyx_v_op, __pyx_v_targets, __pyx_v_little_endian, __pyx_v_rng};
-        __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_10, 6+__pyx_t_10); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 227, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_10, 6+__pyx_t_10); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 240, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_GOTREF(__pyx_t_3);
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
         PyObject *__pyx_temp[7] = {__pyx_t_5, __pyx_v_num_virtual_qubits, __pyx_v_state, __pyx_v_op, __pyx_v_targets, __pyx_v_little_endian, __pyx_v_rng};
-        __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_10, 6+__pyx_t_10); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 227, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_10, 6+__pyx_t_10); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 240, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_GOTREF(__pyx_t_3);
       } else
       #endif
       {
-        __pyx_t_13 = PyTuple_New(6+__pyx_t_10); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 227, __pyx_L1_error)
+        __pyx_t_13 = PyTuple_New(6+__pyx_t_10); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 240, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_13);
         if (__pyx_t_5) {
           __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_13, 0, __pyx_t_5); __pyx_t_5 = NULL;
         }
         __Pyx_INCREF(__pyx_v_num_virtual_qubits);
         __Pyx_GIVEREF(__pyx_v_num_virtual_qubits);
         PyTuple_SET_ITEM(__pyx_t_13, 0+__pyx_t_10, __pyx_v_num_virtual_qubits);
@@ -6515,79 +6515,79 @@
         PyTuple_SET_ITEM(__pyx_t_13, 3+__pyx_t_10, __pyx_v_targets);
         __Pyx_INCREF(__pyx_v_little_endian);
         __Pyx_GIVEREF(__pyx_v_little_endian);
         PyTuple_SET_ITEM(__pyx_t_13, 4+__pyx_t_10, __pyx_v_little_endian);
         __Pyx_INCREF(__pyx_v_rng);
         __Pyx_GIVEREF(__pyx_v_rng);
         PyTuple_SET_ITEM(__pyx_t_13, 5+__pyx_t_10, __pyx_v_rng);
-        __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_13, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 227, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_13, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 240, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
       }
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "dwave/gate/simulator/simulator.pyx":231
+      /* "dwave/gate/simulator/simulator.pyx":244
  *             )
  *             # then apply conjugate transpose to corresponding virtual qubit
  *             virtual_targets = [t + num_qubits for t in targets]             # <<<<<<<<<<<<<<
  *             apply_instruction(
  *                 num_virtual_qubits, state, op, virtual_targets, little_endian, rng,
  */
-      __Pyx_TraceLine(231,0,__PYX_ERR(0, 231, __pyx_L1_error))
+      __Pyx_TraceLine(244,0,__PYX_ERR(0, 244, __pyx_L1_error))
       { /* enter inner scope */
-        __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 231, __pyx_L14_error)
+        __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 244, __pyx_L14_error)
         __Pyx_GOTREF(__pyx_t_3);
         __pyx_t_4 = __pyx_v_targets; __Pyx_INCREF(__pyx_t_4); __pyx_t_11 = 0;
         for (;;) {
           if (__pyx_t_11 >= PyList_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_13 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_11); __Pyx_INCREF(__pyx_t_13); __pyx_t_11++; if (unlikely(0 < 0)) __PYX_ERR(0, 231, __pyx_L14_error)
+          __pyx_t_13 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_11); __Pyx_INCREF(__pyx_t_13); __pyx_t_11++; if (unlikely(0 < 0)) __PYX_ERR(0, 244, __pyx_L14_error)
           #else
-          __pyx_t_13 = PySequence_ITEM(__pyx_t_4, __pyx_t_11); __pyx_t_11++; if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 231, __pyx_L14_error)
+          __pyx_t_13 = PySequence_ITEM(__pyx_t_4, __pyx_t_11); __pyx_t_11++; if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 244, __pyx_L14_error)
           __Pyx_GOTREF(__pyx_t_13);
           #endif
           __Pyx_XDECREF_SET(__pyx_8genexpr2__pyx_v_t, __pyx_t_13);
           __pyx_t_13 = 0;
-          __pyx_t_13 = PyNumber_Add(__pyx_8genexpr2__pyx_v_t, __pyx_v_num_qubits); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 231, __pyx_L14_error)
+          __pyx_t_13 = PyNumber_Add(__pyx_8genexpr2__pyx_v_t, __pyx_v_num_qubits); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 244, __pyx_L14_error)
           __Pyx_GOTREF(__pyx_t_13);
-          if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_13))) __PYX_ERR(0, 231, __pyx_L14_error)
+          if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_13))) __PYX_ERR(0, 244, __pyx_L14_error)
           __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
         }
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_t); __pyx_8genexpr2__pyx_v_t = 0;
         goto __pyx_L17_exit_scope;
         __pyx_L14_error:;
         __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_t); __pyx_8genexpr2__pyx_v_t = 0;
         goto __pyx_L1_error;
         __pyx_L17_exit_scope:;
       } /* exit inner scope */
       __Pyx_XDECREF_SET(__pyx_v_virtual_targets, ((PyObject*)__pyx_t_3));
       __pyx_t_3 = 0;
 
-      /* "dwave/gate/simulator/simulator.pyx":232
+      /* "dwave/gate/simulator/simulator.pyx":245
  *             # then apply conjugate transpose to corresponding virtual qubit
  *             virtual_targets = [t + num_qubits for t in targets]
  *             apply_instruction(             # <<<<<<<<<<<<<<
  *                 num_virtual_qubits, state, op, virtual_targets, little_endian, rng,
  *                 conjugate_gate=True,
  */
-      __Pyx_TraceLine(232,0,__PYX_ERR(0, 232, __pyx_L1_error))
-      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_apply_instruction); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 232, __pyx_L1_error)
+      __Pyx_TraceLine(245,0,__PYX_ERR(0, 245, __pyx_L1_error))
+      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_apply_instruction); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 245, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
 
-      /* "dwave/gate/simulator/simulator.pyx":233
+      /* "dwave/gate/simulator/simulator.pyx":246
  *             virtual_targets = [t + num_qubits for t in targets]
  *             apply_instruction(
  *                 num_virtual_qubits, state, op, virtual_targets, little_endian, rng,             # <<<<<<<<<<<<<<
  *                 conjugate_gate=True,
  *             )
  */
-      __Pyx_TraceLine(233,0,__PYX_ERR(0, 233, __pyx_L1_error))
-      __pyx_t_4 = PyTuple_New(6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 232, __pyx_L1_error)
+      __Pyx_TraceLine(246,0,__PYX_ERR(0, 246, __pyx_L1_error))
+      __pyx_t_4 = PyTuple_New(6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 245, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_INCREF(__pyx_v_num_virtual_qubits);
       __Pyx_GIVEREF(__pyx_v_num_virtual_qubits);
       PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_num_virtual_qubits);
       __Pyx_INCREF(__pyx_v_state);
       __Pyx_GIVEREF(__pyx_v_state);
       PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_v_state);
@@ -6600,69 +6600,69 @@
       __Pyx_INCREF(__pyx_v_little_endian);
       __Pyx_GIVEREF(__pyx_v_little_endian);
       PyTuple_SET_ITEM(__pyx_t_4, 4, __pyx_v_little_endian);
       __Pyx_INCREF(__pyx_v_rng);
       __Pyx_GIVEREF(__pyx_v_rng);
       PyTuple_SET_ITEM(__pyx_t_4, 5, __pyx_v_rng);
 
-      /* "dwave/gate/simulator/simulator.pyx":234
+      /* "dwave/gate/simulator/simulator.pyx":247
  *             apply_instruction(
  *                 num_virtual_qubits, state, op, virtual_targets, little_endian, rng,
  *                 conjugate_gate=True,             # <<<<<<<<<<<<<<
  *             )
  *     density_matrix = state.reshape((1 << num_qubits, 1 << num_qubits))
  */
-      __Pyx_TraceLine(234,0,__PYX_ERR(0, 234, __pyx_L1_error))
-      __pyx_t_13 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 234, __pyx_L1_error)
+      __Pyx_TraceLine(247,0,__PYX_ERR(0, 247, __pyx_L1_error))
+      __pyx_t_13 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 247, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_13);
-      if (PyDict_SetItem(__pyx_t_13, __pyx_n_s_conjugate_gate, Py_True) < 0) __PYX_ERR(0, 234, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_13, __pyx_n_s_conjugate_gate, Py_True) < 0) __PYX_ERR(0, 247, __pyx_L1_error)
 
-      /* "dwave/gate/simulator/simulator.pyx":232
+      /* "dwave/gate/simulator/simulator.pyx":245
  *             # then apply conjugate transpose to corresponding virtual qubit
  *             virtual_targets = [t + num_qubits for t in targets]
  *             apply_instruction(             # <<<<<<<<<<<<<<
  *                 num_virtual_qubits, state, op, virtual_targets, little_endian, rng,
  *                 conjugate_gate=True,
  */
-      __Pyx_TraceLine(232,0,__PYX_ERR(0, 232, __pyx_L1_error))
-      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_13); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 232, __pyx_L1_error)
+      __Pyx_TraceLine(245,0,__PYX_ERR(0, 245, __pyx_L1_error))
+      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_13); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 245, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __pyx_L5:;
 
-    /* "dwave/gate/simulator/simulator.pyx":221
+    /* "dwave/gate/simulator/simulator.pyx":234
  *     state[0] = 1
  * 
  *     for op in circuit.circuit:             # <<<<<<<<<<<<<<
  *         if isinstance(op, ops.Measurement):
  *             _measure(op, state, circuit, rng)
  */
-    __Pyx_TraceLine(221,0,__PYX_ERR(0, 221, __pyx_L1_error))
+    __Pyx_TraceLine(234,0,__PYX_ERR(0, 234, __pyx_L1_error))
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "dwave/gate/simulator/simulator.pyx":236
+  /* "dwave/gate/simulator/simulator.pyx":249
  *                 conjugate_gate=True,
  *             )
  *     density_matrix = state.reshape((1 << num_qubits, 1 << num_qubits))             # <<<<<<<<<<<<<<
  * 
  *     return density_matrix
  */
-  __Pyx_TraceLine(236,0,__PYX_ERR(0, 236, __pyx_L1_error))
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_reshape); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __Pyx_TraceLine(249,0,__PYX_ERR(0, 249, __pyx_L1_error))
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_reshape); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_13 = PyNumber_Lshift(__pyx_int_1, __pyx_v_num_qubits); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __pyx_t_13 = PyNumber_Lshift(__pyx_int_1, __pyx_v_num_qubits); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
-  __pyx_t_4 = PyNumber_Lshift(__pyx_int_1, __pyx_v_num_qubits); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __pyx_t_4 = PyNumber_Lshift(__pyx_int_1, __pyx_v_num_qubits); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_13);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_13);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_4);
   __pyx_t_13 = 0;
   __pyx_t_4 = 0;
@@ -6675,32 +6675,32 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 236, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_density_matrix = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "dwave/gate/simulator/simulator.pyx":238
+  /* "dwave/gate/simulator/simulator.pyx":251
  *     density_matrix = state.reshape((1 << num_qubits, 1 << num_qubits))
  * 
  *     return density_matrix             # <<<<<<<<<<<<<<
  */
-  __Pyx_TraceLine(238,0,__PYX_ERR(0, 238, __pyx_L1_error))
+  __Pyx_TraceLine(251,0,__PYX_ERR(0, 251, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_density_matrix);
   __pyx_r = __pyx_v_density_matrix;
   goto __pyx_L0;
 
-  /* "dwave/gate/simulator/simulator.pyx":210
+  /* "dwave/gate/simulator/simulator.pyx":223
  * 
  * 
  * def _simulate_circuit_density_matrix(             # <<<<<<<<<<<<<<
  *     circuit: Circuit,
  *     rng: np.random.Generator,
  */
 
@@ -7321,15 +7321,15 @@
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __Pyx_TraceLine(945,0,__PYX_ERR(1, 945, __pyx_L5_except_error))
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -7460,15 +7460,15 @@
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __Pyx_TraceLine(951,0,__PYX_ERR(1, 951, __pyx_L5_except_error))
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -7599,15 +7599,15 @@
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __Pyx_TraceLine(957,0,__PYX_ERR(1, 957, __pyx_L5_except_error))
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -9022,15 +9022,15 @@
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 384, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 384, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(2, 384, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__10, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 384, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__9, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 384, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_norms = __pyx_t_4;
   __pyx_t_4 = 0;
 
   /* "dwave/gate/simulator/ops.pxd":387
@@ -9627,15 +9627,15 @@
  * 
  *     if p == 0.0:
  *         raise RuntimeError("cannot normalize state vector, norm too small")             # <<<<<<<<<<<<<<
  * 
  *     normalization_factor = 1 / np.sqrt(p)
  */
     __Pyx_TraceLine(465,0,__PYX_ERR(2, 465, __pyx_L1_error))
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 465, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 465, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __PYX_ERR(2, 465, __pyx_L1_error)
 
     /* "dwave/gate/simulator/ops.pxd":464
  * 
@@ -10074,15 +10074,15 @@
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 526, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 526, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(2, 526, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__10, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 526, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__9, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 526, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_norms = __pyx_t_4;
   __pyx_t_4 = 0;
 
   /* "dwave/gate/simulator/ops.pxd":529
@@ -10679,15 +10679,15 @@
  * 
  *     if p == 0.0:
  *         raise RuntimeError("cannot normalize state vector, norm too small")             # <<<<<<<<<<<<<<
  * 
  *     normalization_factor = 1 / np.sqrt(p)
  */
     __Pyx_TraceLine(607,0,__PYX_ERR(2, 607, __pyx_L1_error))
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 607, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 607, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __PYX_ERR(2, 607, __pyx_L1_error)
 
     /* "dwave/gate/simulator/ops.pxd":606
  * 
@@ -11126,15 +11126,15 @@
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 668, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 668, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(2, 668, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__10, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 668, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__9, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 668, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_norms = __pyx_t_4;
   __pyx_t_4 = 0;
 
   /* "dwave/gate/simulator/ops.pxd":671
@@ -11731,15 +11731,15 @@
  * 
  *     if p == 0.0:
  *         raise RuntimeError("cannot normalize state vector, norm too small")             # <<<<<<<<<<<<<<
  * 
  *     normalization_factor = 1 / np.sqrt(p)
  */
     __Pyx_TraceLine(749,0,__PYX_ERR(2, 749, __pyx_L1_error))
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 749, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 749, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __PYX_ERR(2, 749, __pyx_L1_error)
 
     /* "dwave/gate/simulator/ops.pxd":748
  * 
@@ -12306,15 +12306,15 @@
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
     __Pyx_TraceLine(134,0,__PYX_ERR(3, 134, __pyx_L1_error))
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 134, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 134, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(3, 134, __pyx_L1_error)
 
     /* "View.MemoryView":133
  *         self.itemsize = itemsize
@@ -12340,15 +12340,15 @@
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
     __Pyx_TraceLine(137,0,__PYX_ERR(3, 137, __pyx_L1_error))
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 137, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 137, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(3, 137, __pyx_L1_error)
 
     /* "View.MemoryView":136
  *             raise ValueError("Empty shape tuple for cython.array")
@@ -12475,15 +12475,15 @@
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __Pyx_TraceLine(149,0,__PYX_ERR(3, 149, __pyx_L1_error))
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 149, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 149, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(3, 149, __pyx_L1_error)
 
     /* "View.MemoryView":148
  *         self._strides = self._shape + self.ndim
@@ -12768,15 +12768,15 @@
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
       __Pyx_TraceLine(177,0,__PYX_ERR(3, 177, __pyx_L1_error))
-      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(3, 177, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(3, 177, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_Raise(__pyx_t_10, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __PYX_ERR(3, 177, __pyx_L1_error)
 
       /* "View.MemoryView":176
  * 
@@ -13027,15 +13027,15 @@
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
     __Pyx_TraceLine(193,0,__PYX_ERR(3, 193, __pyx_L1_error))
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 193, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(3, 193, __pyx_L1_error)
 
     /* "View.MemoryView":192
  *         elif self.mode == u"fortran":
@@ -13825,15 +13825,15 @@
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
   __Pyx_TraceLine(2,0,__PYX_ERR(3, 2, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(3, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -13885,15 +13885,15 @@
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __Pyx_TraceLine(4,0,__PYX_ERR(3, 4, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(3, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -15745,15 +15745,15 @@
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
     __Pyx_TraceLine(420,0,__PYX_ERR(3, 420, __pyx_L1_error))
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 420, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 420, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(3, 420, __pyx_L1_error)
 
     /* "View.MemoryView":419
  * 
@@ -16854,15 +16854,15 @@
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
       __Pyx_TraceLine(497,0,__PYX_ERR(3, 497, __pyx_L5_except_error))
-      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(3, 497, __pyx_L5_except_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(3, 497, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __PYX_ERR(3, 497, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -17232,15 +17232,15 @@
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
     __Pyx_TraceLine(522,0,__PYX_ERR(3, 522, __pyx_L1_error))
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__21, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 522, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 522, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(3, 522, __pyx_L1_error)
 
     /* "View.MemoryView":521
  *     @cname('getbuffer')
@@ -17824,15 +17824,15 @@
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
     __Pyx_TraceLine(572,0,__PYX_ERR(3, 572, __pyx_L1_error))
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 572, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__21, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 572, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(3, 572, __pyx_L1_error)
 
     /* "View.MemoryView":570
  *     @property
@@ -17947,15 +17947,15 @@
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
     __Pyx_TraceLine(579,0,__PYX_ERR(3, 579, __pyx_L1_error))
     __Pyx_XDECREF(__pyx_r);
     __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__23, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 579, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__22, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
     /* "View.MemoryView":578
@@ -19057,15 +19057,15 @@
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
   __Pyx_TraceLine(2,0,__PYX_ERR(3, 2, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(3, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -19117,15 +19117,15 @@
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __Pyx_TraceLine(4,0,__PYX_ERR(3, 4, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(3, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -19503,17 +19503,17 @@
  */
         __Pyx_TraceLine(684,0,__PYX_ERR(3, 684, __pyx_L1_error))
         __pyx_t_8 = PyObject_Length(__pyx_v_tup); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(3, 684, __pyx_L1_error)
         __pyx_t_7 = PyList_New(1 * ((((__pyx_v_ndim - __pyx_t_8) + 1)<0) ? 0:((__pyx_v_ndim - __pyx_t_8) + 1))); if (unlikely(!__pyx_t_7)) __PYX_ERR(3, 684, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         { Py_ssize_t __pyx_temp;
           for (__pyx_temp=0; __pyx_temp < ((__pyx_v_ndim - __pyx_t_8) + 1); __pyx_temp++) {
-            __Pyx_INCREF(__pyx_slice__26);
-            __Pyx_GIVEREF(__pyx_slice__26);
-            PyList_SET_ITEM(__pyx_t_7, __pyx_temp, __pyx_slice__26);
+            __Pyx_INCREF(__pyx_slice__25);
+            __Pyx_GIVEREF(__pyx_slice__25);
+            PyList_SET_ITEM(__pyx_t_7, __pyx_temp, __pyx_slice__25);
           }
         }
         __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(3, 684, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
         /* "View.MemoryView":685
  *             if not seen_ellipsis:
@@ -19540,15 +19540,15 @@
  *             else:
  *                 result.append(slice(None))             # <<<<<<<<<<<<<<
  *             have_slices = True
  *         else:
  */
       __Pyx_TraceLine(687,0,__PYX_ERR(3, 687, __pyx_L1_error))
       /*else*/ {
-        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__26); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(3, 687, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__25); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(3, 687, __pyx_L1_error)
       }
       __pyx_L7:;
 
       /* "View.MemoryView":688
  *             else:
  *                 result.append(slice(None))
  *             have_slices = True             # <<<<<<<<<<<<<<
@@ -19689,17 +19689,17 @@
  *     return have_slices or nslices, tuple(result)
  */
     __Pyx_TraceLine(698,0,__PYX_ERR(3, 698, __pyx_L1_error))
     __pyx_t_3 = PyList_New(1 * ((__pyx_v_nslices<0) ? 0:__pyx_v_nslices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 698, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     { Py_ssize_t __pyx_temp;
       for (__pyx_temp=0; __pyx_temp < __pyx_v_nslices; __pyx_temp++) {
-        __Pyx_INCREF(__pyx_slice__26);
-        __Pyx_GIVEREF(__pyx_slice__26);
-        PyList_SET_ITEM(__pyx_t_3, __pyx_temp, __pyx_slice__26);
+        __Pyx_INCREF(__pyx_slice__25);
+        __Pyx_GIVEREF(__pyx_slice__25);
+        PyList_SET_ITEM(__pyx_t_3, __pyx_temp, __pyx_slice__25);
       }
     }
     __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_3); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(3, 698, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "View.MemoryView":697
  * 
@@ -19825,15 +19825,15 @@
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __Pyx_TraceLine(705,0,__PYX_ERR(3, 705, __pyx_L1_error))
-      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 705, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 705, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_Raise(__pyx_t_5, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __PYX_ERR(3, 705, __pyx_L1_error)
 
       /* "View.MemoryView":704
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
@@ -22173,15 +22173,15 @@
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
   __Pyx_TraceLine(2,0,__PYX_ERR(3, 2, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(3, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -22233,15 +22233,15 @@
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __Pyx_TraceLine(4,0,__PYX_ERR(3, 4, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__29, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(3, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -25822,29 +25822,29 @@
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceFrameInit(__pyx_codeobj__30)
+  __Pyx_TraceFrameInit(__pyx_codeobj__29)
   __Pyx_RefNannySetupContext("__pyx_unpickle_Enum", 0);
   __Pyx_TraceCall("__pyx_unpickle_Enum", __pyx_f[3], 1, 0, __PYX_ERR(3, 1, __pyx_L1_error));
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  */
   __Pyx_TraceLine(4,0,__PYX_ERR(3, 4, __pyx_L1_error))
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__31, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(3, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__30, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(3, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):
@@ -26953,15 +26953,15 @@
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_RuntimeError, __pyx_k_RuntimeError, sizeof(__pyx_k_RuntimeError), 0, 0, 1, 1},
   {&__pyx_n_s_SWAP, __pyx_k_SWAP, sizeof(__pyx_k_SWAP), 0, 0, 1, 1},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_kp_s_Unable_to_convert_item_to_object, __pyx_k_Unable_to_convert_item_to_object, sizeof(__pyx_k_Unable_to_convert_item_to_object), 0, 0, 1, 0},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_View_MemoryView, __pyx_k_View_MemoryView, sizeof(__pyx_k_View_MemoryView), 0, 0, 1, 1},
-  {&__pyx_n_s__32, __pyx_k__32, sizeof(__pyx_k__32), 0, 0, 1, 1},
+  {&__pyx_n_s__31, __pyx_k__31, sizeof(__pyx_k__31), 0, 0, 1, 1},
   {&__pyx_n_s_all, __pyx_k_all, sizeof(__pyx_k_all), 0, 0, 1, 1},
   {&__pyx_n_s_allocate_buffer, __pyx_k_allocate_buffer, sizeof(__pyx_k_allocate_buffer), 0, 0, 1, 1},
   {&__pyx_n_s_append, __pyx_k_append, sizeof(__pyx_k_append), 0, 0, 1, 1},
   {&__pyx_n_s_apply_instruction, __pyx_k_apply_instruction, sizeof(__pyx_k_apply_instruction), 0, 0, 1, 1},
   {&__pyx_n_s_array, __pyx_k_array, sizeof(__pyx_k_array), 0, 0, 1, 1},
   {&__pyx_n_s_ascontiguousarray, __pyx_k_ascontiguousarray, sizeof(__pyx_k_ascontiguousarray), 0, 0, 1, 1},
   {&__pyx_n_s_base, __pyx_k_base, sizeof(__pyx_k_base), 0, 0, 1, 1},
@@ -27057,16 +27057,18 @@
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
   {&__pyx_n_s_reshape, __pyx_k_reshape, sizeof(__pyx_k_reshape), 0, 0, 1, 1},
   {&__pyx_n_s_rng, __pyx_k_rng, sizeof(__pyx_k_rng), 0, 0, 1, 1},
   {&__pyx_n_s_rng_seed, __pyx_k_rng_seed, sizeof(__pyx_k_rng_seed), 0, 0, 1, 1},
   {&__pyx_n_s_round, __pyx_k_round, sizeof(__pyx_k_round), 0, 0, 1, 1},
-  {&__pyx_n_s_sample, __pyx_k_sample, sizeof(__pyx_k_sample), 0, 0, 1, 1},
+  {&__pyx_n_s_sample_qubit, __pyx_k_sample_qubit, sizeof(__pyx_k_sample_qubit), 0, 0, 1, 1},
+  {&__pyx_n_u_sample_qubit, __pyx_k_sample_qubit, sizeof(__pyx_k_sample_qubit), 0, 1, 0, 1},
   {&__pyx_n_s_set, __pyx_k_set, sizeof(__pyx_k_set), 0, 0, 1, 1},
+  {&__pyx_n_s_set_state, __pyx_k_set_state, sizeof(__pyx_k_set_state), 0, 0, 1, 1},
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
   {&__pyx_n_s_shape, __pyx_k_shape, sizeof(__pyx_k_shape), 0, 0, 1, 1},
   {&__pyx_n_s_simulate, __pyx_k_simulate, sizeof(__pyx_k_simulate), 0, 0, 1, 1},
   {&__pyx_n_u_simulate, __pyx_k_simulate, sizeof(__pyx_k_simulate), 0, 1, 0, 1},
   {&__pyx_n_s_simulate_circuit_density_matrix, __pyx_k_simulate_circuit_density_matrix, sizeof(__pyx_k_simulate_circuit_density_matrix), 0, 0, 1, 1},
   {&__pyx_kp_u_simulator_encountered_unknown_mu, __pyx_k_simulator_encountered_unknown_mu, sizeof(__pyx_k_simulator_encountered_unknown_mu), 0, 1, 0, 0},
@@ -27098,19 +27100,19 @@
   {&__pyx_n_s_virtual_targets, __pyx_k_virtual_targets, sizeof(__pyx_k_virtual_targets), 0, 0, 1, 1},
   {&__pyx_n_s_warn, __pyx_k_warn, sizeof(__pyx_k_warn), 0, 0, 1, 1},
   {&__pyx_n_s_warnings, __pyx_k_warnings, sizeof(__pyx_k_warnings), 0, 0, 1, 1},
   {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 122, __pyx_L1_error)
-  __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(0, 180, __pyx_L1_error)
-  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(0, 185, __pyx_L1_error)
-  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 185, __pyx_L1_error)
-  __pyx_builtin_round = __Pyx_GetBuiltinName(__pyx_n_s_round); if (!__pyx_builtin_round) __PYX_ERR(0, 198, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 123, __pyx_L1_error)
+  __pyx_builtin_round = __Pyx_GetBuiltinName(__pyx_n_s_round); if (!__pyx_builtin_round) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(0, 212, __pyx_L1_error)
+  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(0, 217, __pyx_L1_error)
+  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 217, __pyx_L1_error)
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 945, __pyx_L1_error)
   __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(2, 465, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(3, 149, __pyx_L1_error)
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(3, 181, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(3, 406, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(3, 615, __pyx_L1_error)
   return 0;
@@ -27118,399 +27120,388 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "dwave/gate/simulator/simulator.pyx":98
+  /* "dwave/gate/simulator/simulator.pyx":99
  *         else:
  *             gate = op.target_operation.matrix
  *         assert gate.shape == (2, 2), (op, gate)             # <<<<<<<<<<<<<<
  *         if conjugate_gate:
  *             gate = np.ascontiguousarray(gate.conjugate())
  */
-  __pyx_tuple__2 = PyTuple_Pack(2, __pyx_int_2, __pyx_int_2); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 98, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(2, __pyx_int_2, __pyx_int_2); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "dwave/gate/simulator/simulator.pyx":160
- *     num_qubits = circuit.num_qubits
- *     if num_qubits == 0:
- *         return np.empty(0, dtype=np.complex128)             # <<<<<<<<<<<<<<
- * 
- *     rng = np.random.default_rng(rng_seed)
- */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_int_0); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 160, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
-
   /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 945, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
+  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 945, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
 
   /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 951, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 951, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
 
   /* "dwave/gate/simulator/ops.pxd":384
  * ):
  * 
  *     norms = np.empty(2, dtype=np.float64)             # <<<<<<<<<<<<<<
  * 
  *     # the accumlative probability
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_int_2); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 384, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__10);
-  __Pyx_GIVEREF(__pyx_tuple__10);
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_int_2); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 384, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
 
   /* "dwave/gate/simulator/ops.pxd":465
  * 
  *     if p == 0.0:
  *         raise RuntimeError("cannot normalize state vector, norm too small")             # <<<<<<<<<<<<<<
  * 
  *     normalization_factor = 1 / np.sqrt(p)
  */
-  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_u_cannot_normalize_state_vector_no); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(2, 465, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__11);
-  __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_cannot_normalize_state_vector_no); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 465, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__10);
+  __Pyx_GIVEREF(__pyx_tuple__10);
 
   /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(3, 134, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__12);
-  __Pyx_GIVEREF(__pyx_tuple__12);
+  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(3, 134, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
 
   /* "View.MemoryView":137
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(3, 137, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__13);
-  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(3, 137, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__12);
+  __Pyx_GIVEREF(__pyx_tuple__12);
 
   /* "View.MemoryView":149
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(3, 149, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
+  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(3, 149, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
 
   /* "View.MemoryView":177
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(3, 177, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__15);
-  __Pyx_GIVEREF(__pyx_tuple__15);
+  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(3, 177, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__14);
+  __Pyx_GIVEREF(__pyx_tuple__14);
 
   /* "View.MemoryView":193
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(3, 193, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
+  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(3, 193, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__15);
+  __Pyx_GIVEREF(__pyx_tuple__15);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(3, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__17);
-  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(3, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__16);
+  __Pyx_GIVEREF(__pyx_tuple__16);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(3, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
+  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(3, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__17);
+  __Pyx_GIVEREF(__pyx_tuple__17);
 
   /* "View.MemoryView":420
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(3, 420, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__19);
-  __Pyx_GIVEREF(__pyx_tuple__19);
+  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(3, 420, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__18);
+  __Pyx_GIVEREF(__pyx_tuple__18);
 
   /* "View.MemoryView":497
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(3, 497, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__20);
-  __Pyx_GIVEREF(__pyx_tuple__20);
+  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(3, 497, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
 
   /* "View.MemoryView":522
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(3, 522, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__21);
-  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(3, 522, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__20);
+  __Pyx_GIVEREF(__pyx_tuple__20);
 
   /* "View.MemoryView":572
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(3, 572, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
-  __Pyx_GIVEREF(__pyx_tuple__22);
+  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(3, 572, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
 
   /* "View.MemoryView":579
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
-  __pyx_tuple__23 = PyTuple_New(1); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(3, 579, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__23);
+  __pyx_tuple__22 = PyTuple_New(1); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(3, 579, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__22);
   __Pyx_INCREF(__pyx_int_neg_1);
   __Pyx_GIVEREF(__pyx_int_neg_1);
-  PyTuple_SET_ITEM(__pyx_tuple__23, 0, __pyx_int_neg_1);
-  __Pyx_GIVEREF(__pyx_tuple__23);
+  PyTuple_SET_ITEM(__pyx_tuple__22, 0, __pyx_int_neg_1);
+  __Pyx_GIVEREF(__pyx_tuple__22);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(3, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
+  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(3, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(3, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__25);
-  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(3, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__24);
+  __Pyx_GIVEREF(__pyx_tuple__24);
 
   /* "View.MemoryView":684
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))             # <<<<<<<<<<<<<<
  *                 seen_ellipsis = True
  *             else:
  */
-  __pyx_slice__26 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__26)) __PYX_ERR(3, 684, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_slice__26);
-  __Pyx_GIVEREF(__pyx_slice__26);
+  __pyx_slice__25 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__25)) __PYX_ERR(3, 684, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_slice__25);
+  __Pyx_GIVEREF(__pyx_slice__25);
 
   /* "View.MemoryView":705
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(3, 705, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__27);
-  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(3, 705, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__26);
+  __Pyx_GIVEREF(__pyx_tuple__26);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(3, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__28);
-  __Pyx_GIVEREF(__pyx_tuple__28);
+  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(3, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
+  __Pyx_GIVEREF(__pyx_tuple__27);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__29 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(3, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__29);
-  __Pyx_GIVEREF(__pyx_tuple__29);
-  __pyx_tuple__31 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(3, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__31);
-  __Pyx_GIVEREF(__pyx_tuple__31);
+  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(3, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__28);
+  __Pyx_GIVEREF(__pyx_tuple__28);
+  __pyx_tuple__30 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(3, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__30);
+  __Pyx_GIVEREF(__pyx_tuple__30);
 
-  /* "dwave/gate/simulator/simulator.pyx":44
+  /* "dwave/gate/simulator/simulator.pyx":45
  * 
  * 
  * def apply_instruction(             # <<<<<<<<<<<<<<
  *     num_qubits: int,
  *     state: np.ndarray,
  */
-  __pyx_tuple__33 = PyTuple_Pack(14, __pyx_n_s_num_qubits, __pyx_n_s_state, __pyx_n_s_op, __pyx_n_s_targets, __pyx_n_s_little_endian, __pyx_n_s_rng, __pyx_n_s_conjugate_gate, __pyx_n_s_gate, __pyx_n_s_target0, __pyx_n_s_target1, __pyx_n_s_control, __pyx_n_s_target, __pyx_n_s_control0, __pyx_n_s_control1); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 44, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__33);
-  __Pyx_GIVEREF(__pyx_tuple__33);
-  __pyx_codeobj_ = (PyObject*)__Pyx_PyCode_New(7, 0, 14, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_dwave_gate_simulator_simulator_p, __pyx_n_s_apply_instruction, 44, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj_)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_tuple__32 = PyTuple_Pack(14, __pyx_n_s_num_qubits, __pyx_n_s_state, __pyx_n_s_op, __pyx_n_s_targets, __pyx_n_s_little_endian, __pyx_n_s_rng, __pyx_n_s_conjugate_gate, __pyx_n_s_gate, __pyx_n_s_target0, __pyx_n_s_target1, __pyx_n_s_control, __pyx_n_s_target, __pyx_n_s_control0, __pyx_n_s_control1); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__32);
+  __Pyx_GIVEREF(__pyx_tuple__32);
+  __pyx_codeobj_ = (PyObject*)__Pyx_PyCode_New(7, 0, 14, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_dwave_gate_simulator_simulator_p, __pyx_n_s_apply_instruction, 45, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj_)) __PYX_ERR(0, 45, __pyx_L1_error)
 
-  /* "dwave/gate/simulator/simulator.pyx":133
+  /* "dwave/gate/simulator/simulator.pyx":134
  * 
  * 
  * def simulate(             # <<<<<<<<<<<<<<
  *     circuit: Circuit,
  *     mixed_state: bool = False,
  */
-  __pyx_tuple__34 = PyTuple_Pack(10, __pyx_n_s_circuit, __pyx_n_s_mixed_state, __pyx_n_s_little_endian, __pyx_n_s_rng_seed, __pyx_n_s_num_qubits, __pyx_n_s_rng, __pyx_n_s_state, __pyx_n_s_op, __pyx_n_s_targets, __pyx_n_s_qb); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_tuple__33 = PyTuple_Pack(10, __pyx_n_s_circuit, __pyx_n_s_mixed_state, __pyx_n_s_little_endian, __pyx_n_s_rng_seed, __pyx_n_s_num_qubits, __pyx_n_s_rng, __pyx_n_s_state, __pyx_n_s_op, __pyx_n_s_targets, __pyx_n_s_qb); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 134, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__33);
+  __Pyx_GIVEREF(__pyx_tuple__33);
+  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(4, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_dwave_gate_simulator_simulator_p, __pyx_n_s_simulate, 134, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 134, __pyx_L1_error)
+
+  /* "dwave/gate/simulator/simulator.pyx":177
+ * 
+ * 
+ * def sample_qubit(             # <<<<<<<<<<<<<<
+ *     qubit: int,
+ *     state: np.typing.NDArray,
+ */
+  __pyx_tuple__34 = PyTuple_Pack(6, __pyx_n_s_qubit, __pyx_n_s_state, __pyx_n_s_rng, __pyx_n_s_collapse_state, __pyx_n_s_little_endian, __pyx_n_s_num_qubits); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(0, 177, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__34);
   __Pyx_GIVEREF(__pyx_tuple__34);
-  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(4, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_dwave_gate_simulator_simulator_p, __pyx_n_s_simulate, 133, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(5, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_dwave_gate_simulator_simulator_p, __pyx_n_s_sample_qubit, 177, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 177, __pyx_L1_error)
 
-  /* "dwave/gate/simulator/simulator.pyx":177
+  /* "dwave/gate/simulator/simulator.pyx":209
  * 
  * 
  * def _measure(op, state, targets, rng):             # <<<<<<<<<<<<<<
  *     op._measured_state = state.copy()
  * 
  */
-  __pyx_tuple__35 = PyTuple_Pack(7, __pyx_n_s_op, __pyx_n_s_state, __pyx_n_s_targets, __pyx_n_s_rng, __pyx_n_s_idx, __pyx_n_s_t, __pyx_n_s_m); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(0, 177, __pyx_L1_error)
+  __pyx_tuple__35 = PyTuple_Pack(7, __pyx_n_s_op, __pyx_n_s_state, __pyx_n_s_targets, __pyx_n_s_rng, __pyx_n_s_idx, __pyx_n_s_t, __pyx_n_s_m); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(0, 209, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__35);
   __Pyx_GIVEREF(__pyx_tuple__35);
-  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(4, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_dwave_gate_simulator_simulator_p, __pyx_n_s_measure, 177, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 177, __pyx_L1_error)
+  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(4, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_dwave_gate_simulator_simulator_p, __pyx_n_s_measure, 209, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 209, __pyx_L1_error)
 
-  /* "dwave/gate/simulator/simulator.pyx":191
- * 
- * 
- * def _sample(             # <<<<<<<<<<<<<<
- *     qubit: int,
- *     state: np.typing.NDArray,
- */
-  __pyx_tuple__36 = PyTuple_Pack(6, __pyx_n_s_qubit, __pyx_n_s_state, __pyx_n_s_rng, __pyx_n_s_collapse_state, __pyx_n_s_little_endian, __pyx_n_s_num_qubits); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(0, 191, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__36);
-  __Pyx_GIVEREF(__pyx_tuple__36);
-  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(5, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__36, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_dwave_gate_simulator_simulator_p, __pyx_n_s_sample, 191, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 191, __pyx_L1_error)
-
-  /* "dwave/gate/simulator/simulator.pyx":210
+  /* "dwave/gate/simulator/simulator.pyx":223
  * 
  * 
  * def _simulate_circuit_density_matrix(             # <<<<<<<<<<<<<<
  *     circuit: Circuit,
  *     rng: np.random.Generator,
  */
-  __pyx_tuple__37 = PyTuple_Pack(12, __pyx_n_s_circuit, __pyx_n_s_rng, __pyx_n_s_little_endian, __pyx_n_s_num_qubits, __pyx_n_s_num_virtual_qubits, __pyx_n_s_state, __pyx_n_s_op, __pyx_n_s_targets, __pyx_n_s_virtual_targets, __pyx_n_s_density_matrix, __pyx_n_s_qb, __pyx_n_s_t); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(0, 210, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__37);
-  __Pyx_GIVEREF(__pyx_tuple__37);
-  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(3, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__37, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_dwave_gate_simulator_simulator_p, __pyx_n_s_simulate_circuit_density_matrix, 210, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 210, __pyx_L1_error)
+  __pyx_tuple__36 = PyTuple_Pack(12, __pyx_n_s_circuit, __pyx_n_s_rng, __pyx_n_s_little_endian, __pyx_n_s_num_qubits, __pyx_n_s_num_virtual_qubits, __pyx_n_s_state, __pyx_n_s_op, __pyx_n_s_targets, __pyx_n_s_virtual_targets, __pyx_n_s_density_matrix, __pyx_n_s_qb, __pyx_n_s_t); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(0, 223, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__36);
+  __Pyx_GIVEREF(__pyx_tuple__36);
+  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(3, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__36, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_dwave_gate_simulator_simulator_p, __pyx_n_s_simulate_circuit_density_matrix, 223, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 223, __pyx_L1_error)
 
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_tuple__38 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(3, 287, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__38);
-  __Pyx_GIVEREF(__pyx_tuple__38);
+  __pyx_tuple__37 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(3, 287, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__37);
+  __Pyx_GIVEREF(__pyx_tuple__37);
 
   /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_tuple__39 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(3, 288, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__39);
-  __Pyx_GIVEREF(__pyx_tuple__39);
+  __pyx_tuple__38 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(3, 288, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__38);
+  __Pyx_GIVEREF(__pyx_tuple__38);
 
   /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__40 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(3, 289, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__40);
-  __Pyx_GIVEREF(__pyx_tuple__40);
+  __pyx_tuple__39 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(3, 289, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__39);
+  __Pyx_GIVEREF(__pyx_tuple__39);
 
   /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_tuple__41 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(3, 292, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__41);
-  __Pyx_GIVEREF(__pyx_tuple__41);
+  __pyx_tuple__40 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(3, 292, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__40);
+  __Pyx_GIVEREF(__pyx_tuple__40);
 
   /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__42 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__42)) __PYX_ERR(3, 293, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__42);
-  __Pyx_GIVEREF(__pyx_tuple__42);
+  __pyx_tuple__41 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(3, 293, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__41);
+  __Pyx_GIVEREF(__pyx_tuple__41);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__43 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(3, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__43);
-  __Pyx_GIVEREF(__pyx_tuple__43);
-  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(3, 1, __pyx_L1_error)
+  __pyx_tuple__42 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__42)) __PYX_ERR(3, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__42);
+  __Pyx_GIVEREF(__pyx_tuple__42);
+  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__42, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(3, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -27912,204 +27903,207 @@
   __Pyx_TraceCall("__Pyx_PyMODINIT_FUNC PyInit_simulator(void)", __pyx_f[0], 1, 0, __PYX_ERR(0, 1, __pyx_L1_error));
 
   /* "dwave/gate/simulator/simulator.pyx":19
  * #    limitations under the License.
  * 
  * __all__ = [             # <<<<<<<<<<<<<<
  *     "simulate",
- * ]
+ *     "sample_qubit",
  */
   __Pyx_TraceLine(19,0,__PYX_ERR(0, 19, __pyx_L1_error))
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_u_simulate);
   __Pyx_GIVEREF(__pyx_n_u_simulate);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_u_simulate);
+  __Pyx_INCREF(__pyx_n_u_sample_qubit);
+  __Pyx_GIVEREF(__pyx_n_u_sample_qubit);
+  PyList_SET_ITEM(__pyx_t_1, 1, __pyx_n_u_sample_qubit);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_all, __pyx_t_1) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "dwave/gate/simulator/simulator.pyx":23
+  /* "dwave/gate/simulator/simulator.pyx":24
  * ]
  * 
  * import random             # <<<<<<<<<<<<<<
  * import warnings
  * from typing import List, Optional
  */
-  __Pyx_TraceLine(23,0,__PYX_ERR(0, 23, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_random, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __Pyx_TraceLine(24,0,__PYX_ERR(0, 24, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_random, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random, __pyx_t_1) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random, __pyx_t_1) < 0) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "dwave/gate/simulator/simulator.pyx":24
+  /* "dwave/gate/simulator/simulator.pyx":25
  * 
  * import random
  * import warnings             # <<<<<<<<<<<<<<
  * from typing import List, Optional
  * 
  */
-  __Pyx_TraceLine(24,0,__PYX_ERR(0, 24, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_warnings, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __Pyx_TraceLine(25,0,__PYX_ERR(0, 25, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_warnings, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_warnings, __pyx_t_1) < 0) __PYX_ERR(0, 24, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_warnings, __pyx_t_1) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "dwave/gate/simulator/simulator.pyx":25
+  /* "dwave/gate/simulator/simulator.pyx":26
  * import random
  * import warnings
  * from typing import List, Optional             # <<<<<<<<<<<<<<
  * 
  * import numpy as np
  */
-  __Pyx_TraceLine(25,0,__PYX_ERR(0, 25, __pyx_L1_error))
-  __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __Pyx_TraceLine(26,0,__PYX_ERR(0, 26, __pyx_L1_error))
+  __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_List);
   __Pyx_GIVEREF(__pyx_n_s_List);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_List);
   __Pyx_INCREF(__pyx_n_s_Optional);
   __Pyx_GIVEREF(__pyx_n_s_Optional);
   PyList_SET_ITEM(__pyx_t_1, 1, __pyx_n_s_Optional);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_typing, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_typing, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_List); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_List); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_List, __pyx_t_1) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_List, __pyx_t_1) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Optional); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Optional); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Optional, __pyx_t_1) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Optional, __pyx_t_1) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "dwave/gate/simulator/simulator.pyx":27
+  /* "dwave/gate/simulator/simulator.pyx":28
  * from typing import List, Optional
  * 
  * import numpy as np             # <<<<<<<<<<<<<<
  * 
  * cimport numpy as np
  */
-  __Pyx_TraceLine(27,0,__PYX_ERR(0, 27, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 27, __pyx_L1_error)
+  __Pyx_TraceLine(28,0,__PYX_ERR(0, 28, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_2) < 0) __PYX_ERR(0, 27, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_2) < 0) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "dwave/gate/simulator/simulator.pyx":31
+  /* "dwave/gate/simulator/simulator.pyx":32
  * cimport numpy as np
  * 
  * import dwave.gate.operations as ops             # <<<<<<<<<<<<<<
  * from dwave.gate.circuit import Circuit, CircuitError
  * 
  */
-  __Pyx_TraceLine(31,0,__PYX_ERR(0, 31, __pyx_L1_error))
-  __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __Pyx_TraceLine(32,0,__PYX_ERR(0, 32, __pyx_L1_error))
+  __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_INCREF(__pyx_n_s__32);
-  __Pyx_GIVEREF(__pyx_n_s__32);
-  PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s__32);
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_dwave_gate_operations, __pyx_t_2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __Pyx_INCREF(__pyx_n_s__31);
+  __Pyx_GIVEREF(__pyx_n_s__31);
+  PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s__31);
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_dwave_gate_operations, __pyx_t_2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ops, __pyx_t_1) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ops, __pyx_t_1) < 0) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "dwave/gate/simulator/simulator.pyx":32
+  /* "dwave/gate/simulator/simulator.pyx":33
  * 
  * import dwave.gate.operations as ops
  * from dwave.gate.circuit import Circuit, CircuitError             # <<<<<<<<<<<<<<
  * 
  * from dwave.gate.simulator.ops cimport (
  */
-  __Pyx_TraceLine(32,0,__PYX_ERR(0, 32, __pyx_L1_error))
-  __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __Pyx_TraceLine(33,0,__PYX_ERR(0, 33, __pyx_L1_error))
+  __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_Circuit);
   __Pyx_GIVEREF(__pyx_n_s_Circuit);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_Circuit);
   __Pyx_INCREF(__pyx_n_s_CircuitError);
   __Pyx_GIVEREF(__pyx_n_s_CircuitError);
   PyList_SET_ITEM(__pyx_t_1, 1, __pyx_n_s_CircuitError);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_dwave_gate_circuit, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_dwave_gate_circuit, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Circuit); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Circuit); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Circuit, __pyx_t_1) < 0) __PYX_ERR(0, 32, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Circuit, __pyx_t_1) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_CircuitError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_CircuitError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_CircuitError, __pyx_t_1) < 0) __PYX_ERR(0, 32, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_CircuitError, __pyx_t_1) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "dwave/gate/simulator/simulator.pyx":44
+  /* "dwave/gate/simulator/simulator.pyx":45
  * 
  * 
  * def apply_instruction(             # <<<<<<<<<<<<<<
  *     num_qubits: int,
  *     state: np.ndarray,
  */
-  __Pyx_TraceLine(44,0,__PYX_ERR(0, 44, __pyx_L1_error))
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5dwave_4gate_9simulator_9simulator_1apply_instruction, NULL, __pyx_n_s_dwave_gate_simulator_simulator); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __Pyx_TraceLine(45,0,__PYX_ERR(0, 45, __pyx_L1_error))
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5dwave_4gate_9simulator_9simulator_1apply_instruction, NULL, __pyx_n_s_dwave_gate_simulator_simulator); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_apply_instruction, __pyx_t_2) < 0) __PYX_ERR(0, 44, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_apply_instruction, __pyx_t_2) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "dwave/gate/simulator/simulator.pyx":133
+  /* "dwave/gate/simulator/simulator.pyx":134
  * 
  * 
  * def simulate(             # <<<<<<<<<<<<<<
  *     circuit: Circuit,
  *     mixed_state: bool = False,
  */
-  __Pyx_TraceLine(133,0,__PYX_ERR(0, 133, __pyx_L1_error))
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5dwave_4gate_9simulator_9simulator_3simulate, NULL, __pyx_n_s_dwave_gate_simulator_simulator); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __Pyx_TraceLine(134,0,__PYX_ERR(0, 134, __pyx_L1_error))
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5dwave_4gate_9simulator_9simulator_3simulate, NULL, __pyx_n_s_dwave_gate_simulator_simulator); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_simulate, __pyx_t_2) < 0) __PYX_ERR(0, 133, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_simulate, __pyx_t_2) < 0) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "dwave/gate/simulator/simulator.pyx":177
  * 
  * 
- * def _measure(op, state, targets, rng):             # <<<<<<<<<<<<<<
- *     op._measured_state = state.copy()
- * 
+ * def sample_qubit(             # <<<<<<<<<<<<<<
+ *     qubit: int,
+ *     state: np.typing.NDArray,
  */
   __Pyx_TraceLine(177,0,__PYX_ERR(0, 177, __pyx_L1_error))
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5dwave_4gate_9simulator_9simulator_5_measure, NULL, __pyx_n_s_dwave_gate_simulator_simulator); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 177, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5dwave_4gate_9simulator_9simulator_5sample_qubit, NULL, __pyx_n_s_dwave_gate_simulator_simulator); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 177, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_measure, __pyx_t_2) < 0) __PYX_ERR(0, 177, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_sample_qubit, __pyx_t_2) < 0) __PYX_ERR(0, 177, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "dwave/gate/simulator/simulator.pyx":191
+  /* "dwave/gate/simulator/simulator.pyx":209
  * 
  * 
- * def _sample(             # <<<<<<<<<<<<<<
- *     qubit: int,
- *     state: np.typing.NDArray,
+ * def _measure(op, state, targets, rng):             # <<<<<<<<<<<<<<
+ *     op._measured_state = state.copy()
+ * 
  */
-  __Pyx_TraceLine(191,0,__PYX_ERR(0, 191, __pyx_L1_error))
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5dwave_4gate_9simulator_9simulator_7_sample, NULL, __pyx_n_s_dwave_gate_simulator_simulator); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
+  __Pyx_TraceLine(209,0,__PYX_ERR(0, 209, __pyx_L1_error))
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5dwave_4gate_9simulator_9simulator_7_measure, NULL, __pyx_n_s_dwave_gate_simulator_simulator); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 209, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_sample, __pyx_t_2) < 0) __PYX_ERR(0, 191, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_measure, __pyx_t_2) < 0) __PYX_ERR(0, 209, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "dwave/gate/simulator/simulator.pyx":210
+  /* "dwave/gate/simulator/simulator.pyx":223
  * 
  * 
  * def _simulate_circuit_density_matrix(             # <<<<<<<<<<<<<<
  *     circuit: Circuit,
  *     rng: np.random.Generator,
  */
-  __Pyx_TraceLine(210,0,__PYX_ERR(0, 210, __pyx_L1_error))
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5dwave_4gate_9simulator_9simulator_9_simulate_circuit_density_matrix, NULL, __pyx_n_s_dwave_gate_simulator_simulator); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 210, __pyx_L1_error)
+  __Pyx_TraceLine(223,0,__PYX_ERR(0, 223, __pyx_L1_error))
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5dwave_4gate_9simulator_9simulator_9_simulate_circuit_density_matrix, NULL, __pyx_n_s_dwave_gate_simulator_simulator); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_simulate_circuit_density_matrix, __pyx_t_2) < 0) __PYX_ERR(0, 210, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_simulate_circuit_density_matrix, __pyx_t_2) < 0) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "dwave/gate/simulator/simulator.pyx":1
  * # distutils: language = c++             # <<<<<<<<<<<<<<
  * # cython: language_level=3
  * # cython: linetrace=True
  */
@@ -28397,75 +28391,75 @@
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
   __Pyx_TraceLine(287,0,__PYX_ERR(3, 287, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__38, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 287, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__37, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_XGOTREF(generic);
   __Pyx_DECREF_SET(generic, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
   __Pyx_TraceLine(288,0,__PYX_ERR(3, 288, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__39, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 288, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__38, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 288, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_XGOTREF(strided);
   __Pyx_DECREF_SET(strided, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_TraceLine(289,0,__PYX_ERR(3, 289, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__40, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 289, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__39, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_XGOTREF(indirect);
   __Pyx_DECREF_SET(indirect, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
   __Pyx_TraceLine(292,0,__PYX_ERR(3, 292, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__41, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 292, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__40, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 292, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_XGOTREF(contiguous);
   __Pyx_DECREF_SET(contiguous, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_TraceLine(293,0,__PYX_ERR(3, 293, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__42, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 293, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__41, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_XGOTREF(indirect_contiguous);
   __Pyx_DECREF_SET(indirect_contiguous, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "View.MemoryView":299
```

### Comparing `dwave-gate-0.2.0/dwave/gate/simulator/simulator.pyx` & `dwave-gate-0.2.1/dwave/gate/simulator/simulator.pyx`

 * *Files 11% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 __all__ = [
     "simulate",
+    "sample_qubit",
 ]
 
 import random
 import warnings
 from typing import List, Optional
 
 import numpy as np
@@ -131,86 +132,98 @@
 
 
 def simulate(
     circuit: Circuit,
     mixed_state: bool = False,
     little_endian: bool = False,
     rng_seed: Optional[int] = None,
-) -> np.typing.NDArray:
-    """Simulate the given circuit with either a state vector or density matrix
-    simulation.
+) -> None:
+    """Simulate the given circuit with either a state vector or density matrix simulation.
+
+    The resulting state is stored in the circuit object, together with the measured value in the
+    classical register.
 
     Args:
         circuit: The circuit to simulate.
 
         mixed_state:
             If true, use the full density matrix method to simulate the circuit.
             Otherwise, simulate using the state vector method.
 
         little_endian:
             If true, return the state vector using little-endian indexing for
             the qubits. Otherwise use big-endian.
 
-    Returns:
-        The resulting state vector or density matrix.
-
     """
 
     num_qubits = circuit.num_qubits
     if num_qubits == 0:
-        return np.empty(0, dtype=np.complex128)
+        return
 
     rng = np.random.default_rng(rng_seed)
 
     if mixed_state:
-        return _simulate_circuit_density_matrix(circuit, rng)
-
-    state = np.zeros(1 << num_qubits, dtype=np.complex128)
-    state[0] = 1
-
-    for op in circuit.circuit:
-        targets = [circuit.qubits.index(qb) for qb in op.qubits]
-        apply_instruction(num_qubits, state, op, targets, little_endian, rng)
-
-    return state
-
-
-def _measure(op, state, targets, rng):
-    op._measured_state = state.copy()
-
-    for idx, t in enumerate(targets):
-        m = _sample(t, state, rng)
+        state = _simulate_circuit_density_matrix(circuit, rng)
+    else:
+        state = np.zeros(1 << num_qubits, dtype=np.complex128)
+        state[0] = 1
 
-        try:
-            op.bits[idx].set(m, force=True)
-        except (IndexError, TypeError):
-            warnings.warn("Measurements not stored in the classical register.")
+        for op in circuit.circuit:
+            targets = [circuit.qubits.index(qb) for qb in op.qubits]
+            apply_instruction(num_qubits, state, op, targets, little_endian, rng)
 
-        op._measured_qubit_indices.append(t)
+    circuit.set_state(state, force=True)
 
 
-def _sample(
+def sample_qubit(
     qubit: int,
     state: np.typing.NDArray,
     rng: np.random.Generator,
     collapse_state: bool = True,
     little_endian: bool = False,
 ) -> int:
+    """Sample a single qubit.
+
+    Args:
+        qubit: The qubit index that is measured.
+        state: The state to sample from.
+        rng: Random number generator to use for measuring in the computational basis.
+        collapse_state: Whether to collapse the state after measuring.
+        little_endian: If true, return the state vector using little-endian indexing for
+            the qubits. Otherwise use big-endian.
+
+    Returns:
+        int: The measurement sample (0 or 1).
+    """
     cdef int num_qubits = round(np.log2(state.shape[0]))
 
     return measurement_computational_basis(
         num_qubits,
         state,
         qubit,
         rng,
         little_endian=little_endian,
         apply_operator=collapse_state,
     )
 
 
+def _measure(op, state, targets, rng):
+    op._measured_state = state.copy()
+
+    for idx, t in enumerate(targets):
+        m = sample_qubit(t, state, rng)
+
+        try:
+            op.bits[idx].set(m, force=True)
+        except (IndexError, TypeError):
+            warnings.warn("Measurements not stored in the classical register.")
+
+        op._measured_qubit_indices.append(t)
+
+
 def _simulate_circuit_density_matrix(
     circuit: Circuit,
     rng: np.random.Generator,
     little_endian: bool = False,
 ) -> np.typing.NDArray:
 
     num_qubits = circuit.num_qubits
```

### Comparing `dwave-gate-0.2.0/dwave/gate/tools/__init__.py` & `dwave-gate-0.2.1/dwave/gate/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.0/dwave/gate/tools/counters.py` & `dwave-gate-0.2.1/dwave/gate/tools/counters.py`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.0/dwave/gate/tools/unitary.py` & `dwave-gate-0.2.1/dwave/gate/tools/unitary.py`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.0/dwave/gate/utils.py` & `dwave-gate-0.2.1/dwave/gate/utils.py`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.0/dwave_gate.egg-info/PKG-INFO` & `dwave-gate-0.2.1/dwave_gate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwave-gate
-Version: 0.2.0
+Version: 0.2.1
 Summary: Gate model library.
 Home-page: https://github.com/dwavesystems/dwave-gate
 Author: D-Wave Systems Inc.
 Author-email: tools@dwavesys.com
 License: UNKNOWN
 Download-URL: https://github.com/dwavesystems/dwave-gate/releases
 Platform: UNKNOWN
```

### Comparing `dwave-gate-0.2.0/dwave_gate.egg-info/SOURCES.txt` & `dwave-gate-0.2.1/dwave_gate.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 dwave/gate/simulator/operation_generation.py
 dwave/gate/simulator/ops.h
 dwave/gate/simulator/ops.pxd
 dwave/gate/simulator/simulator.cpp
 dwave/gate/simulator/simulator.pyx
 dwave/gate/tools/__init__.py
 dwave/gate/tools/counters.py
-dwave/gate/tools/samples.py
 dwave/gate/tools/unitary.py
 dwave_gate.egg-info/PKG-INFO
 dwave_gate.egg-info/SOURCES.txt
 dwave_gate.egg-info/dependency_links.txt
 dwave_gate.egg-info/not-zip-safe
 dwave_gate.egg-info/requires.txt
 dwave_gate.egg-info/top_level.txt
```

### Comparing `dwave-gate-0.2.0/pyproject.toml` & `dwave-gate-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.0/setup.cfg` & `dwave-gate-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.0/setup.py` & `dwave-gate-0.2.1/setup.py`

 * *Files identical despite different names*

