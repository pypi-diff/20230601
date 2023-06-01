# Comparing `tmp/cheminftools-0.1.2.tar.gz` & `tmp/cheminftools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheminftools-0.1.2.tar", last modified: Tue May 30 22:14:57 2023, max compression
+gzip compressed data, was "cheminftools-0.1.3.tar", last modified: Thu Jun  1 07:47:17 2023, max compression
```

## Comparing `cheminftools-0.1.2.tar` & `cheminftools-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:14:57.882634 cheminftools-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-05-30 22:14:57.882634 cheminftools-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-05-30 22:14:40.000000 cheminftools-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:14:57.878634 cheminftools-0.1.2/cheminftools/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 22:14:40.000000 cheminftools-0.1.2/cheminftools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:14:57.882634 cheminftools-0.1.2/cheminftools/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:14:40.000000 cheminftools-0.1.2/cheminftools/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-05-30 22:14:40.000000 cheminftools-0.1.2/cheminftools/tools/featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-05-30 22:14:40.000000 cheminftools-0.1.2/cheminftools/tools/filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)    16392 2023-05-30 22:14:40.000000 cheminftools-0.1.2/cheminftools/tools/sanitizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-30 22:14:40.000000 cheminftools-0.1.2/cheminftools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:14:57.882634 cheminftools-0.1.2/cheminftools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-05-30 22:14:57.000000 cheminftools-0.1.2/cheminftools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-30 22:14:57.000000 cheminftools-0.1.2/cheminftools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 22:14:57.000000 cheminftools-0.1.2/cheminftools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 22:14:57.000000 cheminftools-0.1.2/cheminftools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-30 22:14:57.000000 cheminftools-0.1.2/cheminftools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 22:14:57.000000 cheminftools-0.1.2/cheminftools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 22:14:57.882634 cheminftools-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-30 22:14:40.000000 cheminftools-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:47:17.407322 cheminftools-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-06-01 07:47:17.407322 cheminftools-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-06-01 07:47:01.000000 cheminftools-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:47:17.403322 cheminftools-0.1.3/cheminftools/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-01 07:47:01.000000 cheminftools-0.1.3/cheminftools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:47:17.403322 cheminftools-0.1.3/cheminftools/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:47:01.000000 cheminftools-0.1.3/cheminftools/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-06-01 07:47:01.000000 cheminftools-0.1.3/cheminftools/tools/featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-06-01 07:47:01.000000 cheminftools-0.1.3/cheminftools/tools/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17757 2023-06-01 07:47:01.000000 cheminftools-0.1.3/cheminftools/tools/sanitizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-01 07:47:01.000000 cheminftools-0.1.3/cheminftools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:47:17.403322 cheminftools-0.1.3/cheminftools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-06-01 07:47:17.000000 cheminftools-0.1.3/cheminftools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-01 07:47:17.000000 cheminftools-0.1.3/cheminftools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 07:47:17.000000 cheminftools-0.1.3/cheminftools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 07:47:17.000000 cheminftools-0.1.3/cheminftools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-01 07:47:17.000000 cheminftools-0.1.3/cheminftools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-01 07:47:17.000000 cheminftools-0.1.3/cheminftools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 07:47:17.407322 cheminftools-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-01 07:47:01.000000 cheminftools-0.1.3/setup.py
```

### Comparing `cheminftools-0.1.2/PKG-INFO` & `cheminftools-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheminftools
-Version: 0.1.2
+Version: 0.1.3
 Summary: A collection of tools for daily cheminformatics tasks.
 Home-page: https://github.com/marcossantanaioc/cheminftools
 Author: marcossantanaioc
 Author-email: marcosvssantana@gmail.com
 License: Apache Software License 2.0
 Keywords: cheminformatics computational chemistry rdkit
 Classifier: Development Status :: 4 - Beta
@@ -36,39 +36,37 @@
 Chemtools offer a collection of cheminformatics scripts for daily tasks.
 Currently supported tasks include:
 
     1 - Standardization of chemical structures
 
     2 - Calculation of molecular descriptors
 
-    3 - Filtering datasets using predefined alerts (e.g. PAINS, Dundee, Glaxo, etc.)
+    3 - Filtering datasets your own or predefined alerts (e.g. PAINS, Dundee, Glaxo, etc.)
 
 # Standardization
 
-A dataset of molecules can be standardize in just 1 line of code!
+A dataset of molecules can be standardized in just 1 line of code!
 
 ``` python
 import pandas as pd
 import numpy as np
-from chemtools.tools.sanitizer import MolCleaner
-from chemtools.tools.featurizer import MolFeaturizer
-from chemtools.tools.filtering import MolFiltering
+from cheminftools.tools.sanitizer import MolCleaner
+from cheminftools.tools.featurizer import MolFeaturizer
+from cheminftools.tools.filtering import MolFilter
 from rdkit import Chem
 import json
 ```
 
 ``` python
 data = pd.read_csv('../data/example_data.csv')
 ```
 
 # Sanitizing
 
-The
-[`MolCleaner`](https://marcossantanaioc.github.io/cheminftools/sanitizer.html#molcleaner)
-class performs sanitization tasks, including:
+The `MolCleaner` class performs sanitization tasks, including:
 
         1. Standardize unknown stereochemistry (Handled by the RDKit Mol file parser)
             i) Fix wiggly bonds on sp3 carbons - sets atoms and bonds marked as unknown stereo to no stereo
             ii) Fix wiggly bonds on double bonds – set double bond to crossed bond
         2. Clears S Group data from the mol file
         3. Kekulize the structure
         4. Remove H atoms (See the page on explicit Hs for more details)
