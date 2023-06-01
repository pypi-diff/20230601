# Comparing `tmp/meow-sim-0.3.4.tar.gz` & `tmp/meow-sim-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meow-sim-0.3.4.tar", last modified: Wed May 24 22:47:55 2023, max compression
+gzip compressed data, was "meow-sim-0.3.5.tar", last modified: Thu Jun  1 00:57:41 2023, max compression
```

## Comparing `meow-sim-0.3.4.tar` & `meow-sim-0.3.5.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:47:55.135574 meow-sim-0.3.4/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-05-24 22:47:50.000000 meow-sim-0.3.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3178 2023-05-24 22:47:55.135574 meow-sim-0.3.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2060 2023-05-24 22:47:50.000000 meow-sim-0.3.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:47:55.131574 meow-sim-0.3.4/meow/
--rw-r--r--   0 root         (0) root         (0)     1414 2023-05-24 22:47:50.000000 meow-sim-0.3.4/meow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:47:55.131574 meow-sim-0.3.4/meow/assets/
--rw-r--r--   0 root         (0) root         (0)    10307 2023-05-24 22:47:50.000000 meow-sim-0.3.4/meow/assets/silicon.csv
--rw-r--r--   0 root         (0) root         (0)     8535 2023-05-24 22:47:50.000000 meow-sim-0.3.4/meow/assets/silicon_oxide.csv
--rw-r--r--   0 root         (0) root         (0)     8007 2023-05-24 22:47:50.000000 meow-sim-0.3.4/meow/base_model.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-05-24 22:47:50.000000 meow-sim-0.3.4/meow/cache.py
--rw-r--r--   0 root         (0) root         (0)     4818 2023-05-24 22:47:50.000000 meow-sim-0.3.4/meow/cell.py
--rw-r--r--   0 root         (0) root         (0)     2783 2023-05-24 22:47:50.000000 meow-sim-0.3.4/meow/cross_section.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:47:55.135574 meow-sim-0.3.4/meow/eme/
--rw-r--r--   0 root         (0) root         (0)      623 2023-05-24 22:47:50.000000 meow-sim-0.3.4/meow/eme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4600 2023-05-24 22:47:50.000000 meow-sim-0.3.4/meow/eme/common.py
--rw-r--r--   0 root         (0) root         (0)     3316 2023-05-24 22:47:50.000000 meow-sim-0.3.4/meow/eme/sax.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-05-24 22:47:50.000000 meow-sim-0.3.4/meow/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:47:55.135574 meow-sim-0.3.4/meow/fde/
--rw-r--r--   0 root         (0) root         (0)      324 2023-05-24 22:47:50.000000 meow-sim-0.3.4/meow/fde/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3440 2023-05-24 22:47:50.000000 meow-sim-0.3.4/meow/fde/lumerical.py
--rw-r--r--   0 root         (0) root         (0)     2996 2023-05-24 22:47:50.000000 meow-sim-0.3.4/meow/fde/tidy3d.py
--rw-r--r--   0 root         (0) root         (0)     2052 2023-05-24 22:47:50.000000 meow-sim-0.3.4/meow/gds_structures.py
--rw-r--r--   0 root         (0) root         (0)    10197 2023-05-24 22:47:50.000000 meow-sim-0.3.4/meow/geometries.py
--rw-r--r--   0 root         (0) root         (0)      944 2023-05-24 22:47:50.000000 meow-sim-0.3.4/meow/integrate.py
--rw-r--r--   0 root         (0) root         (0)    10785 2023-05-24 22:47:50.000000 meow-sim-0.3.4/meow/materials.py
--rw-r--r--   0 root         (0) root         (0)     3564 2023-05-24 22:47:50.000000 meow-sim-0.3.4/meow/mesh.py
--rw-r--r--   0 root         (0) root         (0)     9814 2023-05-24 22:47:50.000000 meow-sim-0.3.4/meow/mode.py
--rw-r--r--   0 root         (0) root         (0)     1850 2023-05-24 22:47:50.000000 meow-sim-0.3.4/meow/structures.py
--rw-r--r--   0 root         (0) root         (0)     2787 2023-05-24 22:47:50.000000 meow-sim-0.3.4/meow/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:47:55.135574 meow-sim-0.3.4/meow_sim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3178 2023-05-24 22:47:55.000000 meow-sim-0.3.4/meow_sim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      657 2023-05-24 22:47:55.000000 meow-sim-0.3.4/meow_sim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 22:47:55.000000 meow-sim-0.3.4/meow_sim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      395 2023-05-24 22:47:55.000000 meow-sim-0.3.4/meow_sim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-24 22:47:55.000000 meow-sim-0.3.4/meow_sim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1890 2023-05-24 22:47:50.000000 meow-sim-0.3.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 22:47:55.135574 meow-sim-0.3.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:47:55.135574 meow-sim-0.3.4/tests/
--rw-r--r--   0 root         (0) root         (0)     4009 2023-05-24 22:47:50.000000 meow-sim-0.3.4/tests/test_deserialization.py
--rw-r--r--   0 root         (0) root         (0)     1322 2023-05-24 22:47:50.000000 meow-sim-0.3.4/tests/test_nbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 00:57:41.199327 meow-sim-0.3.5/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-06-01 00:57:36.000000 meow-sim-0.3.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3178 2023-06-01 00:57:41.199327 meow-sim-0.3.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-06-01 00:57:36.000000 meow-sim-0.3.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 00:57:41.191327 meow-sim-0.3.5/meow/
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 00:57:41.191327 meow-sim-0.3.5/meow/assets/
+-rw-r--r--   0 root         (0) root         (0)    10307 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/assets/silicon.csv
+-rw-r--r--   0 root         (0) root         (0)     8535 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/assets/silicon_oxide.csv
+-rw-r--r--   0 root         (0) root         (0)     8007 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4818 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/cell.py
+-rw-r--r--   0 root         (0) root         (0)     2783 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/cross_section.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 00:57:41.191327 meow-sim-0.3.5/meow/eme/
+-rw-r--r--   0 root         (0) root         (0)      623 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/eme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4684 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/eme/common.py
+-rw-r--r--   0 root         (0) root         (0)     3667 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/eme/sax.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 00:57:41.195327 meow-sim-0.3.5/meow/fde/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/fde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3440 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/fde/lumerical.py
+-rw-r--r--   0 root         (0) root         (0)     3005 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/fde/tidy3d.py
+-rw-r--r--   0 root         (0) root         (0)     2052 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/gds_structures.py
+-rw-r--r--   0 root         (0) root         (0)    10197 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/geometries.py
+-rw-r--r--   0 root         (0) root         (0)      944 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/integrate.py
+-rw-r--r--   0 root         (0) root         (0)    10785 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/materials.py
+-rw-r--r--   0 root         (0) root         (0)     3564 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/mesh.py
+-rw-r--r--   0 root         (0) root         (0)    11409 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/mode.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/structures.py
+-rw-r--r--   0 root         (0) root         (0)     2787 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 00:57:41.199327 meow-sim-0.3.5/meow_sim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3178 2023-06-01 00:57:41.000000 meow-sim-0.3.5/meow_sim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-06-01 00:57:41.000000 meow-sim-0.3.5/meow_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 00:57:41.000000 meow-sim-0.3.5/meow_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      395 2023-06-01 00:57:41.000000 meow-sim-0.3.5/meow_sim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-01 00:57:41.000000 meow-sim-0.3.5/meow_sim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1890 2023-06-01 00:57:36.000000 meow-sim-0.3.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 00:57:41.199327 meow-sim-0.3.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 00:57:41.199327 meow-sim-0.3.5/tests/
+-rw-r--r--   0 root         (0) root         (0)     4009 2023-06-01 00:57:36.000000 meow-sim-0.3.5/tests/test_deserialization.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2023-06-01 00:57:36.000000 meow-sim-0.3.5/tests/test_mode_operators.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-06-01 00:57:36.000000 meow-sim-0.3.5/tests/test_nbs.py
```

### Comparing `meow-sim-0.3.4/LICENSE` & `meow-sim-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.4/PKG-INFO` & `meow-sim-0.3.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.3.4
+Version: 0.3.5
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.3.4/README.md` & `meow-sim-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.4/meow/__init__.py` & `meow-sim-0.3.5/meow/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ MEOW: Modeling of Eigenmodes and Overlaps in Waveguides """
 
 __author__ = "Floris Laporte"
-__version__ = "0.3.4"
+__version__ = "0.3.5"
 
 import warnings
 
 # Silence Excessive Logging...
 
 try:
     from loguru import logger
```

### Comparing `meow-sim-0.3.4/meow/assets/silicon.csv` & `meow-sim-0.3.5/meow/assets/silicon.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.4/meow/assets/silicon_oxide.csv` & `meow-sim-0.3.5/meow/assets/silicon_oxide.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.4/meow/base_model.py` & `meow-sim-0.3.5/meow/base_model.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.4/meow/cache.py` & `meow-sim-0.3.5/meow/cache.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.4/meow/cell.py` & `meow-sim-0.3.5/meow/cell.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.4/meow/cross_section.py` & `meow-sim-0.3.5/meow/cross_section.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.4/meow/eme/__init__.py` & `meow-sim-0.3.5/meow/eme/__init__.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.4/meow/eme/common.py` & `meow-sim-0.3.5/meow/eme/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,28 +37,28 @@
     # yet another alternative phase correction (probably worth testing this out too)
     # O_LR = O_LR@np.diag(np.exp(-1j*np.angle(np.diag(O_LR))))
     # O_RL = O_RL@np.diag(np.exp(-1j*np.angle(np.diag(O_RL))))
 
     # transmission L->R
     LHS = O_LR + O_RL.T
     RHS = np.diag(2 * O_LL)
-    T_LR = np.linalg.solve(LHS, RHS)
-    U, t, V = np.linalg.svd(T_LR)
+    T_LR, _, _, _ = np.linalg.lstsq(LHS, RHS, rcond=None)
+    U, t, V = np.linalg.svd(T_LR, full_matrices=False)
 
     # HACK: we don't expect gain --> invert singular values that lead to gain
     # see: https://github.com/BYUCamachoLab/emepy/issues/12
     t = np.where(t > 1, 1 / t, t)
 
     T_LR = U @ np.diag(t) @ V
 
     # transmission R->L
     LHS = O_RL + O_LR.T
     RHS = np.diag(2 * O_RR)
-    T_RL = np.linalg.solve(LHS, RHS)
-    U, t, V = np.linalg.svd(T_RL)
+    T_RL, _, _, _ = np.linalg.lstsq(LHS, RHS, rcond=None)
+    U, t, V = np.linalg.svd(T_RL, full_matrices=False)
 
     # HACK: we don't expect gain --> invert singular values that lead to gain
     t = np.where(t > 1, 1 / t, t)
 
     T_RL = U @ np.diag(t) @ V
 
     # reflection
```

### Comparing `meow-sim-0.3.4/meow/environment.py` & `meow-sim-0.3.5/meow/environment.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.4/meow/fde/lumerical.py` & `meow-sim-0.3.5/meow/fde/lumerical.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.4/meow/fde/tidy3d.py` & `meow-sim-0.3.5/meow/fde/tidy3d.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import tidy3d
 from ..cross_section import CrossSection
 from ..mode import Mode, Modes, normalize_energy, zero_phase
 
 
 from packaging import version
 
+
 @validate_arguments
 def compute_modes_tidy3d(
     cs: CrossSection,
     num_modes: PositiveInt = 10,
     target_neff: Optional[PositiveFloat] = None,
 ) -> Modes:
     """compute ``Modes`` for a given ``FdeSpec`` (Tidy3D backend)
