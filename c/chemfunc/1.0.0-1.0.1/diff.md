# Comparing `tmp/chemfunc-1.0.0.tar.gz` & `tmp/chemfunc-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemfunc-1.0.0.tar", last modified: Tue May 23 23:33:38 2023, max compression
+gzip compressed data, was "chemfunc-1.0.1.tar", last modified: Thu Jun  1 18:58:04 2023, max compression
```

## Comparing `chemfunc-1.0.0.tar` & `chemfunc-1.0.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-05-23 23:33:38.006001 chemfunc-1.0.0/
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1069 2023-03-07 02:37:32.000000 chemfunc-1.0.0/LICENSE
--rw-r--r--   0 kyleswanson   (501) staff       (20)     5085 2023-05-23 23:33:38.006169 chemfunc-1.0.0/PKG-INFO
--rw-r--r--   0 kyleswanson   (501) staff       (20)     4343 2023-05-23 23:26:14.000000 chemfunc-1.0.0/README.md
-drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-05-23 23:33:38.002431 chemfunc-1.0.0/chemfunc/
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2014 2023-05-23 23:24:43.000000 chemfunc-1.0.0/chemfunc/__init__.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)      176 2023-05-23 23:24:43.000000 chemfunc-1.0.0/chemfunc/_version.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2841 2023-05-23 23:24:43.000000 chemfunc-1.0.0/chemfunc/canonicalize_smiles.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2007 2023-05-23 23:24:43.000000 chemfunc-1.0.0/chemfunc/chemical_diversity.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1583 2023-05-23 23:24:43.000000 chemfunc-1.0.0/chemfunc/cluster_molecules.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1520 2023-05-23 23:24:43.000000 chemfunc-1.0.0/chemfunc/compute_properties.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)      137 2023-03-07 00:44:25.000000 chemfunc-1.0.0/chemfunc/constants.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)      877 2023-05-23 23:24:43.000000 chemfunc-1.0.0/chemfunc/deduplicate_smiles.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     4002 2023-05-23 18:54:45.000000 chemfunc-1.0.0/chemfunc/filter_molecules.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1199 2023-05-23 23:24:43.000000 chemfunc-1.0.0/chemfunc/main.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2643 2023-05-23 20:59:02.000000 chemfunc-1.0.0/chemfunc/measure_experimental_reproducibility.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     4557 2023-05-23 23:24:43.000000 chemfunc-1.0.0/chemfunc/molecular_fingerprints.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     3492 2023-05-23 23:24:43.000000 chemfunc-1.0.0/chemfunc/molecular_properties.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     8551 2023-05-23 23:24:43.000000 chemfunc-1.0.0/chemfunc/molecular_similarities.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     3387 2023-05-23 23:24:43.000000 chemfunc-1.0.0/chemfunc/nearest_neighbor.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1659 2023-05-23 21:00:59.000000 chemfunc-1.0.0/chemfunc/plot_property_distribution.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     6620 2023-05-23 23:24:43.000000 chemfunc-1.0.0/chemfunc/plot_tsne.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1672 2023-05-23 18:54:45.000000 chemfunc-1.0.0/chemfunc/regression_to_classification.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1654 2023-05-23 18:54:45.000000 chemfunc-1.0.0/chemfunc/sample_molecules.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1956 2023-05-23 23:24:43.000000 chemfunc-1.0.0/chemfunc/sdf_to_smiles.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1223 2023-05-23 23:24:43.000000 chemfunc-1.0.0/chemfunc/select_from_clusters.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)      878 2023-05-23 21:04:54.000000 chemfunc-1.0.0/chemfunc/smiles_to_svg.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2129 2023-05-23 18:54:45.000000 chemfunc-1.0.0/chemfunc/utils.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2514 2023-05-23 23:24:43.000000 chemfunc-1.0.0/chemfunc/visualize_molecules.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2141 2023-05-23 21:10:47.000000 chemfunc-1.0.0/chemfunc/visualize_reactions.py
-drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-05-23 23:33:38.005634 chemfunc-1.0.0/chemfunc.egg-info/
--rw-r--r--   0 kyleswanson   (501) staff       (20)     5085 2023-05-23 23:33:37.000000 chemfunc-1.0.0/chemfunc.egg-info/PKG-INFO
--rw-r--r--   0 kyleswanson   (501) staff       (20)      974 2023-05-23 23:33:37.000000 chemfunc-1.0.0/chemfunc.egg-info/SOURCES.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)        1 2023-05-23 23:33:37.000000 chemfunc-1.0.0/chemfunc.egg-info/dependency_links.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)       48 2023-05-23 23:33:37.000000 chemfunc-1.0.0/chemfunc.egg-info/entry_points.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)       93 2023-05-23 23:33:37.000000 chemfunc-1.0.0/chemfunc.egg-info/requires.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)        9 2023-05-23 23:33:37.000000 chemfunc-1.0.0/chemfunc.egg-info/top_level.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)       79 2023-05-23 23:33:38.006798 chemfunc-1.0.0/setup.cfg
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1612 2023-05-23 23:24:43.000000 chemfunc-1.0.0/setup.py
+drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-06-01 18:58:04.023733 chemfunc-1.0.1/
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1069 2023-03-07 02:37:32.000000 chemfunc-1.0.1/LICENSE
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     6386 2023-06-01 18:58:04.024005 chemfunc-1.0.1/PKG-INFO
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     5644 2023-05-25 21:30:47.000000 chemfunc-1.0.1/README.md
+drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-06-01 18:58:04.018480 chemfunc-1.0.1/chemfunc/
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2014 2023-05-23 23:24:43.000000 chemfunc-1.0.1/chemfunc/__init__.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      176 2023-06-01 18:56:51.000000 chemfunc-1.0.1/chemfunc/_version.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2841 2023-05-23 23:24:43.000000 chemfunc-1.0.1/chemfunc/canonicalize_smiles.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2007 2023-05-23 23:24:43.000000 chemfunc-1.0.1/chemfunc/chemical_diversity.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1583 2023-05-23 23:24:43.000000 chemfunc-1.0.1/chemfunc/cluster_molecules.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1520 2023-05-23 23:24:43.000000 chemfunc-1.0.1/chemfunc/compute_properties.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      137 2023-03-07 00:44:25.000000 chemfunc-1.0.1/chemfunc/constants.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      877 2023-05-23 23:24:43.000000 chemfunc-1.0.1/chemfunc/deduplicate_smiles.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     4002 2023-05-23 18:54:45.000000 chemfunc-1.0.1/chemfunc/filter_molecules.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1199 2023-05-23 23:24:43.000000 chemfunc-1.0.1/chemfunc/main.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2643 2023-05-23 20:59:02.000000 chemfunc-1.0.1/chemfunc/measure_experimental_reproducibility.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     4557 2023-05-23 23:24:43.000000 chemfunc-1.0.1/chemfunc/molecular_fingerprints.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     3588 2023-06-01 18:56:11.000000 chemfunc-1.0.1/chemfunc/molecular_properties.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     8551 2023-05-23 23:24:43.000000 chemfunc-1.0.1/chemfunc/molecular_similarities.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     3387 2023-05-23 23:24:43.000000 chemfunc-1.0.1/chemfunc/nearest_neighbor.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1659 2023-05-23 21:00:59.000000 chemfunc-1.0.1/chemfunc/plot_property_distribution.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     6620 2023-05-23 23:24:43.000000 chemfunc-1.0.1/chemfunc/plot_tsne.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1672 2023-05-23 18:54:45.000000 chemfunc-1.0.1/chemfunc/regression_to_classification.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1654 2023-05-23 18:54:45.000000 chemfunc-1.0.1/chemfunc/sample_molecules.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1956 2023-05-23 23:24:43.000000 chemfunc-1.0.1/chemfunc/sdf_to_smiles.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1223 2023-05-23 23:24:43.000000 chemfunc-1.0.1/chemfunc/select_from_clusters.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      878 2023-05-23 21:04:54.000000 chemfunc-1.0.1/chemfunc/smiles_to_svg.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2129 2023-05-23 18:54:45.000000 chemfunc-1.0.1/chemfunc/utils.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2514 2023-05-23 23:24:43.000000 chemfunc-1.0.1/chemfunc/visualize_molecules.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2141 2023-05-23 21:10:47.000000 chemfunc-1.0.1/chemfunc/visualize_reactions.py
+drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-06-01 18:58:04.023175 chemfunc-1.0.1/chemfunc.egg-info/
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     6386 2023-06-01 18:58:03.000000 chemfunc-1.0.1/chemfunc.egg-info/PKG-INFO
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      974 2023-06-01 18:58:03.000000 chemfunc-1.0.1/chemfunc.egg-info/SOURCES.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)        1 2023-06-01 18:58:03.000000 chemfunc-1.0.1/chemfunc.egg-info/dependency_links.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)       48 2023-06-01 18:58:03.000000 chemfunc-1.0.1/chemfunc.egg-info/entry_points.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)       93 2023-06-01 18:58:03.000000 chemfunc-1.0.1/chemfunc.egg-info/requires.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)        9 2023-06-01 18:58:03.000000 chemfunc-1.0.1/chemfunc.egg-info/top_level.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)       79 2023-06-01 18:58:04.024853 chemfunc-1.0.1/setup.cfg
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1612 2023-05-23 23:24:43.000000 chemfunc-1.0.1/setup.py
```

### Comparing `chemfunc-1.0.0/LICENSE` & `chemfunc-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.0/PKG-INFO` & `chemfunc-1.0.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chemfunc
-Version: 1.0.0
+Version: 1.0.1
 Summary: Chem Func
 Home-page: https://github.com/swansonk14/chemfunc
