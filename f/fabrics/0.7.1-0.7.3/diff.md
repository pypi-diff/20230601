# Comparing `tmp/fabrics-0.7.1.tar.gz` & `tmp/fabrics-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrics-0.7.1.tar", max compression
+gzip compressed data, was "fabrics-0.7.3.tar", max compression
```

## Comparing `fabrics-0.7.1.tar` & `fabrics-0.7.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    35306 2023-03-20 15:52:59.275034 fabrics-0.7.1/LICENSE
--rw-r--r--   0        0        0     4739 2023-03-20 15:53:26.435348 fabrics-0.7.1/README.md
--rw-r--r--   0        0        0       40 2023-03-20 15:52:59.319034 fabrics-0.7.1/fabrics/.gitignore
--rw-r--r--   0        0        0       71 2023-03-20 15:52:59.319034 fabrics-0.7.1/fabrics/__init__.py
--rw-r--r--   0        0        0      249 2023-03-20 15:52:59.319034 fabrics-0.7.1/fabrics/components/energies/execution_energies.py
--rw-r--r--   0        0        0     3042 2023-03-20 15:52:59.319034 fabrics-0.7.1/fabrics/components/leaves/attractor.py
--rw-r--r--   0        0        0     2453 2023-03-20 15:52:59.319034 fabrics-0.7.1/fabrics/components/leaves/dynamic_attractor.py
--rw-r--r--   0        0        0     4365 2023-03-20 15:52:59.319034 fabrics-0.7.1/fabrics/components/leaves/dynamic_geometry.py
--rw-r--r--   0        0        0     2915 2023-03-20 15:52:59.319034 fabrics-0.7.1/fabrics/components/leaves/dynamic_leaf.py
--rw-r--r--   0        0        0     8640 2023-03-20 15:53:26.439348 fabrics-0.7.1/fabrics/components/leaves/geometry.py
--rw-r--r--   0        0        0     1059 2023-03-20 15:52:59.319034 fabrics-0.7.1/fabrics/components/leaves/leaf.py
--rw-r--r--   0        0        0     1171 2023-03-20 15:52:59.319034 fabrics-0.7.1/fabrics/components/maps/parameterized_maps.py
--rw-r--r--   0        0        0     1319 2023-03-20 15:52:59.319034 fabrics-0.7.1/fabrics/defaults/default_energies.py
--rw-r--r--   0        0        0     1609 2023-03-20 15:52:59.319034 fabrics-0.7.1/fabrics/defaults/default_geometries.py
--rw-r--r--   0        0        0      918 2023-03-20 15:52:59.319034 fabrics-0.7.1/fabrics/defaults/default_leaves.py
--rw-r--r--   0        0        0     1852 2023-03-20 15:52:59.323035 fabrics-0.7.1/fabrics/defaults/default_maps.py
--rw-r--r--   0        0        0      260 2023-03-20 15:52:59.323035 fabrics-0.7.1/fabrics/diffGeometry/casadi_helpers.py
--rw-r--r--   0        0        0     3605 2023-03-20 15:53:26.439348 fabrics-0.7.1/fabrics/diffGeometry/diffMap.py
--rw-r--r--   0        0        0     4016 2023-03-20 15:52:59.323035 fabrics-0.7.1/fabrics/diffGeometry/energized_geometry.py
--rw-r--r--   0        0        0     6868 2023-03-20 15:52:59.323035 fabrics-0.7.1/fabrics/diffGeometry/energy.py
--rw-r--r--   0        0        0     3416 2023-03-20 15:52:59.323035 fabrics-0.7.1/fabrics/diffGeometry/geometry.py
--rw-r--r--   0        0        0     6927 2023-03-20 15:52:59.323035 fabrics-0.7.1/fabrics/diffGeometry/spec.py
--rw-r--r--   0        0        0     2818 2023-03-20 15:52:59.323035 fabrics-0.7.1/fabrics/diffGeometry/speedControl.py
--rw-r--r--   0        0        0     4123 2023-03-20 15:52:59.323035 fabrics-0.7.1/fabrics/helpers/casadiFunctionWrapper.py
--rw-r--r--   0        0        0       75 2023-03-20 15:52:59.323035 fabrics-0.7.1/fabrics/helpers/constants.py
--rw-r--r--   0        0        0      273 2023-03-20 15:52:59.323035 fabrics-0.7.1/fabrics/helpers/exceptions.py
--rw-r--r--   0        0        0     2461 2023-03-20 15:52:59.323035 fabrics-0.7.1/fabrics/helpers/functions.py
--rw-r--r--   0        0        0     3940 2023-03-20 15:52:59.323035 fabrics-0.7.1/fabrics/helpers/variables.py
--rw-r--r--   0        0        0     5908 2023-03-20 15:53:26.439348 fabrics-0.7.1/fabrics/planner/non_holonomic_parameterized_planner.py
--rw-r--r--   0        0        0    21730 2023-03-20 15:53:26.439348 fabrics-0.7.1/fabrics/planner/parameterized_planner.py
--rw-r--r--   0        0        0     1548 2023-03-20 15:52:59.323035 fabrics-0.7.1/fabrics/planner/serialized_planner.py
--rw-r--r--   0        0        0     1049 2023-03-20 15:53:26.439348 fabrics-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     5706 1970-01-01 00:00:00.000000 fabrics-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    35306 2023-06-01 01:03:50.659173 fabrics-0.7.3/LICENSE
+-rw-r--r--   0        0        0     4831 2023-06-01 01:04:18.409175 fabrics-0.7.3/README.md
+-rw-r--r--   0        0        0       40 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/.gitignore
+-rw-r--r--   0        0        0       71 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/__init__.py
+-rw-r--r--   0        0        0      249 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/components/energies/execution_energies.py
+-rw-r--r--   0        0        0     3048 2023-06-01 01:04:18.517182 fabrics-0.7.3/fabrics/components/leaves/attractor.py
+-rw-r--r--   0        0        0     2453 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/components/leaves/dynamic_attractor.py
+-rw-r--r--   0        0        0     4365 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/components/leaves/dynamic_geometry.py
+-rw-r--r--   0        0        0     2915 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/components/leaves/dynamic_leaf.py
+-rw-r--r--   0        0        0     8399 2023-06-01 01:04:18.517182 fabrics-0.7.3/fabrics/components/leaves/geometry.py
+-rw-r--r--   0        0        0     2307 2023-06-01 01:04:18.517182 fabrics-0.7.3/fabrics/components/leaves/leaf.py
+-rw-r--r--   0        0        0     1171 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/components/maps/parameterized_maps.py
+-rw-r--r--   0        0        0     1319 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/defaults/default_energies.py
+-rw-r--r--   0        0        0     1609 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/defaults/default_geometries.py
+-rw-r--r--   0        0        0      918 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/defaults/default_leaves.py
+-rw-r--r--   0        0        0     1852 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/defaults/default_maps.py
+-rw-r--r--   0        0        0      260 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/diffGeometry/casadi_helpers.py
+-rw-r--r--   0        0        0     3605 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/diffGeometry/diffMap.py
+-rw-r--r--   0        0        0     4016 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/diffGeometry/energized_geometry.py
+-rw-r--r--   0        0        0     6868 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/diffGeometry/energy.py
+-rw-r--r--   0        0        0     3416 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/diffGeometry/geometry.py
+-rw-r--r--   0        0        0     6927 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/diffGeometry/spec.py
+-rw-r--r--   0        0        0     2818 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/diffGeometry/speedControl.py
+-rw-r--r--   0        0        0     6194 2023-06-01 01:04:18.517182 fabrics-0.7.3/fabrics/helpers/casadiFunctionWrapper.py
+-rw-r--r--   0        0        0       75 2023-06-01 01:03:50.819185 fabrics-0.7.3/fabrics/helpers/constants.py
+-rw-r--r--   0        0        0      273 2023-06-01 01:03:50.819185 fabrics-0.7.3/fabrics/helpers/exceptions.py
+-rw-r--r--   0        0        0     2461 2023-06-01 01:03:50.819185 fabrics-0.7.3/fabrics/helpers/functions.py
+-rw-r--r--   0        0        0     3940 2023-06-01 01:03:50.819185 fabrics-0.7.3/fabrics/helpers/variables.py
+-rw-r--r--   0        0        0     6592 2023-06-01 01:04:18.517182 fabrics-0.7.3/fabrics/planner/non_holonomic_parameterized_planner.py
+-rw-r--r--   0        0        0    21854 2023-06-01 01:04:18.517182 fabrics-0.7.3/fabrics/planner/parameterized_planner.py
+-rw-r--r--   0        0        0     1548 2023-06-01 01:03:50.819185 fabrics-0.7.3/fabrics/planner/serialized_planner.py
+-rw-r--r--   0        0        0     1045 2023-06-01 01:04:18.521183 fabrics-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     5837 1970-01-01 00:00:00.000000 fabrics-0.7.3/PKG-INFO
```

### Comparing `fabrics-0.7.1/LICENSE` & `fabrics-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.1/README.md` & `fabrics-0.7.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,17 @@
     <td> <img src="./assets/panda_ring.gif"  alt="1" width = 360px ></td>
     <td> <img src="./assets/boxer.gif"  alt="1" width = 360px ></td>
   </tr> 
   <tr>
     <td> <img src="./assets/panda_dynamic_avoidance.gif"  alt="1" width = 360px ></td>
     <td> <img src="./assets/albert.gif"  alt="1" width = 360px ></td>
   </tr>