@@ -118,85 +116,72 @@
     +-------------------------------------------------------------+-------------------------------------------------------------+
     | Cc1cc2cc(Nc3ccnc4cc(-c5ccc(CNCCN6CCNCC6)cc5)sc34)ccc2[nH]1  | Cc1cc2cc(Nc3ccnc4cc(-c5ccc(CNCCN6CCNCC6)cc5)sc34)ccc2[nH]1  |
     +-------------------------------------------------------------+-------------------------------------------------------------+
 
 # Filtering
 
 The
-[`MolFiltering`](https://marcossantanaioc.github.io/chemtools/filtering.html#molfiltering)
+`MolFilter`
 class is responsible for removing compounds that match defined
-substructural alerts, including PAINS and rules defined by different
-organizations, such as GSK and University of Dundee.
-
-``` python
-with open('../data/libraries/Glaxo_alerts.json') as f:
-    alerts_dict = json.load(f)['structural_alerts']
-    structural_alerts = alerts_dict.get('structural_alerts', None)
-```
+substructural alerts. The class `AlertMatcher` can be used to generate your own catalog of alerts
+based on a dictionary. You can also use catalogs from RDKIT, such as [PAINS catalog](http://rdkit.org/docs/source/rdkit.Chem.rdfiltercatalog.html).
 
+The example below shows how to create an alerts catalog starting from a json of the Glaxos alerts.
+### Load json and prepare dictionary
 ``` python
-alerts_data = MolFiltering.from_df(processed_data, smiles_col='processed_smiles', alerts_dict=alerts_dict)
-```
-
-    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+------------------+
-    |                                  _smiles                                   |     Alert_SMARTS      |     Alert_description     |  Alert_rule_set  |   Alert_num_hits |
-    +============================================================================+=======================+===========================+==================+==================+
-    |        Cc1ncc([N+](=O)[O-])n1C/C(=N/NC(=O)c1ccc(O)cc1)c1ccc(Br)cc1         |   [N;R0][N;R0]C(=O)   |     R17 acylhydrazide     |      Glaxo       |                1 |
-    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+------------------+
-    |               O=NN(CCCl)C(=O)Nc1ccc2ncnc(Nc3cccc(Cl)c3)c2c1                | [Br,Cl,I][CX4;CH,CH2] | R1 Reactive alkyl halides |      Glaxo       |                1 |
-    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+------------------+
-    |               O=NN(CCCl)C(=O)Nc1ccc2ncnc(Nc3cccc(Cl)c3)c2c1                |   [N;R0][N;R0]C(=O)   |     R17 acylhydrazide     |      Glaxo       |                1 |
-    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+------------------+
-    |               O=NN(CCCl)C(=O)Nc1ccc2ncnc(Nc3cccc(Cl)c3)c2c1                |      [N&D2](=O)       |        R21 Nitroso        |      Glaxo       |                1 |
-    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+------------------+
-    | CS(=O)(=O)O[C@H]1CN[C@H](C#Cc2cc3ncnc(Nc4ccc(OCc5cccc(F)c5)c(Cl)c4)c3s2)C1 |   COS(=O)(=O)[C,c]    |      R5 Sulphonates       |      Glaxo       |                1 |
-    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+------------------+
-
-#### Quinone
-
-``` python
-mol = Chem.MolFromSmiles('COC1/C=C\OC2(C)Oc3c(C)c(O)c4c(c3C2=O)C(=O)C=C(NC(=O)/C(C)=C\C=C/C(C)C(O)C(C)C(O)C(C)C(OC(C)=O)C1C)C4=O')
-mol.GetSubstructMatches(Chem.MolFromSmarts('O=C1[#6]~[#6]C(=O)[#6]~[#6]1'))
-mol
-```
-
-![](index_files/figure-commonmark/cell-10-output-1.png)
+alerts_df = pd.read_csv('../data/libraries/alert_collection.csv')
+alerts_df = alerts_df[alerts_df['rule_set_name']=='Glaxo']
+alerts_df.rename(columns={'smarts':'SMARTS'},inplace=True)
+alerts_df_reindex = alerts_df[['description','SMARTS','rule_set_name','priority','max_matches']].set_index('description')
+alerts_dict = alerts_df_reindex.to_dict(orient='index')
+
+```
+### Create matcher object from dict
+``` python
+matcher = AlertMatcher(alerts_dict)
+catalog = matcher.create_matcher()
+```
+### Run filtering
+``` python
+alerts_data = MolFilter.from_df(df=processed_data, smiles_column='processed_smiles', catalog=catalog)
+```
+
+    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+
+    |                                  smiles                                    |         SMARTS        |          alert_name       |   rule_set_name  |
+    +============================================================================+=======================+===========================+==================+
+    |        Cc1ncc([N+](=O)[O-])n1C/C(=N/NC(=O)c1ccc(O)cc1)c1ccc(Br)cc1         |   [N;R0][N;R0]C(=O)   |     R17 acylhydrazide     |      Glaxo       |
+    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+
+    |               O=NN(CCCl)C(=O)Nc1ccc2ncnc(Nc3cccc(Cl)c3)c2c1                | [Br,Cl,I][CX4;CH,CH2] | R1 Reactive alkyl halides |      Glaxo       |
+    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+
+    |               O=NN(CCCl)C(=O)Nc1ccc2ncnc(Nc3cccc(Cl)c3)c2c1                |   [N;R0][N;R0]C(=O)   |     R17 acylhydrazide     |      Glaxo       |
+    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+
+    |               O=NN(CCCl)C(=O)Nc1ccc2ncnc(Nc3cccc(Cl)c3)c2c1                |      [N&D2](=O)       |        R21 Nitroso        |      Glaxo       |
+    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+
+    | CS(=O)(=O)O[C@H]1CN[C@H](C#Cc2cc3ncnc(Nc4ccc(OCc5cccc(F)c5)c(Cl)c4)c3s2)C1 |   COS(=O)(=O)[C,c]    |      R5 Sulphonates       |      Glaxo       |
+    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+
 
-#### Cynamide
-
-``` python
-mol1 = Chem.MolFromSmiles('Cc1cccc(C[C@H](NC(=O)c2cc(C(C)(C)C)nn2C)C(=O)NCC#N)c1')
-mol1.GetSubstructMatches(Chem.MolFromSmarts('N[CH2]C#N'))
-mol1
-```
-
-![](index_files/figure-commonmark/cell-11-output-1.png)
-
-#### R18 Quaternary C, Cl, I, P or S
-
-``` python
-mol = Chem.MolFromSmiles('CC[C@H](NC(=O)c1c([S+](C)[O-])c(-c2ccccc2)nc2ccccc12)c1ccccc1')
-mol.GetSubstructMatches(Chem.MolFromSmarts('[C+,Cl+,I+,P+,S+]'))
-mol
-```
-
-![](index_files/figure-commonmark/cell-12-output-1.png)
 
 # Featurization
 
 The
-[`MolFeaturizer`](https://marcossantanaioc.github.io/chemtools/featurizer.html#molfeaturizer)
+`MolFeaturizer`
 class converts SMILES into molecular descriptors. The current version
 supports Morgan fingerprints, Atom Pairs, Torsion Fingerprints, RDKit
 fingerprints and 200 constitutional descriptors, and MACCS keys.
 
 ``` python
 fingerprinter = MolFeaturizer('rdkit2d')
 ```
 
 ``` python
-X = fingerprinter.process_smiles_list(processed_data['processed_smiles'].values)
+X = fingerprinter.transform(processed_data['processed_smiles'])
 ```
 
 ``` python
-X[0:5,0:5]
+X[:5, :5]
+array([[0, 0, 0, 0, 0],
+       [0, 0, 0, 0, 0],
+       [0, 0, 0, 0, 0],
+       [0, 0, 0, 0, 0],
+       [0, 0, 0, 0, 0]], dtype=uint8)
+
 ```
```

### Comparing `cheminftools-0.1.2/README.md` & `cheminftools-0.1.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -17,39 +17,37 @@
 Chemtools offer a collection of cheminformatics scripts for daily tasks.
 Currently supported tasks include:
 
     1 - Standardization of chemical structures
 
     2 - Calculation of molecular descriptors
 
-    3 - Filtering datasets using predefined alerts (e.g. PAINS, Dundee, Glaxo, etc.)
+    3 - Filtering datasets your own or predefined alerts (e.g. PAINS, Dundee, Glaxo, etc.)
 
 # Standardization
 
-A dataset of molecules can be standardize in just 1 line of code!
+A dataset of molecules can be standardized in just 1 line of code!
 
 ``` python
 import pandas as pd
 import numpy as np
-from chemtools.tools.sanitizer import MolCleaner
-from chemtools.tools.featurizer import MolFeaturizer
-from chemtools.tools.filtering import MolFiltering
+from cheminftools.tools.sanitizer import MolCleaner
+from cheminftools.tools.featurizer import MolFeaturizer
+from cheminftools.tools.filtering import MolFilter
 from rdkit import Chem
 import json
 ```
 
 ``` python
 data = pd.read_csv('../data/example_data.csv')
 ```
 
 # Sanitizing
 
-The
-[`MolCleaner`](https://marcossantanaioc.github.io/cheminftools/sanitizer.html#molcleaner)
-class performs sanitization tasks, including:
+The `MolCleaner` class performs sanitization tasks, including:
 
         1. Standardize unknown stereochemistry (Handled by the RDKit Mol file parser)
             i) Fix wiggly bonds on sp3 carbons - sets atoms and bonds marked as unknown stereo to no stereo
             ii) Fix wiggly bonds on double bonds – set double bond to crossed bond
         2. Clears S Group data from the mol file
         3. Kekulize the structure
         4. Remove H atoms (See the page on explicit Hs for more details)
@@ -99,85 +97,72 @@
     +-------------------------------------------------------------+-------------------------------------------------------------+
     | Cc1cc2cc(Nc3ccnc4cc(-c5ccc(CNCCN6CCNCC6)cc5)sc34)ccc2[nH]1  | Cc1cc2cc(Nc3ccnc4cc(-c5ccc(CNCCN6CCNCC6)cc5)sc34)ccc2[nH]1  |
     +-------------------------------------------------------------+-------------------------------------------------------------+
 
 # Filtering
 
 The
-[`MolFiltering`](https://marcossantanaioc.github.io/chemtools/filtering.html#molfiltering)
+`MolFilter`
 class is responsible for removing compounds that match defined
-substructural alerts, including PAINS and rules defined by different
-organizations, such as GSK and University of Dundee.
-
-``` python
-with open('../data/libraries/Glaxo_alerts.json') as f:
-    alerts_dict = json.load(f)['structural_alerts']
-    structural_alerts = alerts_dict.get('structural_alerts', None)
-```
+substructural alerts. The class `AlertMatcher` can be used to generate your own catalog of alerts
+based on a dictionary. You can also use catalogs from RDKIT, such as [PAINS catalog](http://rdkit.org/docs/source/rdkit.Chem.rdfiltercatalog.html).
 
+The example below shows how to create an alerts catalog starting from a json of the Glaxos alerts.
+### Load json and prepare dictionary
 ``` python
-alerts_data = MolFiltering.from_df(processed_data, smiles_col='processed_smiles', alerts_dict=alerts_dict)
-```
-
-    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+------------------+
-    |                                  _smiles                                   |     Alert_SMARTS      |     Alert_description     |  Alert_rule_set  |   Alert_num_hits |
-    +============================================================================+=======================+===========================+==================+==================+
-    |        Cc1ncc([N+](=O)[O-])n1C/C(=N/NC(=O)c1ccc(O)cc1)c1ccc(Br)cc1         |   [N;R0][N;R0]C(=O)   |     R17 acylhydrazide     |      Glaxo       |                1 |
-    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+------------------+
-    |               O=NN(CCCl)C(=O)Nc1ccc2ncnc(Nc3cccc(Cl)c3)c2c1                | [Br,Cl,I][CX4;CH,CH2] | R1 Reactive alkyl halides |      Glaxo       |                1 |
-    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+------------------+
-    |               O=NN(CCCl)C(=O)Nc1ccc2ncnc(Nc3cccc(Cl)c3)c2c1                |   [N;R0][N;R0]C(=O)   |     R17 acylhydrazide     |      Glaxo       |                1 |
-    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+------------------+
-    |               O=NN(CCCl)C(=O)Nc1ccc2ncnc(Nc3cccc(Cl)c3)c2c1                |      [N&D2](=O)       |        R21 Nitroso        |      Glaxo       |                1 |
-    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+------------------+
-    | CS(=O)(=O)O[C@H]1CN[C@H](C#Cc2cc3ncnc(Nc4ccc(OCc5cccc(F)c5)c(Cl)c4)c3s2)C1 |   COS(=O)(=O)[C,c]    |      R5 Sulphonates       |      Glaxo       |                1 |
-    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+------------------+
-
-#### Quinone
-
-``` python
-mol = Chem.MolFromSmiles('COC1/C=C\OC2(C)Oc3c(C)c(O)c4c(c3C2=O)C(=O)C=C(NC(=O)/C(C)=C\C=C/C(C)C(O)C(C)C(O)C(C)C(OC(C)=O)C1C)C4=O')
-mol.GetSubstructMatches(Chem.MolFromSmarts('O=C1[#6]~[#6]C(=O)[#6]~[#6]1'))
-mol
-```
-
-![](index_files/figure-commonmark/cell-10-output-1.png)
+alerts_df = pd.read_csv('../data/libraries/alert_collection.csv')
+alerts_df = alerts_df[alerts_df['rule_set_name']=='Glaxo']
+alerts_df.rename(columns={'smarts':'SMARTS'},inplace=True)
+alerts_df_reindex = alerts_df[['description','SMARTS','rule_set_name','priority','max_matches']].set_index('description')
+alerts_dict = alerts_df_reindex.to_dict(orient='index')
+
+```
+### Create matcher object from dict
+``` python
+matcher = AlertMatcher(alerts_dict)
+catalog = matcher.create_matcher()
+```
+### Run filtering
+``` python
+alerts_data = MolFilter.from_df(df=processed_data, smiles_column='processed_smiles', catalog=catalog)
+```
+
+    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+
+    |                                  smiles                                    |         SMARTS        |          alert_name       |   rule_set_name  |
+    +============================================================================+=======================+===========================+==================+
+    |        Cc1ncc([N+](=O)[O-])n1C/C(=N/NC(=O)c1ccc(O)cc1)c1ccc(Br)cc1         |   [N;R0][N;R0]C(=O)   |     R17 acylhydrazide     |      Glaxo       |
+    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+
+    |               O=NN(CCCl)C(=O)Nc1ccc2ncnc(Nc3cccc(Cl)c3)c2c1                | [Br,Cl,I][CX4;CH,CH2] | R1 Reactive alkyl halides |      Glaxo       |
+    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+
+    |               O=NN(CCCl)C(=O)Nc1ccc2ncnc(Nc3cccc(Cl)c3)c2c1                |   [N;R0][N;R0]C(=O)   |     R17 acylhydrazide     |      Glaxo       |
+    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+
+    |               O=NN(CCCl)C(=O)Nc1ccc2ncnc(Nc3cccc(Cl)c3)c2c1                |      [N&D2](=O)       |        R21 Nitroso        |      Glaxo       |
+    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+
+    | CS(=O)(=O)O[C@H]1CN[C@H](C#Cc2cc3ncnc(Nc4ccc(OCc5cccc(F)c5)c(Cl)c4)c3s2)C1 |   COS(=O)(=O)[C,c]    |      R5 Sulphonates       |      Glaxo       |
+    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+
 
-#### Cynamide
-
-``` python
-mol1 = Chem.MolFromSmiles('Cc1cccc(C[C@H](NC(=O)c2cc(C(C)(C)C)nn2C)C(=O)NCC#N)c1')
-mol1.GetSubstructMatches(Chem.MolFromSmarts('N[CH2]C#N'))
-mol1
-```
-
-![](index_files/figure-commonmark/cell-11-output-1.png)
-
-#### R18 Quaternary C, Cl, I, P or S
-
-``` python
-mol = Chem.MolFromSmiles('CC[C@H](NC(=O)c1c([S+](C)[O-])c(-c2ccccc2)nc2ccccc12)c1ccccc1')
-mol.GetSubstructMatches(Chem.MolFromSmarts('[C+,Cl+,I+,P+,S+]'))
-mol
-```
-
-![](index_files/figure-commonmark/cell-12-output-1.png)
 
 # Featurization
 
 The
-[`MolFeaturizer`](https://marcossantanaioc.github.io/chemtools/featurizer.html#molfeaturizer)
+`MolFeaturizer`
 class converts SMILES into molecular descriptors. The current version
 supports Morgan fingerprints, Atom Pairs, Torsion Fingerprints, RDKit
 fingerprints and 200 constitutional descriptors, and MACCS keys.
 
 ``` python
 fingerprinter = MolFeaturizer('rdkit2d')
 ```
 
 ``` python
-X = fingerprinter.process_smiles_list(processed_data['processed_smiles'].values)
+X = fingerprinter.transform(processed_data['processed_smiles'])
 ```
 
 ``` python
-X[0:5,0:5]
+X[:5, :5]
+array([[0, 0, 0, 0, 0],
+       [0, 0, 0, 0, 0],
+       [0, 0, 0, 0, 0],
+       [0, 0, 0, 0, 0],
+       [0, 0, 0, 0, 0]], dtype=uint8)
+
 ```
```

### Comparing `cheminftools-0.1.2/cheminftools/tools/featurizer.py` & `cheminftools-0.1.3/cheminftools/tools/featurizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 __all__ = ['MolFeaturizer']
 
 import numpy as np
 from rdkit import Chem
 from ctypes import ArgumentError
 from cheminftools.utils import convert_smiles
 from rdkit.Chem import MACCSkeys, rdFingerprintGenerator, Descriptors
+from rdkit.Chem.rdReducedGraphs import GetErGFingerprint
 from rdkit.DataStructs.cDataStructs import ConvertToNumpyArray
 from functools import partial
 from typing import List
 from tqdm import tqdm
 
 
 class MolFeaturizer:
@@ -34,15 +35,16 @@
         self.descriptor_type = descriptor_type
 
         self.DESCS = {'morgan': rdFingerprintGenerator.GetMorganGenerator,
                       'atom_pairs': rdFingerprintGenerator.GetAtomPairGenerator,
                       'rdkit': rdFingerprintGenerator.GetRDKitFPGenerator,
                       'rdkit2d': self.get_rdkit2d_descriptors,
                       'torsion': rdFingerprintGenerator.GetTopologicalTorsionGenerator,
-                      'maccs': MACCSkeys.GenMACCSKeys}
+                      'maccs': MACCSkeys.GenMACCSKeys,
+                      'erg': GetErGFingerprint}
 
         self.RDKIT_PROPERTIES = ['BalabanJ', 'BertzCT', 'Chi0', 'Chi0n', 'Chi0v', 'Chi1', 'Chi1n',
                                  'Chi1v', 'Chi2n', 'Chi2v', 'Chi3n', 'Chi3v', 'Chi4n', 'Chi4v',
                                  'EState_VSA1', 'EState_VSA10', 'EState_VSA11', 'EState_VSA2',
                                  'EState_VSA3', 'EState_VSA4', 'EState_VSA5', 'EState_VSA6',
                                  'EState_VSA7', 'EState_VSA8', 'EState_VSA9', 'ExactMolWt',
                                  'FractionCSP3', 'HallKierAlpha', 'HeavyAtomCount',
@@ -104,24 +106,26 @@
 
         """
         mol = convert_smiles(smi, sanitize=True)
 
         if not mol:
             return None
 
+        if self.descriptor_type == 'erg':
+            return self.generator(mol)
+
         if self.descriptor_type == 'maccs':
             fps = np.array([])
             ConvertToNumpyArray(self.generator(mol), fps)
             return fps.reshape(1, -1)
 
         elif self.descriptor_type == 'rdkit2d':
             return self.generator(mol)
 
         else:
-
             if use_counts:
                 fps = self.generator.GetCountFingerprintAsNumPy(mol)
                 return fps.reshape(1, -1)
 
             fps = self.generator.GetFingerprintAsNumPy(mol)
             return fps.reshape(1, -1)
```

### Comparing `cheminftools-0.1.2/cheminftools/tools/filtering.py` & `cheminftools-0.1.3/cheminftools/tools/filtering.py`

 * *Files identical despite different names*

### Comparing `cheminftools-0.1.2/cheminftools/tools/sanitizer.py` & `cheminftools-0.1.3/cheminftools/tools/sanitizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 __all__ = ['mol_to_inchi', 'add_nitrogen_charges',
            'remove_unwanted', 'normalize_mol', 'get_stereo_info',
            'process_duplicates', 'MolCleaner']
 
 from typing import List, Union
+import re
 import numpy as np
 import pandas as pd
 from rdkit import Chem
 from rdkit import RDLogger
 from rdkit.Chem.MolStandardize import rdMolStandardize
 from rdkit.Chem.rdchem import Atom
 from cheminftools.utils import MolBatcher, convert_smiles, get_delta_act
@@ -21,14 +22,36 @@
 
 _allowed_atoms = [Atom(i) for i in
                   [1, 3, 4, 5, 6, 7, 8, 9, 11, 12, 13, 15, 16, 17, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31,
                    35, 37, 38, 39, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50, 53, 55, 56, 72, 73, 74, 75, 76, 77, 78,
                    79, 80, 81, 82, 83, 84, 87, 88]]
 
 
+def check_stereo(smi):
+    """
+    Check if a SMILES
+    has any stereo marks
+    such as @ or double bonds.
+    Parameters
+    ----------
+    smi
+        a SMILES string
+    Returns
+    -------
+        a boolean indicating whether `smi` has or not stereo marks.
+    """
+    smi = str(smi)
+    double_bond_patt = r'[\\\/]'
+    r_s_patt = '@'
+
+    patt = re.compile('|'.join([double_bond_patt, r_s_patt]))
+    out = bool(re.search(patt, smi))
+    return out
+
+
 def get_stereo_info(mol: Union[Chem.Mol, str]):
     """
     Return the stereo information on a given molecule.
     Stereo information includes CIS/TRANS, E/Z, R/S isomerism info
     for each bond in a molecule.
 
     Parameters
@@ -212,15 +235,14 @@
 
 
 def process_duplicates(data: pd.DataFrame,
                        smiles_column: str,
                        act_column: str,
                        cols_to_check: List[str],
                        keep: str = 'first'):
-
     """
     Aggregates duplicates in a dataset.
     It is usually enough to look for duplicates by
     grouping on standardized SMILES or InChiKeys.
     However, in cases where there's a racemic mixture and
     defined isomers present, the standard deduplication
     procedure will return separate entries. When these
@@ -264,18 +286,28 @@
 
     """
     assert keep in ['first', 'last']
     data = data.copy()
 
     # Generate inchikeys and stereo info
     logger.info(f'Converting {smiles_column} into inchikeys.')
-    data['inchikey'] = data[smiles_column].progress_apply(mol_to_inchi)
+    data['smiles_no_isomeric'] = data[smiles_column].progress_apply(
+        lambda x: Chem.MolToSmiles(Chem.MolFromSmiles(x), isomericSmiles=False))
+    data['inchikey'] = data['smiles_no_isomeric'].progress_apply(mol_to_inchi)
     data['Stereo'] = data[smiles_column].progress_apply(lambda x: get_stereo_info(x))
 
-    c = [smiles_column] + cols_to_check
+    # Remove SMILES without stereo information IF a similar SMILES has stereo info
+    # This is the case when unspecified and isolated isomers are present in the dataset
+
+    data['has_stereo_mark'] = data[smiles_column].apply(check_stereo)  # Find
+    data['group_size'] = data.groupby('inchikey')[smiles_column].transform('count')
+    data = data.drop(data[(data['has_stereo_mark'] == False) & (data['group_size'] > 1)].index)
+    data.reset_index(drop=True, inplace=True)
+
+    c = ['inchikey'] + cols_to_check
 
     # Get potential duplicates
     data['duplicated'] = data.groupby(c)[act_column].transform(get_delta_act)
 
     to_keep = data[data['duplicated'] == 'to_keep']
     to_merge = data[data['duplicated'] == 'to_merge']
     no_duplicates = data[~data['duplicated'].isin(['to_merge', 'to_keep'])]
@@ -295,35 +327,39 @@
 
     # Collect results
     results = []
 
     if not to_merge.empty:
         logger.info(f'Merging potential duplicates - '
                     f'This is usually caused by isomers with undefined chiral centers or E/Z information on SMILES.')
-
-        merged = to_merge.groupby(c).agg({'inchikey': lambda x: x[0],
-                                          'Stereo': lambda x: x[0],
-                                          act_column: 'median',
-                                          'duplicated': lambda x: x[0]})
+        cols = to_merge.columns
+        aggs = {c: lambda x: x[0] for c in cols}  # Aggregate and get first entry on each group.
+        aggs[act_column] = 'median'  # Take median of activity column.
+        merged = to_merge.groupby(c).agg(aggs)
 
         logger.info(f'Number of duplicates merged: {len(merged)} out of {len(to_merge)}.')
         results.append(merged)
 
     if not to_keep.empty and keep == 'first':
         logger.info(f'Check which duplicates should be kept -'
                     f' This usually happens with isomers with very different activities.')
 
-        duplis_kept = to_keep.groupby(smiles_column, group_keys=False).apply(
+        duplis_kept = to_keep.groupby('inchikey', group_keys=False).apply(
             lambda x: x.loc[x[act_column].idxmax()]).copy().reset_index(drop=True)
+        duplis_kept.reset_index(drop=True, inplace=True)
+        results.append(duplis_kept)
+
+    elif not to_keep.empty and keep == 'last':
+        duplis_kept = to_keep.groupby('inchikey', group_keys=False).apply(
+            lambda x: x.loc[x[act_column].idxmin()]).copy().reset_index(drop=True)
 
         duplis_kept.reset_index(drop=True, inplace=True)
         results.append(duplis_kept)
 
     # Recombine data
-
     recombined_data = pd.concat([no_duplicates, *results], axis=0, ignore_index=True)
     logger.info(f'Duplicates removal reduced the number of rows from {len(data)} to {len(recombined_data)}')
     recombined_data.reset_index(drop=True, inplace=True)
 
     return recombined_data
```

### Comparing `cheminftools-0.1.2/cheminftools/utils.py` & `cheminftools-0.1.3/cheminftools/utils.py`

 * *Files identical despite different names*

### Comparing `cheminftools-0.1.2/cheminftools.egg-info/PKG-INFO` & `cheminftools-0.1.3/cheminftools.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheminftools
-Version: 0.1.2
+Version: 0.1.3
 Summary: A collection of tools for daily cheminformatics tasks.
 Home-page: https://github.com/marcossantanaioc/cheminftools
 Author: marcossantanaioc
 Author-email: marcosvssantana@gmail.com
 License: Apache Software License 2.0
 Keywords: cheminformatics computational chemistry rdkit
 Classifier: Development Status :: 4 - Beta
@@ -36,39 +36,37 @@
 Chemtools offer a collection of cheminformatics scripts for daily tasks.
 Currently supported tasks include:
 
     1 - Standardization of chemical structures
 
     2 - Calculation of molecular descriptors
 
-    3 - Filtering datasets using predefined alerts (e.g. PAINS, Dundee, Glaxo, etc.)
+    3 - Filtering datasets your own or predefined alerts (e.g. PAINS, Dundee, Glaxo, etc.)
 
 # Standardization
 
-A dataset of molecules can be standardize in just 1 line of code!
+A dataset of molecules can be standardized in just 1 line of code!
 
 ``` python
 import pandas as pd
 import numpy as np
-from chemtools.tools.sanitizer import MolCleaner
-from chemtools.tools.featurizer import MolFeaturizer
-from chemtools.tools.filtering import MolFiltering
+from cheminftools.tools.sanitizer import MolCleaner
+from cheminftools.tools.featurizer import MolFeaturizer
+from cheminftools.tools.filtering import MolFilter
 from rdkit import Chem
 import json
 ```
 
 ``` python
 data = pd.read_csv('../data/example_data.csv')
 ```
 
 # Sanitizing
 
-The
-[`MolCleaner`](https://marcossantanaioc.github.io/cheminftools/sanitizer.html#molcleaner)
-class performs sanitization tasks, including:
+The `MolCleaner` class performs sanitization tasks, including:
 
         1. Standardize unknown stereochemistry (Handled by the RDKit Mol file parser)
             i) Fix wiggly bonds on sp3 carbons - sets atoms and bonds marked as unknown stereo to no stereo
             ii) Fix wiggly bonds on double bonds – set double bond to crossed bond
         2. Clears S Group data from the mol file
         3. Kekulize the structure
         4. Remove H atoms (See the page on explicit Hs for more details)
@@ -118,85 +116,72 @@
     +-------------------------------------------------------------+-------------------------------------------------------------+
     | Cc1cc2cc(Nc3ccnc4cc(-c5ccc(CNCCN6CCNCC6)cc5)sc34)ccc2[nH]1  | Cc1cc2cc(Nc3ccnc4cc(-c5ccc(CNCCN6CCNCC6)cc5)sc34)ccc2[nH]1  |
     +-------------------------------------------------------------+-------------------------------------------------------------+
 
 # Filtering
 
 The
-[`MolFiltering`](https://marcossantanaioc.github.io/chemtools/filtering.html#molfiltering)
+`MolFilter`
 class is responsible for removing compounds that match defined
-substructural alerts, including PAINS and rules defined by different
-organizations, such as GSK and University of Dundee.
-
-``` python
-with open('../data/libraries/Glaxo_alerts.json') as f:
-    alerts_dict = json.load(f)['structural_alerts']
-    structural_alerts = alerts_dict.get('structural_alerts', None)
-```
+substructural alerts. The class `AlertMatcher` can be used to generate your own catalog of alerts
+based on a dictionary. You can also use catalogs from RDKIT, such as [PAINS catalog](http://rdkit.org/docs/source/rdkit.Chem.rdfiltercatalog.html).
 
+The example below shows how to create an alerts catalog starting from a json of the Glaxos alerts.
+### Load json and prepare dictionary
 ``` python
-alerts_data = MolFiltering.from_df(processed_data, smiles_col='processed_smiles', alerts_dict=alerts_dict)
-```
-
-    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+------------------+
-    |                                  _smiles                                   |     Alert_SMARTS      |     Alert_description     |  Alert_rule_set  |   Alert_num_hits |
-    +============================================================================+=======================+===========================+==================+==================+
-    |        Cc1ncc([N+](=O)[O-])n1C/C(=N/NC(=O)c1ccc(O)cc1)c1ccc(Br)cc1         |   [N;R0][N;R0]C(=O)   |     R17 acylhydrazide     |      Glaxo       |                1 |
-    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+------------------+
-    |               O=NN(CCCl)C(=O)Nc1ccc2ncnc(Nc3cccc(Cl)c3)c2c1                | [Br,Cl,I][CX4;CH,CH2] | R1 Reactive alkyl halides |      Glaxo       |                1 |
-    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+------------------+
-    |               O=NN(CCCl)C(=O)Nc1ccc2ncnc(Nc3cccc(Cl)c3)c2c1                |   [N;R0][N;R0]C(=O)   |     R17 acylhydrazide     |      Glaxo       |                1 |
-    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+------------------+
-    |               O=NN(CCCl)C(=O)Nc1ccc2ncnc(Nc3cccc(Cl)c3)c2c1                |      [N&D2](=O)       |        R21 Nitroso        |      Glaxo       |                1 |
-    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+------------------+
-    | CS(=O)(=O)O[C@H]1CN[C@H](C#Cc2cc3ncnc(Nc4ccc(OCc5cccc(F)c5)c(Cl)c4)c3s2)C1 |   COS(=O)(=O)[C,c]    |      R5 Sulphonates       |      Glaxo       |                1 |
-    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+------------------+
-
-#### Quinone
-
-``` python
-mol = Chem.MolFromSmiles('COC1/C=C\OC2(C)Oc3c(C)c(O)c4c(c3C2=O)C(=O)C=C(NC(=O)/C(C)=C\C=C/C(C)C(O)C(C)C(O)C(C)C(OC(C)=O)C1C)C4=O')
-mol.GetSubstructMatches(Chem.MolFromSmarts('O=C1[#6]~[#6]C(=O)[#6]~[#6]1'))
-mol
-```
-
-![](index_files/figure-commonmark/cell-10-output-1.png)
+alerts_df = pd.read_csv('../data/libraries/alert_collection.csv')
+alerts_df = alerts_df[alerts_df['rule_set_name']=='Glaxo']
+alerts_df.rename(columns={'smarts':'SMARTS'},inplace=True)
+alerts_df_reindex = alerts_df[['description','SMARTS','rule_set_name','priority','max_matches']].set_index('description')
+alerts_dict = alerts_df_reindex.to_dict(orient='index')
+
+```
+### Create matcher object from dict
+``` python
+matcher = AlertMatcher(alerts_dict)
+catalog = matcher.create_matcher()
+```
+### Run filtering
+``` python
+alerts_data = MolFilter.from_df(df=processed_data, smiles_column='processed_smiles', catalog=catalog)
+```
+
+    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+
+    |                                  smiles                                    |         SMARTS        |          alert_name       |   rule_set_name  |
+    +============================================================================+=======================+===========================+==================+
+    |        Cc1ncc([N+](=O)[O-])n1C/C(=N/NC(=O)c1ccc(O)cc1)c1ccc(Br)cc1         |   [N;R0][N;R0]C(=O)   |     R17 acylhydrazide     |      Glaxo       |
+    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+
+    |               O=NN(CCCl)C(=O)Nc1ccc2ncnc(Nc3cccc(Cl)c3)c2c1                | [Br,Cl,I][CX4;CH,CH2] | R1 Reactive alkyl halides |      Glaxo       |
+    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+
+    |               O=NN(CCCl)C(=O)Nc1ccc2ncnc(Nc3cccc(Cl)c3)c2c1                |   [N;R0][N;R0]C(=O)   |     R17 acylhydrazide     |      Glaxo       |
+    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+
+    |               O=NN(CCCl)C(=O)Nc1ccc2ncnc(Nc3cccc(Cl)c3)c2c1                |      [N&D2](=O)       |        R21 Nitroso        |      Glaxo       |
+    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+
+    | CS(=O)(=O)O[C@H]1CN[C@H](C#Cc2cc3ncnc(Nc4ccc(OCc5cccc(F)c5)c(Cl)c4)c3s2)C1 |   COS(=O)(=O)[C,c]    |      R5 Sulphonates       |      Glaxo       |
+    +----------------------------------------------------------------------------+-----------------------+---------------------------+------------------+
 
-#### Cynamide
-
-``` python
-mol1 = Chem.MolFromSmiles('Cc1cccc(C[C@H](NC(=O)c2cc(C(C)(C)C)nn2C)C(=O)NCC#N)c1')
-mol1.GetSubstructMatches(Chem.MolFromSmarts('N[CH2]C#N'))
-mol1
-```
-
-![](index_files/figure-commonmark/cell-11-output-1.png)
-
-#### R18 Quaternary C, Cl, I, P or S
-
-``` python
-mol = Chem.MolFromSmiles('CC[C@H](NC(=O)c1c([S+](C)[O-])c(-c2ccccc2)nc2ccccc12)c1ccccc1')
-mol.GetSubstructMatches(Chem.MolFromSmarts('[C+,Cl+,I+,P+,S+]'))
-mol
-```
-
-![](index_files/figure-commonmark/cell-12-output-1.png)
 
 # Featurization
 
 The
-[`MolFeaturizer`](https://marcossantanaioc.github.io/chemtools/featurizer.html#molfeaturizer)
+`MolFeaturizer`
 class converts SMILES into molecular descriptors. The current version
 supports Morgan fingerprints, Atom Pairs, Torsion Fingerprints, RDKit
 fingerprints and 200 constitutional descriptors, and MACCS keys.
 
 ``` python
 fingerprinter = MolFeaturizer('rdkit2d')
 ```
 
 ``` python
-X = fingerprinter.process_smiles_list(processed_data['processed_smiles'].values)
+X = fingerprinter.transform(processed_data['processed_smiles'])
 ```
 
 ``` python
-X[0:5,0:5]
+X[:5, :5]
+array([[0, 0, 0, 0, 0],
+       [0, 0, 0, 0, 0],
+       [0, 0, 0, 0, 0],
+       [0, 0, 0, 0, 0],
+       [0, 0, 0, 0, 0]], dtype=uint8)
+
 ```
```

### Comparing `cheminftools-0.1.2/setup.py` & `cheminftools-0.1.3/setup.py`

 * *Files identical despite different names*