-Download-URL: https://github.com/swansonk14/chemfunc/v_1.0.0.tar.gz
+Download-URL: https://github.com/swansonk14/chemfunc/v_1.0.1.tar.gz
 Author: Kyle Swanson
 Author-email: swansonk.14@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/swansonk14/chemfunc
 Project-URL: PyPi, https://pypi.org/project/chemfunc/
 Keywords: computational chemistry
 Classifier: Programming Language :: Python :: 3
@@ -21,26 +21,38 @@
 
 # Chem Func
 
 Useful functions and scripts for working with small molecules.
 
 ## Installation
 
+Optionally, create a conda environment.
+```bash
+conda create -y -n chemfunc python=3.10
+conda activate chemfunc
+```
+
 Install the latest version of Chem Func using pip.
 ```
 pip install chemfunc
 ```
 
 Alternatively, clone the repository and install the local version of the package.
 ```
 git clone https://github.com/swansonk14/chemfunc.git
 cd chemfunc
 pip install -e .
 ```
 
+If there are version issues with the required packages, create a conda environment with specific working versions of the packages as follows.
+```bash
+pip install -r requirements.txt
+pip install -e .
+```
+
 
 ## Features
 
 Chem Func contains a variety of useful functions and scripts for working with small molecules.
 
 Functions can be imported from the `chemfunc` package. For example:
 ```python
@@ -65,86 +77,86 @@
 For each script, run `chemfunc <script_name> -h` to see a description of the arguments for that script.
 
 
 ## Contents
 
 Below is a list of the contents of the package.
 
-[`canonicalize_smiles.py`](chemfunc/canonicalize_smiles.py) (function, script)
+[`canonicalize_smiles.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/canonicalize_smiles.py) (function, script)
 
 Canonicalizes SMILES using RDKit canonicalization and optionally strips salts.
 