@@ -30,21 +31,22 @@
     """
 
     if num_modes < 1:
         raise ValueError("You need to request at least 1 mode.")
 
     bend_radius = None if cs.cell.mesh.bend_radius > 1e10 else cs.cell.mesh.bend_radius
     bend_axis = None if bend_radius is None else cs.cell.mesh.bend_axis
-    od = np.zeros_like(cs.nx) #off diagonal entry
+    od = np.zeros_like(cs.nx)  # off diagonal entry
     new_tidy3d = version.parse(tidy3d.__version__) >= version.parse("2.2.0")
     ((Ex, Ey, Ez), (Hx, Hy, Hz)), neffs = (
         x.squeeze()
         for x in _compute_modes(
-            eps_cross=[cs.nx**2, od, od, od, cs.ny**2, od, od, od, cs.nz**2] 
-                if new_tidy3d else [cs.nx**2, cs.ny**2, cs.nz**2], 
+            eps_cross=[cs.nx**2, od, od, od, cs.ny**2, od, od, od, cs.nz**2]
+            if new_tidy3d
+            else [cs.nx**2, cs.ny**2, cs.nz**2],
             coords=[cs.mesh.x, cs.mesh.y],
             freq=c / (cs.env.wl * 1e-6),
             mode_spec=SimpleNamespace(
                 num_modes=num_modes,
                 angle_theta=cs.cell.mesh.angle_theta,
                 angle_phi=cs.cell.mesh.angle_phi,
                 bend_radius=bend_radius,
```

### Comparing `meow-sim-0.3.4/meow/gds_structures.py` & `meow-sim-0.3.5/meow/gds_structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.4/meow/geometries.py` & `meow-sim-0.3.5/meow/geometries.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.4/meow/integrate.py` & `meow-sim-0.3.5/meow/integrate.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.4/meow/materials.py` & `meow-sim-0.3.5/meow/materials.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.4/meow/mesh.py` & `meow-sim-0.3.5/meow/mesh.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.4/meow/mode.py` & `meow-sim-0.3.5/meow/mode.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ An EigenMode """
 
 import pickle
 from itertools import product
 from typing import Any, List, Tuple
