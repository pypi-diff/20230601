# Comparing `tmp/chemfunc-1.0.1.tar.gz` & `tmp/chemfunc-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemfunc-1.0.1.tar", last modified: Thu Jun  1 18:58:04 2023, max compression
+gzip compressed data, was "chemfunc-1.0.2.tar", last modified: Thu Jun  1 19:02:55 2023, max compression
```

## Comparing `chemfunc-1.0.1.tar` & `chemfunc-1.0.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-06-01 18:58:04.023733 chemfunc-1.0.1/
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1069 2023-03-07 02:37:32.000000 chemfunc-1.0.1/LICENSE
--rw-r--r--   0 kyleswanson   (501) staff       (20)     6386 2023-06-01 18:58:04.024005 chemfunc-1.0.1/PKG-INFO
--rw-r--r--   0 kyleswanson   (501) staff       (20)     5644 2023-05-25 21:30:47.000000 chemfunc-1.0.1/README.md
-drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-06-01 18:58:04.018480 chemfunc-1.0.1/chemfunc/
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2014 2023-05-23 23:24:43.000000 chemfunc-1.0.1/chemfunc/__init__.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)      176 2023-06-01 18:56:51.000000 chemfunc-1.0.1/chemfunc/_version.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2841 2023-05-23 23:24:43.000000 chemfunc-1.0.1/chemfunc/canonicalize_smiles.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2007 2023-05-23 23:24:43.000000 chemfunc-1.0.1/chemfunc/chemical_diversity.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1583 2023-05-23 23:24:43.000000 chemfunc-1.0.1/chemfunc/cluster_molecules.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1520 2023-05-23 23:24:43.000000 chemfunc-1.0.1/chemfunc/compute_properties.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)      137 2023-03-07 00:44:25.000000 chemfunc-1.0.1/chemfunc/constants.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)      877 2023-05-23 23:24:43.000000 chemfunc-1.0.1/chemfunc/deduplicate_smiles.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     4002 2023-05-23 18:54:45.000000 chemfunc-1.0.1/chemfunc/filter_molecules.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1199 2023-05-23 23:24:43.000000 chemfunc-1.0.1/chemfunc/main.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2643 2023-05-23 20:59:02.000000 chemfunc-1.0.1/chemfunc/measure_experimental_reproducibility.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     4557 2023-05-23 23:24:43.000000 chemfunc-1.0.1/chemfunc/molecular_fingerprints.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     3588 2023-06-01 18:56:11.000000 chemfunc-1.0.1/chemfunc/molecular_properties.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     8551 2023-05-23 23:24:43.000000 chemfunc-1.0.1/chemfunc/molecular_similarities.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     3387 2023-05-23 23:24:43.000000 chemfunc-1.0.1/chemfunc/nearest_neighbor.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1659 2023-05-23 21:00:59.000000 chemfunc-1.0.1/chemfunc/plot_property_distribution.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     6620 2023-05-23 23:24:43.000000 chemfunc-1.0.1/chemfunc/plot_tsne.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1672 2023-05-23 18:54:45.000000 chemfunc-1.0.1/chemfunc/regression_to_classification.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1654 2023-05-23 18:54:45.000000 chemfunc-1.0.1/chemfunc/sample_molecules.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1956 2023-05-23 23:24:43.000000 chemfunc-1.0.1/chemfunc/sdf_to_smiles.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1223 2023-05-23 23:24:43.000000 chemfunc-1.0.1/chemfunc/select_from_clusters.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)      878 2023-05-23 21:04:54.000000 chemfunc-1.0.1/chemfunc/smiles_to_svg.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2129 2023-05-23 18:54:45.000000 chemfunc-1.0.1/chemfunc/utils.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2514 2023-05-23 23:24:43.000000 chemfunc-1.0.1/chemfunc/visualize_molecules.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2141 2023-05-23 21:10:47.000000 chemfunc-1.0.1/chemfunc/visualize_reactions.py
-drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-06-01 18:58:04.023175 chemfunc-1.0.1/chemfunc.egg-info/
--rw-r--r--   0 kyleswanson   (501) staff       (20)     6386 2023-06-01 18:58:03.000000 chemfunc-1.0.1/chemfunc.egg-info/PKG-INFO
--rw-r--r--   0 kyleswanson   (501) staff       (20)      974 2023-06-01 18:58:03.000000 chemfunc-1.0.1/chemfunc.egg-info/SOURCES.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)        1 2023-06-01 18:58:03.000000 chemfunc-1.0.1/chemfunc.egg-info/dependency_links.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)       48 2023-06-01 18:58:03.000000 chemfunc-1.0.1/chemfunc.egg-info/entry_points.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)       93 2023-06-01 18:58:03.000000 chemfunc-1.0.1/chemfunc.egg-info/requires.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)        9 2023-06-01 18:58:03.000000 chemfunc-1.0.1/chemfunc.egg-info/top_level.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)       79 2023-06-01 18:58:04.024853 chemfunc-1.0.1/setup.cfg
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1612 2023-05-23 23:24:43.000000 chemfunc-1.0.1/setup.py
+drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-06-01 19:02:55.337622 chemfunc-1.0.2/
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1069 2023-03-07 02:37:32.000000 chemfunc-1.0.2/LICENSE
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     6386 2023-06-01 19:02:55.337757 chemfunc-1.0.2/PKG-INFO
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     5644 2023-05-25 21:30:47.000000 chemfunc-1.0.2/README.md
+drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-06-01 19:02:55.335330 chemfunc-1.0.2/chemfunc/
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2014 2023-05-23 23:24:43.000000 chemfunc-1.0.2/chemfunc/__init__.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      176 2023-06-01 19:01:59.000000 chemfunc-1.0.2/chemfunc/_version.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2841 2023-05-23 23:24:43.000000 chemfunc-1.0.2/chemfunc/canonicalize_smiles.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2007 2023-05-23 23:24:43.000000 chemfunc-1.0.2/chemfunc/chemical_diversity.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1583 2023-05-23 23:24:43.000000 chemfunc-1.0.2/chemfunc/cluster_molecules.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1520 2023-05-23 23:24:43.000000 chemfunc-1.0.2/chemfunc/compute_properties.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      137 2023-03-07 00:44:25.000000 chemfunc-1.0.2/chemfunc/constants.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      877 2023-05-23 23:24:43.000000 chemfunc-1.0.2/chemfunc/deduplicate_smiles.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     4002 2023-05-23 18:54:45.000000 chemfunc-1.0.2/chemfunc/filter_molecules.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1199 2023-05-23 23:24:43.000000 chemfunc-1.0.2/chemfunc/main.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2643 2023-05-23 20:59:02.000000 chemfunc-1.0.2/chemfunc/measure_experimental_reproducibility.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     4557 2023-05-23 23:24:43.000000 chemfunc-1.0.2/chemfunc/molecular_fingerprints.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     4093 2023-06-01 19:01:48.000000 chemfunc-1.0.2/chemfunc/molecular_properties.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     8551 2023-05-23 23:24:43.000000 chemfunc-1.0.2/chemfunc/molecular_similarities.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     3387 2023-05-23 23:24:43.000000 chemfunc-1.0.2/chemfunc/nearest_neighbor.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1659 2023-05-23 21:00:59.000000 chemfunc-1.0.2/chemfunc/plot_property_distribution.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     6620 2023-05-23 23:24:43.000000 chemfunc-1.0.2/chemfunc/plot_tsne.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1672 2023-05-23 18:54:45.000000 chemfunc-1.0.2/chemfunc/regression_to_classification.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1654 2023-05-23 18:54:45.000000 chemfunc-1.0.2/chemfunc/sample_molecules.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1956 2023-05-23 23:24:43.000000 chemfunc-1.0.2/chemfunc/sdf_to_smiles.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1223 2023-05-23 23:24:43.000000 chemfunc-1.0.2/chemfunc/select_from_clusters.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      878 2023-05-23 21:04:54.000000 chemfunc-1.0.2/chemfunc/smiles_to_svg.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2129 2023-05-23 18:54:45.000000 chemfunc-1.0.2/chemfunc/utils.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2514 2023-05-23 23:24:43.000000 chemfunc-1.0.2/chemfunc/visualize_molecules.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2141 2023-05-23 21:10:47.000000 chemfunc-1.0.2/chemfunc/visualize_reactions.py
+drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-06-01 19:02:55.337341 chemfunc-1.0.2/chemfunc.egg-info/
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     6386 2023-06-01 19:02:55.000000 chemfunc-1.0.2/chemfunc.egg-info/PKG-INFO
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      974 2023-06-01 19:02:55.000000 chemfunc-1.0.2/chemfunc.egg-info/SOURCES.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)        1 2023-06-01 19:02:55.000000 chemfunc-1.0.2/chemfunc.egg-info/dependency_links.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)       48 2023-06-01 19:02:55.000000 chemfunc-1.0.2/chemfunc.egg-info/entry_points.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)       93 2023-06-01 19:02:55.000000 chemfunc-1.0.2/chemfunc.egg-info/requires.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)        9 2023-06-01 19:02:55.000000 chemfunc-1.0.2/chemfunc.egg-info/top_level.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)       79 2023-06-01 19:02:55.338273 chemfunc-1.0.2/setup.cfg
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1612 2023-05-23 23:24:43.000000 chemfunc-1.0.2/setup.py
```

### Comparing `chemfunc-1.0.1/LICENSE` & `chemfunc-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.1/PKG-INFO` & `chemfunc-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chemfunc
-Version: 1.0.1
+Version: 1.0.2
 Summary: Chem Func
 Home-page: https://github.com/swansonk14/chemfunc