-[`chemical_diversity.py`](chemfunc/chemical_diversity.py) (function, script)
+[`chemical_diversity.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/chemical_diversity.py) (function, script)
 
 Computes the chemical diversity of a set of molecules in terms of Tanimoto distances.
 
-[`cluster_molecules.py`](chemfunc/cluster_molecules.py) (function, script)
+[`cluster_molecules.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/cluster_molecules.py) (function, script)
 
 Performs k-means clustering to cluster molecules based on Morgan fingerprints.
 
-[`compute_property_distribution.py`](chemfunc/compute_property_distribution.py) (function, script)
+[`compute_property_distribution.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/compute_property_distribution.py) (function, script)
 
 Computes one or more molecular properties for a set of molecules.
 
-[`deduplicate_smiles.py`](chemfunc/deduplicate_smiles.py) (function, script)
+[`deduplicate_smiles.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/deduplicate_smiles.py) (function, script)
 
 Deduplicate a CSV files by SMILES.
 
-[`filter_molecules.py`](chemfunc/filter_molecules.py) (function, script)
+[`filter_molecules.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/filter_molecules.py) (function, script)
 
 Filters molecules to those with values in a certain range.
 
-[`measure_experimental_reproducibility.py`](chemfunc/measure_experimental_reproducibility.py) (function, script)
+[`measure_experimental_reproducibility.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/measure_experimental_reproducibility.py) (function, script)
 
 Measures the experimental reproducibility of two biological replicates by using one replicate to predict the other.
 