+import numbers
 
 import numpy as np
 from pydantic import Field, PrivateAttr
 from scipy.constants import epsilon_0 as eps0
 from scipy.constants import mu_0 as mu0
 from scipy.linalg import norm
 
@@ -189,14 +190,64 @@
             pickle.dump(self, file)
 
     @classmethod
     def load(cls, filename):
         with open(filename, "rb") as file:
             return pickle.load(file)
 
+    def __add__(self, other):
+        if not isinstance(other, Mode):
+            raise TypeError(
+                f"unsupported operand type(s) for +: 'Mode' and '{type(other).__name__}'"
+            )
+        new_mode = Mode(
+            neff=np.mean([self.neff, other.neff]),
+            cs=self.cs,
+            Ex=self.Ex + other.Ex,
+            Ey=self.Ey + other.Ey,
+            Ez=self.Ez + other.Ez,
+            Hx=self.Hx + other.Hx,
+            Hy=self.Hy + other.Hy,
+            Hz=self.Hz + other.Hz,
+        )
+        return new_mode
+
+    def __mul__(self, other):
+        if not isinstance(other, numbers.Number):
+            raise TypeError(
+                f"unsupported operand type(s) for *: 'Mode' and '{type(other).__name__}'"
+            )
+        new_mode = Mode(
+            neff=self.neff,
+            cs=self.cs,
+            Ex=self.Ex * other,
+            Ey=self.Ey * other,
+            Ez=self.Ez * other,
+            Hx=self.Hx * other,
+            Hy=self.Hy * other,
+            Hz=self.Hz * other,
+        )
+        return new_mode
+
+    __rmul__ = __mul__
+
+    def __truediv__(self, other):
+        if not isinstance(other, numbers.Number):
+            raise TypeError(
+                f"unsupported operand type(s) for /: 'Mode' and '{type(other).__name__}'"
+            )
+        return self * (1 / other)
+
+    def __sub__(self, other):
+        if not isinstance(other, Mode):
+            raise TypeError(
+                f"unsupported operand type(s) for -: 'Mode' and '{type(other).__name__}'"
+            )
+        return self + other * (-1)
+
 
 Modes = List[Mode]
 
 
 def zero_phase(mode: Mode) -> Mode:
     """normalize (zero out) the phase of a `Mode`"""
     e = np.abs(energy_density(mode))