+  <tr>
+    <td> <img src="./assets/panda_picking.gif"  alt="1" width = 360px ></td>
+  </tr>
 </table>
 
 
 ## Installation
 
 Install the package through pip, using 
 ```bash
```

#### html2text {}

```diff
@@ -11,14 +11,15 @@
 very shortly when compatibility is > verified. Geometric Fabrics represent a
 geometric approach to motion generation for various robot structures. The idea
 is a next development step after Riemannian Motion Policies and offers
 increased stability and accessibility.
 Holonomic robots Non-Holonomic robots
 [1]              [1]
 [1]              [1]
+[1]
 ## Installation Install the package through pip, using ```bash pip3 install "."
 ``` or from PyPI using ```bash pip3 install fabrics ``` Options are [agents]
 and [tutorials]. Those can be installed using ``` pip3 install ".[agents]" pip3
 install ".[tutorials]" ``` Install the package through poetry, using ```bash
 poetry install --with
 ``` ## Publications This repository was used in several publications. The major
 one being [Dynamic Optimization Fabrics for Motion Generation](https://
```

### Comparing `fabrics-0.7.1/fabrics/components/leaves/attractor.py` & `fabrics-0.7.3/fabrics/components/leaves/attractor.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,16 +46,17 @@
         else:
             weight_variable = ca.SX.sym(weight_name, 1)
         self._geo_parameters = {
             reference_name: reference_variable,
             weight_name: weight_variable
         }
         self._weight = weight_variable