-[`molecular_fingerprints.py`](chemfunc/molecular_fingerprints.py) (functions)
+[`molecular_fingerprints.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/molecular_fingerprints.py) (functions)
 
 Contains functions to compute fingerprints for molecules. Parallelized for speed.
 
-[`molecular_properties.py`](chemfunc/molecular_properties.py) (functions)
+[`molecular_properties.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/molecular_properties.py) (functions)
 
 Contains functions to compute molecular properties. Parallelized for speed.
 
-[`molecular_similarities.py`](chemfunc/molecular_similarities.py) (functions)
+[`molecular_similarities.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/molecular_similarities.py) (functions)
 
 Contains functions to compute similarities between molecules. Parallelized for speed.
 
-[`nearest_neighbor.py`](chemfunc/nearest_neighbor.py) (function, script)
+[`nearest_neighbor.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/nearest_neighbor.py) (function, script)
 
 Given a dataset of molecules, computes the nearest neighbor molecule in a second dataset using one of several similarity metrics.
 
-[`plot_property_distribution.py`](chemfunc/plot_property_distribution.py) (function, script)
+[`plot_property_distribution.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/plot_property_distribution.py) (function, script)
 
 Plots the distribution of molecular properties of a set of molecules.
 
-[`plot_tsne.py`](chemfunc/plot_tsne.py) (function, script)
+[`plot_tsne.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/plot_tsne.py) (function, script)
 
 Runs a t-SNE on molecular fingerprints from one or more chemical libraries.
 
-[`regression_to_classification.py`](chemfunc/regression_to_classification.py) (function, script)
+[`regression_to_classification.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/regression_to_classification.py) (function, script)
 
 Converts regression data to classification data using given thresholds.
 
-[`sample_molecules.py`](chemfunc/sample_molecules.py) (function, script)
+[`sample_molecules.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/sample_molecules.py) (function, script)
 
 Samples molecules from a CSV file, either uniformly at random across the entire dataset or uniformly at random from each cluster within the data.
 
-[`sdf_to_smiles.py`](chemfunc/sdf_to_smiles.py) (function, script)
+[`sdf_to_smiles.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/sdf_to_smiles.py) (function, script)
 
 Converts an SDF file to a CSV file with SMILES.
 
-[`select_from_clusters.py`](chemfunc/select_from_clusters.py) (function, script)
+[`select_from_clusters.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/select_from_clusters.py) (function, script)
 
 Selects the best molecule from each cluster.
 
-[`smiles_to_svg.py`](chemfunc/smiles_to_svg.py) (function, script)
+[`smiles_to_svg.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/smiles_to_svg.py) (function, script)
 
 Converts a SMILES string to an SVG image of the molecule.
 
-[`visualize_molecules.py`](chemfunc/visualize_molecules.py)(function, script)
+[`visualize_molecules.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/visualize_molecules.py)(function, script)
 
 Converts a file of SMILES to images of molecular structures.
 
-[`visualize_reactions.py`](chemfunc/visualize_reactions.py) (function, script)
+[`visualize_reactions.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/visualize_reactions.py) (function, script)
 
 Converts a file of reaction SMARTS to images of chemical reactions.
```

### Comparing `chemfunc-1.0.0/README.md` & `chemfunc-1.0.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,37 @@
 # Chem Func
 
 Useful functions and scripts for working with small molecules.
 
 ## Installation
 
+Optionally, create a conda environment.
+```bash
+conda create -y -n chemfunc python=3.10
+conda activate chemfunc
+```
+
 Install the latest version of Chem Func using pip.
 ```
 pip install chemfunc
 ```
 
 Alternatively, clone the repository and install the local version of the package.
 ```
 git clone https://github.com/swansonk14/chemfunc.git
 cd chemfunc
 pip install -e .
 ```
 
+If there are version issues with the required packages, create a conda environment with specific working versions of the packages as follows.
+```bash
+pip install -r requirements.txt
+pip install -e .
+```
+
 
 ## Features
 
 Chem Func contains a variety of useful functions and scripts for working with small molecules.
 
 Functions can be imported from the `chemfunc` package. For example:
 ```python
@@ -44,86 +56,86 @@
 For each script, run `chemfunc <script_name> -h` to see a description of the arguments for that script.
 
 
 ## Contents
 
 Below is a list of the contents of the package.
 
-[`canonicalize_smiles.py`](chemfunc/canonicalize_smiles.py) (function, script)
+[`canonicalize_smiles.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/canonicalize_smiles.py) (function, script)
 
 Canonicalizes SMILES using RDKit canonicalization and optionally strips salts.
 