-Download-URL: https://github.com/swansonk14/chemfunc/v_1.0.1.tar.gz
+Download-URL: https://github.com/swansonk14/chemfunc/v_1.0.2.tar.gz
 Author: Kyle Swanson
 Author-email: swansonk.14@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/swansonk14/chemfunc
 Project-URL: PyPi, https://pypi.org/project/chemfunc/
 Keywords: computational chemistry
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chemfunc-1.0.1/README.md` & `chemfunc-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.1/chemfunc/__init__.py` & `chemfunc-1.0.2/chemfunc/__init__.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.1/chemfunc/canonicalize_smiles.py` & `chemfunc-1.0.2/chemfunc/canonicalize_smiles.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.1/chemfunc/chemical_diversity.py` & `chemfunc-1.0.2/chemfunc/chemical_diversity.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.1/chemfunc/cluster_molecules.py` & `chemfunc-1.0.2/chemfunc/cluster_molecules.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.1/chemfunc/compute_properties.py` & `chemfunc-1.0.2/chemfunc/compute_properties.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.1/chemfunc/deduplicate_smiles.py` & `chemfunc-1.0.2/chemfunc/deduplicate_smiles.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.1/chemfunc/filter_molecules.py` & `chemfunc-1.0.2/chemfunc/filter_molecules.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.1/chemfunc/main.py` & `chemfunc-1.0.2/chemfunc/main.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.1/chemfunc/measure_experimental_reproducibility.py` & `chemfunc-1.0.2/chemfunc/measure_experimental_reproducibility.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.1/chemfunc/molecular_fingerprints.py` & `chemfunc-1.0.2/chemfunc/molecular_fingerprints.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.1/chemfunc/molecular_properties.py` & `chemfunc-1.0.2/chemfunc/molecular_properties.py`

 * *Files 9% similar despite different names*

```diff
@@ -105,8 +105,17 @@
         """Computes the synthetic accessibility (SA) score of a molecule.
 
         :param molecule: A molecule, either a SMILES string or an RDKit molecule.
         :return: The SA score of the molecule.
         """
         return sascorer.calculateScore(molecule)
 except ModuleNotFoundError:
-    pass
+    @register_property_function('sa_score')
+    @smiles_to_mol_wrapper
+    def compute_sa_score(molecule: Molecule) -> float:
+        """Computes the synthetic accessibility (SA) score of a molecule.
+
+        :param molecule: A molecule, either a SMILES string or an RDKit molecule.
+        :return: The SA score of the molecule.
+        """
+        raise ModuleNotFoundError('The SA Score module is not installed properly with RDKit. '
+                                  'Please install it to use this property.')
```

### Comparing `chemfunc-1.0.1/chemfunc/molecular_similarities.py` & `chemfunc-1.0.2/chemfunc/molecular_similarities.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.1/chemfunc/nearest_neighbor.py` & `chemfunc-1.0.2/chemfunc/nearest_neighbor.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.1/chemfunc/plot_property_distribution.py` & `chemfunc-1.0.2/chemfunc/plot_property_distribution.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.1/chemfunc/plot_tsne.py` & `chemfunc-1.0.2/chemfunc/plot_tsne.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.1/chemfunc/regression_to_classification.py` & `chemfunc-1.0.2/chemfunc/regression_to_classification.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.1/chemfunc/sample_molecules.py` & `chemfunc-1.0.2/chemfunc/sample_molecules.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.1/chemfunc/sdf_to_smiles.py` & `chemfunc-1.0.2/chemfunc/sdf_to_smiles.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.1/chemfunc/select_from_clusters.py` & `chemfunc-1.0.2/chemfunc/select_from_clusters.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.1/chemfunc/smiles_to_svg.py` & `chemfunc-1.0.2/chemfunc/smiles_to_svg.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.1/chemfunc/utils.py` & `chemfunc-1.0.2/chemfunc/utils.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.1/chemfunc/visualize_molecules.py` & `chemfunc-1.0.2/chemfunc/visualize_molecules.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.1/chemfunc/visualize_reactions.py` & `chemfunc-1.0.2/chemfunc/visualize_reactions.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.1/chemfunc.egg-info/PKG-INFO` & `chemfunc-1.0.2/chemfunc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chemfunc
-Version: 1.0.1
+Version: 1.0.2
 Summary: Chem Func
 Home-page: https://github.com/swansonk14/chemfunc
-Download-URL: https://github.com/swansonk14/chemfunc/v_1.0.1.tar.gz
+Download-URL: https://github.com/swansonk14/chemfunc/v_1.0.2.tar.gz
 Author: Kyle Swanson
 Author-email: swansonk.14@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/swansonk14/chemfunc
 Project-URL: PyPi, https://pypi.org/project/chemfunc/
 Keywords: computational chemistry
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chemfunc-1.0.1/chemfunc.egg-info/SOURCES.txt` & `chemfunc-1.0.2/chemfunc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.1/setup.py` & `chemfunc-1.0.2/setup.py`

 * *Files identical despite different names*