+        self._leaf_variables.add_parameters(self._geo_parameters)
         self._parent_variables.add_parameters(self._geo_parameters)
-        self._forward_map = ParameterizedGoalMap(
+        self._map = ParameterizedGoalMap(
             self._parent_variables, self._forward_kinematics, reference_variable
         )
 
     def set_potential(self, potential_expression: str) -> None:
         x = self._x
         xdot = self._xdot
         new_parameters, potential = parse_symbolic_input(potential_expression, x, xdot, name=self._leaf_name)
@@ -68,9 +69,7 @@
         x = self._leaf_variables.position_variable()
         xdot = self._leaf_variables.velocity_variable()
         new_parameters, attractor_metric = parse_symbolic_input(attractor_metric_expression, x, xdot, name=self._leaf_name)
         self._parent_variables.add_parameters(new_parameters)
         lagrangian_psi = ca.dot(xdot, ca.mtimes(attractor_metric, xdot))
         self._lag = Lagrangian(lagrangian_psi, var=self._leaf_variables)
 
-    def map(self):
-        return self._forward_map
```

### Comparing `fabrics-0.7.1/fabrics/components/leaves/dynamic_attractor.py` & `fabrics-0.7.3/fabrics/components/leaves/dynamic_attractor.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.1/fabrics/components/leaves/dynamic_geometry.py` & `fabrics-0.7.3/fabrics/components/leaves/dynamic_geometry.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.1/fabrics/components/leaves/dynamic_leaf.py` & `fabrics-0.7.3/fabrics/components/leaves/dynamic_leaf.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.1/fabrics/components/leaves/geometry.py` & `fabrics-0.7.3/fabrics/components/leaves/geometry.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,18 +67,15 @@
             parent_variables,
             f"{limit_name}_leaf",
             phi,
         )
         self.set_forward_map()
 
     def set_forward_map(self):
-        self._forward_map = DifferentialMap(self._forward_kinematics, self._parent_variables)
-
-    def map(self):
-        return self._forward_map
+        self._map = DifferentialMap(self._forward_kinematics, self._parent_variables)
 
 class SelfCollisionLeaf(GenericGeometryLeaf):
     """
     The SelfCollisionLeaf is a geometry leaf for self collision avoidanceself.
 
     This leaf is not parameterized as it is not changing at runtimeself.
     """
@@ -95,18 +92,16 @@
         self.set_forward_map(self_collision_body_radius)
 
     def set_forward_map(self, self_collision_body_radius):
         phi = (
             ca.norm_2(self._forward_kinematics)
             / (2 * self_collision_body_radius) - 1
         )
-        self._forward_map = DifferentialMap(phi, self._parent_variables)
+        self._map = DifferentialMap(phi, self._parent_variables)
 
-    def map(self):
-        return self._forward_map
 
 class ObstacleLeaf(GenericGeometryLeaf):
     """
     The ObstacleLeaf is a geometry leaf for spherical obstacles.
 
     The obstacles are parameterized by the obstacles radius, its position and
     the radius of the englobing sphere for the corresponding link.
@@ -149,24 +144,22 @@
             radius_body_variable = ca.SX.sym(radius_body_name, 1)
         geo_parameters = {
             reference_name: reference_variable,
             radius_name: radius_variable,
             radius_body_name: radius_body_variable,
         }
         self._parent_variables.add_parameters(geo_parameters)
-        self._forward_map = ParameterizedObstacleMap(
+        self._map = ParameterizedObstacleMap(
             self._parent_variables,
             self._forward_kinematics,
             reference_variable,
             radius_variable,
             radius_body_variable,
         )
 
-    def map(self):
-        return self._forward_map
 
 
 class ESDFGeometryLeaf(GenericGeometryLeaf):
     """ESDFGeometryLeaf is a leaf with explicit gradients that can be set
     at runtime.
 
     Euclidean Signed Distance Fields (ESDF) can be exploited to avoid explicit