-[`chemical_diversity.py`](chemfunc/chemical_diversity.py) (function, script)
+[`chemical_diversity.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/chemical_diversity.py) (function, script)
 
 Computes the chemical diversity of a set of molecules in terms of Tanimoto distances.
 
-[`cluster_molecules.py`](chemfunc/cluster_molecules.py) (function, script)
+[`cluster_molecules.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/cluster_molecules.py) (function, script)
 
 Performs k-means clustering to cluster molecules based on Morgan fingerprints.
 
-[`compute_property_distribution.py`](chemfunc/compute_property_distribution.py) (function, script)
+[`compute_property_distribution.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/compute_property_distribution.py) (function, script)
 
 Computes one or more molecular properties for a set of molecules.
 
-[`deduplicate_smiles.py`](chemfunc/deduplicate_smiles.py) (function, script)
+[`deduplicate_smiles.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/deduplicate_smiles.py) (function, script)
 
 Deduplicate a CSV files by SMILES.
 
-[`filter_molecules.py`](chemfunc/filter_molecules.py) (function, script)
+[`filter_molecules.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/filter_molecules.py) (function, script)
 
 Filters molecules to those with values in a certain range.
 
-[`measure_experimental_reproducibility.py`](chemfunc/measure_experimental_reproducibility.py) (function, script)
+[`measure_experimental_reproducibility.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/measure_experimental_reproducibility.py) (function, script)
 
 Measures the experimental reproducibility of two biological replicates by using one replicate to predict the other.
 
-[`molecular_fingerprints.py`](chemfunc/molecular_fingerprints.py) (functions)
+[`molecular_fingerprints.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/molecular_fingerprints.py) (functions)
 
 Contains functions to compute fingerprints for molecules. Parallelized for speed.
 
-[`molecular_properties.py`](chemfunc/molecular_properties.py) (functions)
+[`molecular_properties.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/molecular_properties.py) (functions)
 
 Contains functions to compute molecular properties. Parallelized for speed.
 
-[`molecular_similarities.py`](chemfunc/molecular_similarities.py) (functions)
+[`molecular_similarities.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/molecular_similarities.py) (functions)
 
 Contains functions to compute similarities between molecules. Parallelized for speed.
 
-[`nearest_neighbor.py`](chemfunc/nearest_neighbor.py) (function, script)
+[`nearest_neighbor.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/nearest_neighbor.py) (function, script)
 
 Given a dataset of molecules, computes the nearest neighbor molecule in a second dataset using one of several similarity metrics.
 
-[`plot_property_distribution.py`](chemfunc/plot_property_distribution.py) (function, script)
+[`plot_property_distribution.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/plot_property_distribution.py) (function, script)
 
 Plots the distribution of molecular properties of a set of molecules.
 
-[`plot_tsne.py`](chemfunc/plot_tsne.py) (function, script)
+[`plot_tsne.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/plot_tsne.py) (function, script)
 
 Runs a t-SNE on molecular fingerprints from one or more chemical libraries.
 
-[`regression_to_classification.py`](chemfunc/regression_to_classification.py) (function, script)
+[`regression_to_classification.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/regression_to_classification.py) (function, script)
 
 Converts regression data to classification data using given thresholds.
 
-[`sample_molecules.py`](chemfunc/sample_molecules.py) (function, script)
+[`sample_molecules.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/sample_molecules.py) (function, script)
 
 Samples molecules from a CSV file, either uniformly at random across the entire dataset or uniformly at random from each cluster within the data.
 