```

### Comparing `meow-sim-0.3.4/meow/structures.py` & `meow-sim-0.3.5/meow/structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.4/meow/visualize.py` & `meow-sim-0.3.5/meow/visualize.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.4/meow_sim.egg-info/PKG-INFO` & `meow-sim-0.3.5/meow_sim.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.3.4
+Version: 0.3.5
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.3.4/meow_sim.egg-info/SOURCES.txt` & `meow-sim-0.3.5/meow_sim.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -25,8 +25,9 @@
 meow/fde/tidy3d.py
 meow_sim.egg-info/PKG-INFO
 meow_sim.egg-info/SOURCES.txt
 meow_sim.egg-info/dependency_links.txt
 meow_sim.egg-info/requires.txt
 meow_sim.egg-info/top_level.txt
 tests/test_deserialization.py
+tests/test_mode_operators.py
 tests/test_nbs.py
```

### Comparing `meow-sim-0.3.4/pyproject.toml` & `meow-sim-0.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["build", "pip", "setuptools", "wheel", "pybind11"]
 
 [project]
 name = "meow-sim"
-version = "0.3.4"
+version = "0.3.5"
 authors = [
 { name = "Rockley Photonics" },
 { name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
 ]
 description = "Modeling of Eigenmodes and Overlaps in Waveguide Structures"
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `meow-sim-0.3.4/tests/test_deserialization.py` & `meow-sim-0.3.5/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.4/tests/test_nbs.py` & `meow-sim-0.3.5/tests/test_nbs.py`

 * *Files identical despite different names*