@@ -218,16 +211,14 @@
         else:
             radius_body_variable = ca.SX.sym(radius_body_name, 1)
         geo_parameters = {
             radius_body_name: radius_body_variable,
         }
         self._parent_variables.add_parameters(geo_parameters)
         phi_reduced = self._forward_kinematics - radius_body_variable
-        self._forward_map = ExplicitDifferentialMap(
+        self._map = ExplicitDifferentialMap(
             phi_reduced,
             self._parent_variables,
             J=J,
             Jdot=Jdot,
         )
 
-    def map(self):
-        return self._forward_map
```

### Comparing `fabrics-0.7.1/fabrics/components/maps/parameterized_maps.py` & `fabrics-0.7.3/fabrics/components/maps/parameterized_maps.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.1/fabrics/defaults/default_energies.py` & `fabrics-0.7.3/fabrics/defaults/default_energies.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.1/fabrics/defaults/default_geometries.py` & `fabrics-0.7.3/fabrics/defaults/default_geometries.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.1/fabrics/defaults/default_leaves.py` & `fabrics-0.7.3/fabrics/defaults/default_leaves.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.1/fabrics/defaults/default_maps.py` & `fabrics-0.7.3/fabrics/defaults/default_maps.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.1/fabrics/diffGeometry/diffMap.py` & `fabrics-0.7.3/fabrics/diffGeometry/diffMap.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.1/fabrics/diffGeometry/energized_geometry.py` & `fabrics-0.7.3/fabrics/diffGeometry/energized_geometry.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.1/fabrics/diffGeometry/energy.py` & `fabrics-0.7.3/fabrics/diffGeometry/energy.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.1/fabrics/diffGeometry/geometry.py` & `fabrics-0.7.3/fabrics/diffGeometry/geometry.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.1/fabrics/diffGeometry/spec.py` & `fabrics-0.7.3/fabrics/diffGeometry/spec.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.1/fabrics/diffGeometry/speedControl.py` & `fabrics-0.7.3/fabrics/diffGeometry/speedControl.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.1/fabrics/helpers/casadiFunctionWrapper.py` & `fabrics-0.7.3/fabrics/helpers/casadiFunctionWrapper.py`

 * *Files 25% similar despite different names*

```diff
@@ -32,25 +32,56 @@
             pickle.dump(self._function.serialize(), f)
             pickle.dump(list(self._expressions.keys()), f)
             pickle.dump(self._input_keys, f)
 
     def evaluate(self, **kwargs):
         argument_dictionary = {}
         for key in kwargs:
-            assert isinstance(kwargs[key], np.ndarray) or isinstance(kwargs[key], list) or isinstance(kwargs[key], float)
             if key == 'x_obst' or key == 'x_obsts':
                 obstacle_dictionary = {}
                 for j, x_obst_j in enumerate(kwargs[key]):
                     obstacle_dictionary[f'x_obst_{j}'] = x_obst_j
                 argument_dictionary.update(obstacle_dictionary)
             if key == 'radius_obst' or key == 'radius_obsts':
                 radius_dictionary = {}
                 for j, radius_obst_j in enumerate(kwargs[key]):
                     radius_dictionary[f'radius_obst_{j}'] = radius_obst_j
                 argument_dictionary.update(radius_dictionary)
+            if key == 'x_obst_dynamic' or key == 'x_obsts_dynamic':
+                obstacle_dyn_dictionary = {}
+                for j, x_obst_dyn_j in enumerate(kwargs[key]):
+                    obstacle_dyn_dictionary[f'x_obst_dynamic_{j}'] = x_obst_dyn_j
+                argument_dictionary.update(obstacle_dyn_dictionary)
+            if key == 'xdot_obst_dynamic' or key == 'xdot_obsts_dynamic':
+                xdot_dyn_dictionary = {}
+                for j, xdot_obst_dyn_j in enumerate(kwargs[key]):
+                    xdot_dyn_dictionary[f'xdot_obst_dynamic_{j}'] = xdot_obst_dyn_j
+                argument_dictionary.update(xdot_dyn_dictionary)
+            if key == 'xddot_obst_dynamic' or key == 'xddot_obsts_dynamic':
+                xddot_dyn_dictionary = {}
+                for j, xddot_obst_dyn_j in enumerate(kwargs[key]):
+                    xddot_dyn_dictionary[f'xddot_obst_dynamic_{j}'] = xddot_obst_dyn_j
+                argument_dictionary.update(xddot_dyn_dictionary)
+            if key == 'radius_obst_dynamic' or key == 'radius_obsts_dynamic':
+                radius_dyn_dictionary = {}
+                for j, radius_obst_dyn_j in enumerate(kwargs[key]):
+                    radius_dyn_dictionary[f'radius_obst_dynamic_{j}'] = radius_obst_dyn_j
+                argument_dictionary.update(radius_dyn_dictionary)
+            if key.startswith('radius_body') and key.endswith('links'):
+                # Radius bodies can be passed using a dictionary where the keys are simple integers.
+                radius_body_dictionary = {}
+                body_size_inputs = [input_exp for input_exp in self._input_keys if input_exp.startswith('radius_body')]
+                for link_nr, radius_body_j in kwargs[key].items():
+                    try:
+                        key = [body_size_input for body_size_input in body_size_inputs if str(link_nr) in body_size_input][0]
+                    except IndexError as e:
+                        logging.warning(f"No body link with index {link_nr} in the inputs. Body link {link_nr} is ignored.")
+                    radius_body_dictionary[key] = radius_body_j
+
+                argument_dictionary.update(radius_body_dictionary)
             else:
                 argument_dictionary[key] = kwargs[key]
         input_arrays = []
         try:
             for i in self._input_keys:
                 """
                 if not argument_dictionary[i].size == self._input_sizes[i][0] * self._input_sizes[i][1]:
```

### Comparing `fabrics-0.7.1/fabrics/helpers/functions.py` & `fabrics-0.7.3/fabrics/helpers/functions.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.1/fabrics/helpers/variables.py` & `fabrics-0.7.3/fabrics/helpers/variables.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.1/fabrics/planner/non_holonomic_parameterized_planner.py` & `fabrics-0.7.3/fabrics/planner/non_holonomic_parameterized_planner.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,16 +25,18 @@
     )
 
 class NonHolonomicParameterizedFabricPlanner(ParameterizedFabricPlanner):
     def __init__(
         self,
         dof: int,
         robot_type: str,
+        facing_direction: str = '-y',
         **kwargs
     ):
+        self.leaves = {}
         self._dof = dof
         self._config = NonHolonomicFabricPlannerConfig(**kwargs)
         if self._config.urdf:
             self._forward_kinematics = GenericURDFFk(
                 self._config.urdf,
                 rootLink=self._config.root_link,
                 end_link=self._config.end_link,
@@ -42,36 +44,48 @@
             )
         else:
             self._forward_kinematics = FkCreator(robot_type).fk()
         self.initialize_joint_variables()
         self.set_base_geometry()
         self._target_velocity = np.zeros(self._geometry.x().size()[0])
         self._ref_sign = 1
+        self.set_non_holonomic_constraints(facing_direction=facing_direction)
 
-        # Additional terms introducted by the non-holonomic base
+
+    def set_non_holonomic_constraints(self, facing_direction: str = '-y'):
         q = self._variables.position_variable()
         qdot = self._variables.velocity_variable()
         qudot = ca.SX.sym("qudot", self._dof - 1)
         new_parameters, l_offset = parse_symbolic_input(self._config.l_offset, q, qdot)
         self._variables.add_parameters(new_parameters)
         J_nh = ca.SX(np.zeros((self._dof, self._dof-1)))
-        J_nh[0, 0] = ca.cos(q[2])
-        J_nh[0, 1] = -l_offset * ca.sin(q[2])
-        J_nh[1, 0] = ca.sin(q[2])
-        J_nh[1, 1] = l_offset * ca.cos(q[2])
         for i in range(2, self._dof):
             J_nh[i, i-1] = 1
         f_extra = ca.SX(np.zeros((self._dof, 1)))
-        f_extra[0] = qudot[0] * qudot[1] * -ca.sin(q[2]) - l_offset * ca.cos(q[2]) * qudot[1]**2
-        f_extra[1] = qudot[0] * qudot[1] * ca.sin(q[2]) - l_offset * ca.sin(q[2]) * qudot[1]**2
+        if facing_direction == '-y':
+            J_nh[0, 0] = ca.sin(q[2])
+            J_nh[0, 1] = l_offset * ca.cos(q[2])
+            J_nh[1, 0] = -ca.cos(q[2])
+            J_nh[1, 1] = l_offset * ca.sin(q[2])
+            f_extra[0] = qudot[0] * qudot[1] * ca.cos(q[2]) - l_offset * ca.sin(q[2]) * qudot[1]**2
+            f_extra[1] = qudot[0] * qudot[1] * ca.sin(q[2]) + l_offset * ca.cos(q[2]) * qudot[1]**2
+        elif facing_direction == 'x':
+            logging.warning("Not sure about this, yet.")
+            J_nh[0, 0] = ca.cos(q[2])
+            J_nh[0, 1] = -l_offset * ca.sin(q[2])
+            J_nh[1, 0] = ca.sin(q[2])
+            J_nh[1, 1] = l_offset * ca.cos(q[2])
+            f_extra[0] = qudot[0] * qudot[1] * -ca.sin(q[2]) - l_offset * ca.cos(q[2]) * qudot[1]**2
+            f_extra[1] = qudot[0] * qudot[1] * ca.sin(q[2]) - l_offset * ca.sin(q[2]) * qudot[1]**2
         self._J_nh = J_nh
         self._f_extra = f_extra
         self._qudot = qudot
         self._variables.add_state_variable('qudot', qudot)
 
+
     def set_base_geometry(self):
         q = self._variables.position_variable()
         qdot = self._variables.velocity_variable()
         new_parameters, M_base_energy =  parse_symbolic_input(self._config.M_base_energy, q, qdot)
         self._variables.add_parameters(new_parameters)
         new_parameters, M_arm_energy =  parse_symbolic_input(self._config.M_arm_energy, q, qdot)
         self._variables.add_parameters(new_parameters)
```

### Comparing `fabrics-0.7.1/fabrics/planner/parameterized_planner.py` & `fabrics-0.7.3/fabrics/planner/parameterized_planner.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Dict
 import logging
 import casadi as ca
 from forwardkinematics.urdfFks.urdfFk import LinkNotInURDFError
 import numpy as np
 from copy import deepcopy
 from fabrics.helpers.exceptions import ExpressionSparseError
+from typing import List
 
 from fabrics.helpers.variables import Variables
 from fabrics.helpers.constants import eps
 from fabrics.helpers.functions import is_sparse, parse_symbolic_input
 
 from fabrics.diffGeometry.diffMap import DifferentialMap, DynamicDifferentialMap
 from fabrics.diffGeometry.energy import Lagrangian
@@ -33,14 +34,17 @@
 from forwardkinematics.urdfFks.generic_urdf_fk import GenericURDFFk
 
 from pyquaternion import Quaternion
 
 class InvalidRotationAnglesError(Exception):
     pass
 
+class LeafNotFoundError(Exception):
+    pass
+
 def compute_rotation_matrix(angles) -> np.ndarray:
     if isinstance(angles, float):
         angle = angles
         return np.array([[np.cos(angle), np.sin(angle)], [-np.sin(angle), np.cos(angle)]])
     elif isinstance(angles, list) and len(angles) == 4:
         quaternion = Quaternion(angles)
         return quaternion.rotation_matrix
@@ -111,14 +115,15 @@
             )
         else:
             self._forward_kinematics = FkCreator(robot_type).fk()
         self.initialize_joint_variables()
         self.set_base_geometry()
         self._target_velocity = np.zeros(self._geometry.x().size()[0])
         self._ref_sign = 1
+        self.leaves = {}
 
     """ INITIALIZING """
 
     def initialize_joint_variables(self):
         q = ca.SX.sym("q", self._dof)
         qdot = ca.SX.sym("qdot", self._dof)
         self._variables = Variables(state_variables={"q": q, "qdot": qdot})
@@ -185,14 +190,25 @@
             self.add_forcing_geometry(leaf.map(), leaf.lagrangian(), leaf.geometry(), prime_leaf)
         elif isinstance(leaf, GenericDynamicAttractor):
             self.add_dynamic_forcing_geometry(leaf.map(), leaf.dynamic_map(), leaf.lagrangian(), leaf.geometry(), leaf._xdot_ref, prime_leaf)
         elif isinstance(leaf, GenericGeometryLeaf):
             self.add_geometry(leaf.map(), leaf.lagrangian(), leaf.geometry())
         elif isinstance(leaf, GenericDynamicGeometryLeaf):
             self.add_dynamic_geometry(leaf.map(), leaf.dynamic_map(), leaf.geometry_map(), leaf.lagrangian(), leaf.geometry())
+        self.leaves[leaf._leaf_name] = leaf
+
+    def get_leaves(self, leaf_names:list) -> List[Leaf]:
+        leaves = []
+        for leaf_name in leaf_names:
+            if leaf_name not in self.leaves:
+                error_message = f"Leaf with name {leaf_name} not in leaves.\n"
+                error_message = f"Possible leaves are {list(self.leaves.keys())}."
+                raise LeafNotFoundError(error_message)
+            leaves.append(self.leaves[leaf_name])
+        return leaves
 
     def add_forcing_geometry(
         self,
         forward_map: DifferentialMap,
         lagrangian: Lagrangian,
         geometry: Geometry,
         prime_forcing_leaf: bool,
@@ -281,55 +297,39 @@
             fk = self._forward_kinematics.fk(
                 self._variables.position_variable(),
                 link_name,
                 positionOnly=True
             )
         return fk
 
-    def get_forward_kinematics_F(self, link_name) -> ca.SX:
-        if isinstance(link_name, ca.SX):
-            return link_name
-        if self._config.urdf:
-            fk = self._forward_kinematics.fk(
-                self._variables.position_variable(),
-                self._config.root_link,
-                link_name,
-                positionOnly=True
-            )
-        else:
-            fk = self._forward_kinematics.fk(
-                self._variables.position_variable(),
-                link_name,
-                positionOnly=True
-            )
-        return fk_fun
 
     """ DEFAULT COMPOSITION """
     def set_components(
         self,
         collision_links: list = None,
         self_collision_pairs: dict = None,
         collision_links_esdf: list = None,
         goal: GoalComposition = None,
         limits: list = None,
         number_obstacles: int = 1,
         number_dynamic_obstacles: int = 0,
+        dynamic_obstacle_dimension: int = 3,
     ):
         if collision_links is None:
             collision_links = []
         if collision_links_esdf is None:
             collision_links_esdf = []
         if self_collision_pairs is None:
             self_collision_pairs = {}
         reference_parameter_list = []
         for i in range(number_dynamic_obstacles):
             reference_parameters = {
-                f"x_obst_dynamic_{i}": ca.SX.sym(f"x_obst_dynamic_{i}", 3),
-                f"xdot_obst_dynamic_{i}": ca.SX.sym(f"xdot_obst_dynamic_{i}", 3),
-                f"xddot_obst_dynamic_{i}": ca.SX.sym(f"xddot_obst_dynamic_{i}", 3),
+                f"x_obst_dynamic_{i}": ca.SX.sym(f"x_obst_dynamic_{i}", dynamic_obstacle_dimension),
+                f"xdot_obst_dynamic_{i}": ca.SX.sym(f"xdot_obst_dynamic_{i}", dynamic_obstacle_dimension),
+                f"xddot_obst_dynamic_{i}": ca.SX.sym(f"xddot_obst_dynamic_{i}", dynamic_obstacle_dimension),
             }
             reference_parameter_list.append(reference_parameters)
         for collision_link in collision_links:
             fk = self.get_forward_kinematics(collision_link)
             if is_sparse(fk):
                 logging.warning(f"Expression {fk} for link {collision_link} is sparse and thus skipped.")
                 continue
```

### Comparing `fabrics-0.7.1/fabrics/planner/serialized_planner.py` & `fabrics-0.7.3/fabrics/planner/serialized_planner.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.1/pyproject.toml` & `fabrics-0.7.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fabrics"
-version = "0.7.1"
+version = "0.7.3"
 description = "Optimization fabrics in python."
 authors = ["Max Spahn <m.spahn@tudelft.nl>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 repository = "https://tud-amr/fabrics"
 keywords = ["robotics", "motion-planning", "geometry"]
 
@@ -14,34 +14,34 @@
 numpy = "^1.15.3"
 geomdl = "^5.3.1"
 pyquaternion = "^0.9.9"
 pickle-mixin = "^1.0.2"
 quaternionic = "^1.0.0"
 forwardkinematics = "^1.0"
 mpscenes = "^0.3"
+pynput = "^1.7.6"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.13.4"
 pytest = "^6.2.5"
 pytest-cov = "^4.0.0"
 
 [tool.poetry.group.tutorials]
 optional = true
 
 [tool.poetry.group.tutorials.dependencies]
 planarenvs = "^1.3.2"
-matplotlib = "^3.7.0"
 jupyterlab = "^3.6.1"
 
 [tool.poetry.group.agents]
 optional = true
 
 [tool.poetry.group.agents.dependencies]
-urdfenvs = "^0.5.2"
-planarenvs = "^1.3.1"
+urdfenvs = "^0.7.6"
+planarenvs = "^1.3.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fabrics-0.7.1/PKG-INFO` & `fabrics-0.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabrics
-Version: 0.7.1
+Version: 0.7.3
 Summary: Optimization fabrics in python.
 Home-page: https://tud-amr/fabrics
 License: GPL-3.0-or-later
 Keywords: robotics,motion-planning,geometry
 Author: Max Spahn
 Author-email: m.spahn@tudelft.nl
 Requires-Python: >=3.8,<3.10
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: casadi (>=3.5.4,<4.0.0,!=3.5.5.post1,!=3.5.5.post1)
 Requires-Dist: forwardkinematics (>=1.0,<2.0)
 Requires-Dist: geomdl (>=5.3.1,<6.0.0)
 Requires-Dist: mpscenes (>=0.3,<0.4)
 Requires-Dist: numpy (>=1.15.3,<2.0.0)
 Requires-Dist: pickle-mixin (>=1.0.2,<2.0.0)
+Requires-Dist: pynput (>=1.7.6,<2.0.0)
 Requires-Dist: pyquaternion (>=0.9.9,<0.10.0)
 Requires-Dist: quaternionic (>=1.0.0,<2.0.0)
 Project-URL: Repository, https://tud-amr/fabrics
 Description-Content-Type: text/markdown
 
 # (Geometric) Fabrics
 
@@ -52,14 +53,17 @@
     <td> <img src="./assets/panda_ring.gif"  alt="1" width = 360px ></td>
     <td> <img src="./assets/boxer.gif"  alt="1" width = 360px ></td>
   </tr> 
   <tr>
     <td> <img src="./assets/panda_dynamic_avoidance.gif"  alt="1" width = 360px ></td>
     <td> <img src="./assets/albert.gif"  alt="1" width = 360px ></td>
   </tr>
+  <tr>
+    <td> <img src="./assets/panda_picking.gif"  alt="1" width = 360px ></td>
+  </tr>
 </table>
 
 
 ## Installation
 
 Install the package through pip, using 
 ```bash
```

#### html2text {}

```diff
@@ -1,37 +1,38 @@
-Metadata-Version: 2.1 Name: fabrics Version: 0.7.1 Summary: Optimization
+Metadata-Version: 2.1 Name: fabrics Version: 0.7.3 Summary: Optimization
 fabrics in python. Home-page: https://tud-amr/fabrics License: GPL-3.0-or-later
 Keywords: robotics,motion-planning,geometry Author: Max Spahn Author-email:
 m.spahn@tudelft.nl Requires-Python: >=3.8,<3.10 Classifier: License :: OSI
 Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Requires-Dist: casadi
 (>=3.5.4,<4.0.0,!=3.5.5.post1,!=3.5.5.post1) Requires-Dist: forwardkinematics
 (>=1.0,<2.0) Requires-Dist: geomdl (>=5.3.1,<6.0.0) Requires-Dist: mpscenes
 (>=0.3,<0.4) Requires-Dist: numpy (>=1.15.3,<2.0.0) Requires-Dist: pickle-mixin
-(>=1.0.2,<2.0.0) Requires-Dist: pyquaternion (>=0.9.9,<0.10.0) Requires-Dist:
-quaternionic (>=1.0.0,<2.0.0) Project-URL: Repository, https://tud-amr/fabrics
-Description-Content-Type: text/markdown # (Geometric) Fabrics [![Build and
-Agents](https://github.com/maxspahn/fabrics/actions/workflows/
-diffGeo_agents.yml/badge.svg)](https://github.com/maxspahn/fabrics/actions/
-workflows/diffGeo_agents.yml) [![Build and Unittest](https://github.com/
-maxspahn/fabrics/actions/workflows/unitTest.yml/badge.svg)](https://github.com/
-maxspahn/fabrics/actions/workflows/unitTest.yml) **Note on development** > This
-project is still under heavy development and there is a lack of >
-documentation. I, @maxspahn, am committed to improve and maintain that package.
-> However, I rely on people like you to point me to issues and unclear sections
-of > the code. So feel free to leave issues whenever something bugs you.
-**Fabrics ros-wrapper** > The fabrics-ros wrapper will be released very shortly
-when compatibility is > verified. Geometric Fabrics represent a geometric
-approach to motion generation for various robot structures. The idea is a next
-development step after Riemannian Motion Policies and offers increased
-stability and accessibility.
+(>=1.0.2,<2.0.0) Requires-Dist: pynput (>=1.7.6,<2.0.0) Requires-Dist:
+pyquaternion (>=0.9.9,<0.10.0) Requires-Dist: quaternionic (>=1.0.0,<2.0.0)
+Project-URL: Repository, https://tud-amr/fabrics Description-Content-Type:
+text/markdown # (Geometric) Fabrics [![Build and Agents](https://github.com/
+maxspahn/fabrics/actions/workflows/diffGeo_agents.yml/badge.svg)](https://
+github.com/maxspahn/fabrics/actions/workflows/diffGeo_agents.yml) [![Build and
+Unittest](https://github.com/maxspahn/fabrics/actions/workflows/unitTest.yml/
+badge.svg)](https://github.com/maxspahn/fabrics/actions/workflows/unitTest.yml)
+**Note on development** > This project is still under heavy development and
+there is a lack of > documentation. I, @maxspahn, am committed to improve and
+maintain that package. > However, I rely on people like you to point me to
+issues and unclear sections of > the code. So feel free to leave issues
+whenever something bugs you. **Fabrics ros-wrapper** > The fabrics-ros wrapper
+will be released very shortly when compatibility is > verified. Geometric
+Fabrics represent a geometric approach to motion generation for various robot
+structures. The idea is a next development step after Riemannian Motion
+Policies and offers increased stability and accessibility.
 Holonomic robots Non-Holonomic robots
 [1]              [1]
 [1]              [1]
+[1]
 ## Installation Install the package through pip, using ```bash pip3 install "."
 ``` or from PyPI using ```bash pip3 install fabrics ``` Options are [agents]
 and [tutorials]. Those can be installed using ``` pip3 install ".[agents]" pip3
 install ".[tutorials]" ``` Install the package through poetry, using ```bash
 poetry install --with
 ``` ## Publications This repository was used in several publications. The major
 one being [Dynamic Optimization Fabrics for Motion Generation](https://
```