-[`sdf_to_smiles.py`](chemfunc/sdf_to_smiles.py) (function, script)
+[`sdf_to_smiles.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/sdf_to_smiles.py) (function, script)
 
 Converts an SDF file to a CSV file with SMILES.
 
-[`select_from_clusters.py`](chemfunc/select_from_clusters.py) (function, script)
+[`select_from_clusters.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/select_from_clusters.py) (function, script)
 
 Selects the best molecule from each cluster.
 
-[`smiles_to_svg.py`](chemfunc/smiles_to_svg.py) (function, script)
+[`smiles_to_svg.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/smiles_to_svg.py) (function, script)
 
 Converts a SMILES string to an SVG image of the molecule.
 
-[`visualize_molecules.py`](chemfunc/visualize_molecules.py)(function, script)
+[`visualize_molecules.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/visualize_molecules.py)(function, script)
 
 Converts a file of SMILES to images of molecular structures.
 
-[`visualize_reactions.py`](chemfunc/visualize_reactions.py) (function, script)
+[`visualize_reactions.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/visualize_reactions.py) (function, script)
 
 Converts a file of reaction SMARTS to images of chemical reactions.
```

### Comparing `chemfunc-1.0.0/chemfunc/__init__.py` & `chemfunc-1.0.1/chemfunc/__init__.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.0/chemfunc/canonicalize_smiles.py` & `chemfunc-1.0.1/chemfunc/canonicalize_smiles.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.0/chemfunc/chemical_diversity.py` & `chemfunc-1.0.1/chemfunc/chemical_diversity.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.0/chemfunc/cluster_molecules.py` & `chemfunc-1.0.1/chemfunc/cluster_molecules.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.0/chemfunc/compute_properties.py` & `chemfunc-1.0.1/chemfunc/compute_properties.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.0/chemfunc/deduplicate_smiles.py` & `chemfunc-1.0.1/chemfunc/deduplicate_smiles.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.0/chemfunc/filter_molecules.py` & `chemfunc-1.0.1/chemfunc/filter_molecules.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.0/chemfunc/main.py` & `chemfunc-1.0.1/chemfunc/main.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.0/chemfunc/measure_experimental_reproducibility.py` & `chemfunc-1.0.1/chemfunc/measure_experimental_reproducibility.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.0/chemfunc/molecular_fingerprints.py` & `chemfunc-1.0.1/chemfunc/molecular_fingerprints.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.0/chemfunc/molecular_properties.py` & `chemfunc-1.0.1/chemfunc/molecular_properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 """Contains functions to compute molecular properties."""
-import os
-import sys
 from functools import wraps
 from typing import Callable
 
 from rdkit import Chem
-from rdkit.Chem import RDConfig
 from rdkit.Chem.Crippen import MolLogP
 from rdkit.Chem.Descriptors import MolWt
 from rdkit.Chem.QED import qed
 
-sys.path.append(os.path.join(RDConfig.RDContribDir, 'SA_Score'))
-
-import sascorer
-
 from chemfunc.constants import Molecule
 
 
 PropertyFunction = Callable[[Molecule], float]
 PROPERTY_FUNCTION_REGISTRY = {}
 
 
@@ -92,16 +85,28 @@
 
     :param molecule: A molecule, either a SMILES string or an RDKit molecule.
     :return: The QED score of the molecule.
     """
     return qed(molecule)
 
 
-@register_property_function('sa_score')
-@smiles_to_mol_wrapper
-def compute_sa_score(molecule: Molecule) -> float:
-    """Computes the synthetic accessibility (SA) score of a molecule.
-
-    :param molecule: A molecule, either a SMILES string or an RDKit molecule.
-    :return: The SA score of the molecule.
-    """
-    return sascorer.calculateScore(molecule)
+try:
+    import os
+    import sys
+
+    from rdkit.Chem import RDConfig
+
+    sys.path.append(os.path.join(RDConfig.RDContribDir, 'SA_Score'))
+
+    import sascorer
+
+    @register_property_function('sa_score')
+    @smiles_to_mol_wrapper
+    def compute_sa_score(molecule: Molecule) -> float:
+        """Computes the synthetic accessibility (SA) score of a molecule.
+
+        :param molecule: A molecule, either a SMILES string or an RDKit molecule.
+        :return: The SA score of the molecule.
+        """
+        return sascorer.calculateScore(molecule)
+except ModuleNotFoundError:
+    pass
```

### Comparing `chemfunc-1.0.0/chemfunc/molecular_similarities.py` & `chemfunc-1.0.1/chemfunc/molecular_similarities.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.0/chemfunc/nearest_neighbor.py` & `chemfunc-1.0.1/chemfunc/nearest_neighbor.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.0/chemfunc/plot_property_distribution.py` & `chemfunc-1.0.1/chemfunc/plot_property_distribution.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.0/chemfunc/plot_tsne.py` & `chemfunc-1.0.1/chemfunc/plot_tsne.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.0/chemfunc/regression_to_classification.py` & `chemfunc-1.0.1/chemfunc/regression_to_classification.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.0/chemfunc/sample_molecules.py` & `chemfunc-1.0.1/chemfunc/sample_molecules.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.0/chemfunc/sdf_to_smiles.py` & `chemfunc-1.0.1/chemfunc/sdf_to_smiles.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.0/chemfunc/select_from_clusters.py` & `chemfunc-1.0.1/chemfunc/select_from_clusters.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.0/chemfunc/smiles_to_svg.py` & `chemfunc-1.0.1/chemfunc/smiles_to_svg.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.0/chemfunc/utils.py` & `chemfunc-1.0.1/chemfunc/utils.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.0/chemfunc/visualize_molecules.py` & `chemfunc-1.0.1/chemfunc/visualize_molecules.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.0/chemfunc/visualize_reactions.py` & `chemfunc-1.0.1/chemfunc/visualize_reactions.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.0/chemfunc.egg-info/PKG-INFO` & `chemfunc-1.0.1/chemfunc.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chemfunc
-Version: 1.0.0
+Version: 1.0.1
 Summary: Chem Func
 Home-page: https://github.com/swansonk14/chemfunc
-Download-URL: https://github.com/swansonk14/chemfunc/v_1.0.0.tar.gz
+Download-URL: https://github.com/swansonk14/chemfunc/v_1.0.1.tar.gz
 Author: Kyle Swanson
 Author-email: swansonk.14@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/swansonk14/chemfunc
 Project-URL: PyPi, https://pypi.org/project/chemfunc/
 Keywords: computational chemistry
 Classifier: Programming Language :: Python :: 3
@@ -21,26 +21,38 @@
 
 # Chem Func
 
 Useful functions and scripts for working with small molecules.
 
 ## Installation
 
+Optionally, create a conda environment.
+```bash
+conda create -y -n chemfunc python=3.10
+conda activate chemfunc
+```
+
 Install the latest version of Chem Func using pip.
 ```
 pip install chemfunc
 ```
 
 Alternatively, clone the repository and install the local version of the package.
 ```
 git clone https://github.com/swansonk14/chemfunc.git
 cd chemfunc
 pip install -e .
 ```
 
+If there are version issues with the required packages, create a conda environment with specific working versions of the packages as follows.
+```bash
+pip install -r requirements.txt
+pip install -e .
+```
+
 
 ## Features
 
 Chem Func contains a variety of useful functions and scripts for working with small molecules.
 
 Functions can be imported from the `chemfunc` package. For example:
 ```python
@@ -65,86 +77,86 @@
 For each script, run `chemfunc <script_name> -h` to see a description of the arguments for that script.
 
 
 ## Contents
 
 Below is a list of the contents of the package.
 
-[`canonicalize_smiles.py`](chemfunc/canonicalize_smiles.py) (function, script)
+[`canonicalize_smiles.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/canonicalize_smiles.py) (function, script)
 
 Canonicalizes SMILES using RDKit canonicalization and optionally strips salts.
 
-[`chemical_diversity.py`](chemfunc/chemical_diversity.py) (function, script)
+[`chemical_diversity.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/chemical_diversity.py) (function, script)
 
 Computes the chemical diversity of a set of molecules in terms of Tanimoto distances.
 
-[`cluster_molecules.py`](chemfunc/cluster_molecules.py) (function, script)
+[`cluster_molecules.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/cluster_molecules.py) (function, script)
 
 Performs k-means clustering to cluster molecules based on Morgan fingerprints.
 
-[`compute_property_distribution.py`](chemfunc/compute_property_distribution.py) (function, script)
+[`compute_property_distribution.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/compute_property_distribution.py) (function, script)
 
 Computes one or more molecular properties for a set of molecules.
 
-[`deduplicate_smiles.py`](chemfunc/deduplicate_smiles.py) (function, script)
+[`deduplicate_smiles.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/deduplicate_smiles.py) (function, script)
 
 Deduplicate a CSV files by SMILES.
 
-[`filter_molecules.py`](chemfunc/filter_molecules.py) (function, script)
+[`filter_molecules.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/filter_molecules.py) (function, script)
 
 Filters molecules to those with values in a certain range.
 
-[`measure_experimental_reproducibility.py`](chemfunc/measure_experimental_reproducibility.py) (function, script)
+[`measure_experimental_reproducibility.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/measure_experimental_reproducibility.py) (function, script)
 
 Measures the experimental reproducibility of two biological replicates by using one replicate to predict the other.
 
-[`molecular_fingerprints.py`](chemfunc/molecular_fingerprints.py) (functions)
+[`molecular_fingerprints.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/molecular_fingerprints.py) (functions)
 
 Contains functions to compute fingerprints for molecules. Parallelized for speed.
 
-[`molecular_properties.py`](chemfunc/molecular_properties.py) (functions)
+[`molecular_properties.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/molecular_properties.py) (functions)
 
 Contains functions to compute molecular properties. Parallelized for speed.
 
-[`molecular_similarities.py`](chemfunc/molecular_similarities.py) (functions)
+[`molecular_similarities.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/molecular_similarities.py) (functions)
 
 Contains functions to compute similarities between molecules. Parallelized for speed.
 
-[`nearest_neighbor.py`](chemfunc/nearest_neighbor.py) (function, script)
+[`nearest_neighbor.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/nearest_neighbor.py) (function, script)
 
 Given a dataset of molecules, computes the nearest neighbor molecule in a second dataset using one of several similarity metrics.
 
-[`plot_property_distribution.py`](chemfunc/plot_property_distribution.py) (function, script)
+[`plot_property_distribution.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/plot_property_distribution.py) (function, script)
 
 Plots the distribution of molecular properties of a set of molecules.
 
-[`plot_tsne.py`](chemfunc/plot_tsne.py) (function, script)
+[`plot_tsne.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/plot_tsne.py) (function, script)
 
 Runs a t-SNE on molecular fingerprints from one or more chemical libraries.
 
-[`regression_to_classification.py`](chemfunc/regression_to_classification.py) (function, script)
+[`regression_to_classification.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/regression_to_classification.py) (function, script)
 
 Converts regression data to classification data using given thresholds.
 
-[`sample_molecules.py`](chemfunc/sample_molecules.py) (function, script)
+[`sample_molecules.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/sample_molecules.py) (function, script)
 
 Samples molecules from a CSV file, either uniformly at random across the entire dataset or uniformly at random from each cluster within the data.
 
-[`sdf_to_smiles.py`](chemfunc/sdf_to_smiles.py) (function, script)
+[`sdf_to_smiles.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/sdf_to_smiles.py) (function, script)
 
 Converts an SDF file to a CSV file with SMILES.
 
-[`select_from_clusters.py`](chemfunc/select_from_clusters.py) (function, script)
+[`select_from_clusters.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/select_from_clusters.py) (function, script)
 
 Selects the best molecule from each cluster.
 
-[`smiles_to_svg.py`](chemfunc/smiles_to_svg.py) (function, script)
+[`smiles_to_svg.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/smiles_to_svg.py) (function, script)
 
 Converts a SMILES string to an SVG image of the molecule.
 
-[`visualize_molecules.py`](chemfunc/visualize_molecules.py)(function, script)
+[`visualize_molecules.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/visualize_molecules.py)(function, script)
 
 Converts a file of SMILES to images of molecular structures.
 
-[`visualize_reactions.py`](chemfunc/visualize_reactions.py) (function, script)
+[`visualize_reactions.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/visualize_reactions.py) (function, script)
 
 Converts a file of reaction SMARTS to images of chemical reactions.
```

### Comparing `chemfunc-1.0.0/chemfunc.egg-info/SOURCES.txt` & `chemfunc-1.0.1/chemfunc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.0/setup.py` & `chemfunc-1.0.1/setup.py`

 * *Files identical despite different names*

