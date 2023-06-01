# Comparing `tmp/crimm-2023.5a3.tar.gz` & `tmp/crimm-2023.5a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crimm-2023.5a3.tar", last modified: Tue May 23 18:36:24 2023, max compression
+gzip compressed data, was "crimm-2023.5a4.tar", last modified: Thu Jun  1 00:02:31 2023, max compression
```

## Comparing `crimm-2023.5a3.tar` & `crimm-2023.5a4.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-05-23 18:36:24.877947 crimm-2023.5a3/
--rw-r--r--   0 truman    (1000) truman    (1000)    35149 2023-05-23 16:25:01.000000 crimm-2023.5a3/LICENSE
--rw-r--r--   0 truman    (1000) truman    (1000)      127 2023-05-23 18:28:34.000000 crimm-2023.5a3/MANIFEST.in
--rw-r--r--   0 truman    (1000) truman    (1000)     2572 2023-05-23 18:36:24.877947 crimm-2023.5a3/PKG-INFO
--rw-r--r--   0 truman    (1000) truman    (1000)     1987 2023-05-23 16:36:39.000000 crimm-2023.5a3/README.md
-drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-05-23 18:36:24.870947 crimm-2023.5a3/crimm/
-drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-05-23 18:36:24.871947 crimm-2023.5a3/crimm/Adaptors/
--rw-r--r--   0 truman    (1000) truman    (1000)     4293 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/Adaptors/OMMAdaptors.py
--rw-r--r--   0 truman    (1000) truman    (1000)    10699 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/Adaptors/PropKaAdaptors.py
--rw-r--r--   0 truman    (1000) truman    (1000)     2924 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/Adaptors/RDKitAdaptor.py
--rw-r--r--   0 truman    (1000) truman    (1000)        0 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/Adaptors/__init__.py
--rw-r--r--   0 truman    (1000) truman    (1000)     4746 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/Adaptors/pyCHARMMAdaptors.py
-drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-05-23 18:36:24.871947 crimm-2023.5a3/crimm/Data/
--rw-r--r--   0 truman    (1000) truman    (1000)      528 2023-05-09 20:11:39.000000 crimm-2023.5a3/crimm/Data/connect_records.py
-drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-05-23 18:36:24.874947 crimm-2023.5a3/crimm/Data/toppar/
--rw-r--r--   0 truman    (1000) truman    (1000)   159620 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/Data/toppar/carb.prm
--rw-r--r--   0 truman    (1000) truman    (1000)   292987 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/Data/toppar/carb.rtf
--rw-r--r--   0 truman    (1000) truman    (1000)   926172 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/Data/toppar/cgenff.prm
--rw-r--r--   0 truman    (1000) truman    (1000)  2474554 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/Data/toppar/cgenff.rtf
--rw-r--r--   0 truman    (1000) truman    (1000)    18777 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/Data/toppar/ethers.prm
--rw-r--r--   0 truman    (1000) truman    (1000)    46438 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/Data/toppar/ethers.rtf
--rw-r--r--   0 truman    (1000) truman    (1000)    28988 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/Data/toppar/lipid.prm
--rw-r--r--   0 truman    (1000) truman    (1000)   635614 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/Data/toppar/lipid.rtf
--rw-r--r--   0 truman    (1000) truman    (1000)    64738 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/Data/toppar/na.prm
--rw-r--r--   0 truman    (1000) truman    (1000)    38311 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/Data/toppar/na.rtf
--rw-r--r--   0 truman    (1000) truman    (1000)    38099 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/Data/toppar/na_orig.rtf
--rw-r--r--   0 truman    (1000) truman    (1000)   180976 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/Data/toppar/prot.prm
--rw-r--r--   0 truman    (1000) truman    (1000)    73234 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/Data/toppar/prot.rtf
--rw-r--r--   0 truman    (1000) truman    (1000)    73028 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/Data/toppar/prot_orig.rtf
--rw-r--r--   0 truman    (1000) truman    (1000)     8392 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/Fetchers.py
-drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-05-23 18:36:24.875947 crimm-2023.5a3/crimm/IO/
--rw-r--r--   0 truman    (1000) truman    (1000)     3041 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/IO/MMCIF2Dict.py
--rw-r--r--   0 truman    (1000) truman    (1000)    17524 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/IO/MMCIFParser.py
--rw-r--r--   0 truman    (1000) truman    (1000)     5198 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/IO/PDBParser.py
--rw-r--r--   0 truman    (1000) truman    (1000)     5771 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/IO/PDBString.py
--rw-r--r--   0 truman    (1000) truman    (1000)     7493 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/IO/PRMParser.py
--rw-r--r--   0 truman    (1000) truman    (1000)    11457 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/IO/RTFParser.py
--rw-r--r--   0 truman    (1000) truman    (1000)    12979 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/IO/StructureBuilder.py
--rw-r--r--   0 truman    (1000) truman    (1000)      171 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/IO/__init__.py
-drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-05-23 18:36:24.876947 crimm-2023.5a3/crimm/Modeller/
--rw-r--r--   0 truman    (1000) truman    (1000)     3349 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/Modeller/CoordManipulator.py
--rw-r--r--   0 truman    (1000) truman    (1000)    19512 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/Modeller/LoopBuilder.py
--rw-r--r--   0 truman    (1000) truman    (1000)     9554 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/Modeller/ParamLoader.py
--rw-r--r--   0 truman    (1000) truman    (1000)     6606 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/Modeller/SeqChainGenerator.py
--rw-r--r--   0 truman    (1000) truman    (1000)    17604 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/Modeller/TopoFixer.py
--rw-r--r--   0 truman    (1000) truman    (1000)    31572 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/Modeller/TopoLoader.py
--rw-r--r--   0 truman    (1000) truman    (1000)      220 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/Modeller/__init__.py
-drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-05-23 18:36:24.877947 crimm-2023.5a3/crimm/StructEntities/
--rw-r--r--   0 truman    (1000) truman    (1000)     4166 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/StructEntities/Atom.py
--rw-r--r--   0 truman    (1000) truman    (1000)    15317 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/StructEntities/Chain.py
--rw-r--r--   0 truman    (1000) truman    (1000)     4869 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/StructEntities/Model.py
--rw-r--r--   0 truman    (1000) truman    (1000)     4757 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/StructEntities/Residue.py
--rw-r--r--   0 truman    (1000) truman    (1000)     2110 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/StructEntities/Structure.py
--rw-r--r--   0 truman    (1000) truman    (1000)    12795 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/StructEntities/TopoDefinitions.py
--rw-r--r--   0 truman    (1000) truman    (1000)     9163 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/StructEntities/TopoElements.py
--rw-r--r--   0 truman    (1000) truman    (1000)      691 2023-05-09 21:55:09.000000 crimm-2023.5a3/crimm/StructEntities/Topology.py
--rw-r--r--   0 truman    (1000) truman    (1000)      494 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/StructEntities/__init__.py
-drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-05-23 18:36:24.877947 crimm-2023.5a3/crimm/Superimpose/
--rw-r--r--   0 truman    (1000) truman    (1000)     9264 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/Superimpose/ChainSuperimposer.py
--rw-r--r--   0 truman    (1000) truman    (1000)       65 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/Superimpose/__init__.py
-drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-05-23 18:36:24.877947 crimm-2023.5a3/crimm/Visualization/
--rw-r--r--   0 truman    (1000) truman    (1000)     8050 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/Visualization/NGLVisualization.py
--rw-r--r--   0 truman    (1000) truman    (1000)       85 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/Visualization/__init__.py
--rw-r--r--   0 truman    (1000) truman    (1000)      283 2023-05-23 16:20:45.000000 crimm-2023.5a3/crimm/__init__.py
-drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-05-23 18:36:24.870947 crimm-2023.5a3/crimm.egg-info/
--rw-r--r--   0 truman    (1000) truman    (1000)     2572 2023-05-23 18:36:24.000000 crimm-2023.5a3/crimm.egg-info/PKG-INFO
--rw-r--r--   0 truman    (1000) truman    (1000)     1717 2023-05-23 18:36:24.000000 crimm-2023.5a3/crimm.egg-info/SOURCES.txt
--rw-r--r--   0 truman    (1000) truman    (1000)        1 2023-05-23 18:36:24.000000 crimm-2023.5a3/crimm.egg-info/dependency_links.txt
--rw-r--r--   0 truman    (1000) truman    (1000)       75 2023-05-23 18:36:24.000000 crimm-2023.5a3/crimm.egg-info/requires.txt
--rw-r--r--   0 truman    (1000) truman    (1000)        6 2023-05-23 18:36:24.000000 crimm-2023.5a3/crimm.egg-info/top_level.txt
--rw-r--r--   0 truman    (1000) truman    (1000)      954 2023-05-23 18:33:47.000000 crimm-2023.5a3/pyproject.toml
--rw-r--r--   0 truman    (1000) truman    (1000)       38 2023-05-23 18:36:24.877947 crimm-2023.5a3/setup.cfg
-drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-05-23 18:36:24.869947 crimm-2023.5a3/src/
-drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-05-23 18:36:24.877947 crimm-2023.5a3/src/chatgpt/
--rw-r--r--   0 truman    (1000) truman    (1000)     4768 2023-03-09 21:07:14.000000 crimm-2023.5a3/src/chatgpt/steepestDescent.py
-drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-05-23 18:36:24.877947 crimm-2023.5a3/tests/
--rw-r--r--   0 truman    (1000) truman    (1000)     4470 2023-03-30 02:07:51.000000 crimm-2023.5a3/tests/test_pdb.py
--rw-r--r--   0 truman    (1000) truman    (1000)     6420 2023-03-29 03:20:54.000000 crimm-2023.5a3/tests/test_pdb_standard.py
+drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-06-01 00:02:31.070154 crimm-2023.5a4/
+-rw-r--r--   0 truman    (1000) truman    (1000)    35149 2023-05-24 19:26:01.000000 crimm-2023.5a4/LICENSE
+-rw-r--r--   0 truman    (1000) truman    (1000)      127 2023-05-24 19:26:01.000000 crimm-2023.5a4/MANIFEST.in
+-rw-r--r--   0 truman    (1000) truman    (1000)     2877 2023-06-01 00:02:31.070154 crimm-2023.5a4/PKG-INFO
+-rw-r--r--   0 truman    (1000) truman    (1000)     2292 2023-05-24 19:26:01.000000 crimm-2023.5a4/README.md
+drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-06-01 00:02:31.062154 crimm-2023.5a4/crimm/
+drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-06-01 00:02:31.063154 crimm-2023.5a4/crimm/Adaptors/
+-rw-r--r--   0 truman    (1000) truman    (1000)     4293 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/Adaptors/OMMAdaptors.py
+-rw-r--r--   0 truman    (1000) truman    (1000)    11929 2023-05-31 23:39:20.000000 crimm-2023.5a4/crimm/Adaptors/PropKaAdaptors.py
+-rw-r--r--   0 truman    (1000) truman    (1000)     2924 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/Adaptors/RDKitAdaptor.py
+-rw-r--r--   0 truman    (1000) truman    (1000)        0 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/Adaptors/__init__.py
+-rw-r--r--   0 truman    (1000) truman    (1000)     4573 2023-05-31 16:59:48.000000 crimm-2023.5a4/crimm/Adaptors/pyCHARMMAdaptors.py
+drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-06-01 00:02:31.063154 crimm-2023.5a4/crimm/Data/
+-rw-r--r--   0 truman    (1000) truman    (1000)      528 2023-05-09 20:11:39.000000 crimm-2023.5a4/crimm/Data/connect_records.py
+drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-06-01 00:02:31.067154 crimm-2023.5a4/crimm/Data/toppar/
+-rw-r--r--   0 truman    (1000) truman    (1000)   159620 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/Data/toppar/carb.prm
+-rw-r--r--   0 truman    (1000) truman    (1000)   292987 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/Data/toppar/carb.rtf
+-rw-r--r--   0 truman    (1000) truman    (1000)   926172 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/Data/toppar/cgenff.prm
+-rw-r--r--   0 truman    (1000) truman    (1000)  2474554 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/Data/toppar/cgenff.rtf
+-rw-r--r--   0 truman    (1000) truman    (1000)    18777 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/Data/toppar/ethers.prm
+-rw-r--r--   0 truman    (1000) truman    (1000)    46438 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/Data/toppar/ethers.rtf
+-rw-r--r--   0 truman    (1000) truman    (1000)    28988 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/Data/toppar/lipid.prm
+-rw-r--r--   0 truman    (1000) truman    (1000)   635614 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/Data/toppar/lipid.rtf
+-rw-r--r--   0 truman    (1000) truman    (1000)    64738 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/Data/toppar/na.prm
+-rw-r--r--   0 truman    (1000) truman    (1000)    38311 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/Data/toppar/na.rtf
+-rw-r--r--   0 truman    (1000) truman    (1000)    38099 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/Data/toppar/na_orig.rtf
+-rw-r--r--   0 truman    (1000) truman    (1000)   180976 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/Data/toppar/prot.prm
+-rw-r--r--   0 truman    (1000) truman    (1000)    73234 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/Data/toppar/prot.rtf
+-rw-r--r--   0 truman    (1000) truman    (1000)    73028 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/Data/toppar/prot_orig.rtf
+-rw-r--r--   0 truman    (1000) truman    (1000)     8392 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/Fetchers.py
+drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-06-01 00:02:31.068154 crimm-2023.5a4/crimm/IO/
+-rw-r--r--   0 truman    (1000) truman    (1000)     3041 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/IO/MMCIF2Dict.py
+-rw-r--r--   0 truman    (1000) truman    (1000)    17524 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/IO/MMCIFParser.py
+-rw-r--r--   0 truman    (1000) truman    (1000)     5198 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/IO/PDBParser.py
+-rw-r--r--   0 truman    (1000) truman    (1000)     5771 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/IO/PDBString.py
+-rw-r--r--   0 truman    (1000) truman    (1000)     7493 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/IO/PRMParser.py
+-rw-r--r--   0 truman    (1000) truman    (1000)    11457 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/IO/RTFParser.py
+-rw-r--r--   0 truman    (1000) truman    (1000)    12979 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/IO/StructureBuilder.py
+-rw-r--r--   0 truman    (1000) truman    (1000)      171 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/IO/__init__.py
+drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-06-01 00:02:31.068154 crimm-2023.5a4/crimm/Modeller/
+-rw-r--r--   0 truman    (1000) truman    (1000)     3349 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/Modeller/CoordManipulator.py
+-rw-r--r--   0 truman    (1000) truman    (1000)    19512 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/Modeller/LoopBuilder.py
+-rw-r--r--   0 truman    (1000) truman    (1000)     9554 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/Modeller/ParamLoader.py
+-rw-r--r--   0 truman    (1000) truman    (1000)     6606 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/Modeller/SeqChainGenerator.py
+-rw-r--r--   0 truman    (1000) truman    (1000)    17604 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/Modeller/TopoFixer.py
+-rw-r--r--   0 truman    (1000) truman    (1000)    32180 2023-05-31 15:50:21.000000 crimm-2023.5a4/crimm/Modeller/TopoLoader.py
+-rw-r--r--   0 truman    (1000) truman    (1000)      220 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/Modeller/__init__.py
+drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-06-01 00:02:31.069154 crimm-2023.5a4/crimm/StructEntities/
+-rw-r--r--   0 truman    (1000) truman    (1000)     4166 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/StructEntities/Atom.py
+-rw-r--r--   0 truman    (1000) truman    (1000)    15317 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/StructEntities/Chain.py
+-rw-r--r--   0 truman    (1000) truman    (1000)     4869 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/StructEntities/Model.py
+-rw-r--r--   0 truman    (1000) truman    (1000)     4757 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/StructEntities/Residue.py
+-rw-r--r--   0 truman    (1000) truman    (1000)     2110 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/StructEntities/Structure.py
+-rw-r--r--   0 truman    (1000) truman    (1000)    12795 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/StructEntities/TopoDefinitions.py
+-rw-r--r--   0 truman    (1000) truman    (1000)     9163 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/StructEntities/TopoElements.py
+-rw-r--r--   0 truman    (1000) truman    (1000)      691 2023-05-09 21:55:09.000000 crimm-2023.5a4/crimm/StructEntities/Topology.py
+-rw-r--r--   0 truman    (1000) truman    (1000)      494 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/StructEntities/__init__.py
+drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-06-01 00:02:31.069154 crimm-2023.5a4/crimm/Superimpose/
+-rw-r--r--   0 truman    (1000) truman    (1000)     9264 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/Superimpose/ChainSuperimposer.py
+-rw-r--r--   0 truman    (1000) truman    (1000)       65 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/Superimpose/__init__.py
+drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-06-01 00:02:31.070154 crimm-2023.5a4/crimm/Visualization/
+-rw-r--r--   0 truman    (1000) truman    (1000)     8050 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/Visualization/NGLVisualization.py
+-rw-r--r--   0 truman    (1000) truman    (1000)       85 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/Visualization/__init__.py
+-rw-r--r--   0 truman    (1000) truman    (1000)      283 2023-05-23 16:20:45.000000 crimm-2023.5a4/crimm/__init__.py
+drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-06-01 00:02:31.062154 crimm-2023.5a4/crimm.egg-info/
+-rw-r--r--   0 truman    (1000) truman    (1000)     2877 2023-06-01 00:02:31.000000 crimm-2023.5a4/crimm.egg-info/PKG-INFO
+-rw-r--r--   0 truman    (1000) truman    (1000)     1717 2023-06-01 00:02:31.000000 crimm-2023.5a4/crimm.egg-info/SOURCES.txt
+-rw-r--r--   0 truman    (1000) truman    (1000)        1 2023-06-01 00:02:31.000000 crimm-2023.5a4/crimm.egg-info/dependency_links.txt
+-rw-r--r--   0 truman    (1000) truman    (1000)       75 2023-06-01 00:02:31.000000 crimm-2023.5a4/crimm.egg-info/requires.txt
+-rw-r--r--   0 truman    (1000) truman    (1000)        6 2023-06-01 00:02:31.000000 crimm-2023.5a4/crimm.egg-info/top_level.txt
+-rw-r--r--   0 truman    (1000) truman    (1000)      954 2023-06-01 00:02:15.000000 crimm-2023.5a4/pyproject.toml
+-rw-r--r--   0 truman    (1000) truman    (1000)       38 2023-06-01 00:02:31.070154 crimm-2023.5a4/setup.cfg
+drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-06-01 00:02:31.061154 crimm-2023.5a4/src/
+drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-06-01 00:02:31.070154 crimm-2023.5a4/src/chatgpt/
+-rw-r--r--   0 truman    (1000) truman    (1000)     4768 2023-03-09 21:07:14.000000 crimm-2023.5a4/src/chatgpt/steepestDescent.py
+drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-06-01 00:02:31.070154 crimm-2023.5a4/tests/
+-rw-r--r--   0 truman    (1000) truman    (1000)     4470 2023-03-30 02:07:51.000000 crimm-2023.5a4/tests/test_pdb.py
+-rw-r--r--   0 truman    (1000) truman    (1000)     6420 2023-03-29 03:20:54.000000 crimm-2023.5a4/tests/test_pdb_standard.py
```

### Comparing `crimm-2023.5a3/LICENSE` & `crimm-2023.5a4/LICENSE`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/PKG-INFO` & `crimm-2023.5a4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 Metadata-Version: 2.1
 Name: crimm
-Version: 2023.5a3
+Version: 2023.5a4
 Summary: Chemistry with the ReInvented Macromolecular
 Author-email: Truman Xu <ziqiaoxu@umich.edu>
 Project-URL: Homepage, https://github.com/Truman-Xu/crimm
 Project-URL: Bug Tracker, https://github.com/Truman-Xu/crimm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# **CRIMM**
-**CRIMM** stands for **Chemistry with the ReInvented Macromolecular Mechanics**. This project aims to integrate and supplement CHARMM with better object handle and APIs
+# **crimm**
+**crimm** stands for **Chemistry with the ReInvented Macromolecular Mechanics**. This project aims to integrate and supplement CHARMM with better object handle and APIs
 
 ## Why *"reinvent the wheel"*
 This is a toolkit that is under active development, where many useful macromolecular modeling routines are selected to be reimplemented. This is an attempt to unify many macromolecular preparation/modeling routine under one platform while offering proper object handles and APIs in python. While currently, we aim to integrate with CHARMM and pyCHARMM, the broader goal is to provide highly usable, integratable, and scriptable python library/platform for simplifying any macromolecular modeling pipelines.
 
+-----------------
+## Installations
+crimm can be installed by `pip install crimm`
+
+crimm requires `python>=3.10`. The main dependencies are biopython, nglview, scipy, and requests. To use the adaptors, the respective packages need to be installed separately (e.g. pyCHARMM, rdkit, etc.)
+
+-----------------
 ## Base Library and Object Handles
 This library is built upon the excellent Biopython library. The macromolecular entity representations are derived from Biopython's entity classes and follow the same hierarchy. As a result, the entities in this library remain fully compatible with all functions and routines provided in Biopython.
 ## Parser Module
 New and improved mmCIF parser is implemented to allow accurate structure representations and more complete information.
 
 ## Looper Module
 For a given PDB structure with gaps or missing loops in the chain, this module provides functions to query PDB for the residue sequence and fill in the gaps or missing loop regions with the residues coordinates from the homology models.
```

### Comparing `crimm-2023.5a3/README.md` & `crimm-2023.5a4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,20 @@
-# **CRIMM**
-**CRIMM** stands for **Chemistry with the ReInvented Macromolecular Mechanics**. This project aims to integrate and supplement CHARMM with better object handle and APIs
+# **crimm**
+**crimm** stands for **Chemistry with the ReInvented Macromolecular Mechanics**. This project aims to integrate and supplement CHARMM with better object handle and APIs
 
 ## Why *"reinvent the wheel"*
 This is a toolkit that is under active development, where many useful macromolecular modeling routines are selected to be reimplemented. This is an attempt to unify many macromolecular preparation/modeling routine under one platform while offering proper object handles and APIs in python. While currently, we aim to integrate with CHARMM and pyCHARMM, the broader goal is to provide highly usable, integratable, and scriptable python library/platform for simplifying any macromolecular modeling pipelines.
 
+-----------------
+## Installations
+crimm can be installed by `pip install crimm`
+
+crimm requires `python>=3.10`. The main dependencies are biopython, nglview, scipy, and requests. To use the adaptors, the respective packages need to be installed separately (e.g. pyCHARMM, rdkit, etc.)
+
+-----------------
 ## Base Library and Object Handles
 This library is built upon the excellent Biopython library. The macromolecular entity representations are derived from Biopython's entity classes and follow the same hierarchy. As a result, the entities in this library remain fully compatible with all functions and routines provided in Biopython.
 ## Parser Module
 New and improved mmCIF parser is implemented to allow accurate structure representations and more complete information.
 
 ## Looper Module
 For a given PDB structure with gaps or missing loops in the chain, this module provides functions to query PDB for the residue sequence and fill in the gaps or missing loop regions with the residues coordinates from the homology models.
```

### Comparing `crimm-2023.5a3/crimm/Adaptors/OMMAdaptors.py` & `crimm-2023.5a4/crimm/Adaptors/OMMAdaptors.py`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/Adaptors/PropKaAdaptors.py` & `crimm-2023.5a4/crimm/Adaptors/PropKaAdaptors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Derived Propka Atom class to facilitate atom class conversion for pKa calculation"""
 import os
+import warnings
 from typing import Optional, Tuple
 from propka.input import read_parameter_file
 from propka.parameters import Parameters
 from propka.version import VersionA
 from propka.lib import protein_precheck
 from propka.molecular_container import MolecularContainer as _MolContnr
 from propka.conformation_container import ConformationContainer
@@ -260,26 +261,56 @@
         fixer.build_missing_atoms()
         fixer.build_hydrogens()
         fixer.remove_undefined_atoms()
 
     def apply_patches(self):
         """Apply patches to the model."""
         if len(self.patches) == 0:
+            warnings.warn("No patches to apply.")
             return
         for chain_id, patches in self.patches.items():
             for resseq, patch_name in patches.items():
                 residue = self.model[chain_id][resseq]
                 self._patch_residue(residue, patch_name)
+            chain = self.model[chain_id]
+            if chain.topo_elements is not None:
+                # Update topology elements if they are already defined
+                chain.topo_elements.update()
 
     def report(self):
         fmt = (
             "{chain_id:2s} {i:3d} {resname:3s} pKa={pka:>5.2f} "
             "model_pKa={model_pka:>4.1f} buriedness={buried:5.3f}"
         )
         for chain_id, groups in self.reportable_groups.items():
             for i, g in groups.items():
                 out_str = fmt.format(
                     chain_id = chain_id, i=i, resname=g.atom.res_name, 
                     pka=g.pka_value, model_pka = g.model_pka,
                     buried = g.buried
                 )
-                print(out_str)
+                print(out_str)
+
+    def to_dict(self):
+        """Return a dictionary with pKa values."""
+        data = {}
+        for chain_id, groups in self.reportable_groups.items():
+            data[chain_id] = {}
+            for i, g in groups.items():
+                data[chain_id][i] = {
+                    'resname': g.atom.res_name, 'pka': g.pka_value, 
+                    'model_pka': g.model_pka, 'buriedness': g.buried
+                }
+        return data
+    
+    def to_dataframe(self):
+        """Return a pandas dataframe with pKa values."""
+        data = []
+        for chain_id, groups in self.reportable_groups.items():
+            for i, g in groups.items():
+                data.append({
+                    'chain_id': chain_id, 'resseq': i, 'resname': g.atom.res_name, 
+                    'pka': g.pka_value, 'model_pka': g.model_pka,
+                    'buriedness': g.buried
+                })
+        import pandas as pd
+        return pd.DataFrame(data)
```

### Comparing `crimm-2023.5a3/crimm/Adaptors/RDKitAdaptor.py` & `crimm-2023.5a4/crimm/Adaptors/RDKitAdaptor.py`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/Adaptors/pyCHARMMAdaptors.py` & `crimm-2023.5a4/crimm/Adaptors/pyCHARMMAdaptors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import os
 import tempfile
 import pycharmm as chm
 from pycharmm import read, write, psf, coor
-from pycharmm.psf import delete_atoms
-from pycharmm.select_atoms import SelectAtoms
 from pycharmm import generate
 from pycharmm import ic, cons_harm
 from pycharmm import minimize as _minimize
 from crimm.IO import get_pdb_str
 
 nucleic_letters_1to3 = {
     'A': 'ADE', 'C': 'CYT', 'G': 'GUA', 'T': 'THY', 'U': 'URA',
@@ -59,15 +57,15 @@
         
 def _get_charmm_named_chain(chain, segid):
     m_chain = chain.copy()
     if chain.chain_type == 'Polypeptide(L)':
         for res in m_chain:
             res.segid = segid
             if res.resname == 'HIS':
-                res.resname = 'HSD'
+                res.resname = res.topo_definition.resname
     elif chain.chain_type == 'Polyribonucleotide':
         for res in m_chain:
             res.segid = segid
             res.resname = nucleic_letters_1to3[res.resname]
     return m_chain
 
 
@@ -137,11 +135,7 @@
     atom_coords = list(zip(psf.get_atype(), new_coord_df.to_numpy()))
     for i, (st, end) in enumerate(zip(ibase[:-1], ibase[1:])):
         cur_res = chain.residues[i]
         for atom_name, coordinate in atom_coords[st:end]:
             if atom_name in cur_res:
                 cur_res[atom_name].coord = coordinate
     print(f'Synchronized: {chain}')
-    
-def remove_all_atoms():
-    all_atoms = SelectAtoms(select_all=True)
-    delete_atoms(selection=all_atoms)
```

### Comparing `crimm-2023.5a3/crimm/Data/connect_records.py` & `crimm-2023.5a4/crimm/Data/connect_records.py`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/Data/toppar/carb.prm` & `crimm-2023.5a4/crimm/Data/toppar/carb.prm`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/Data/toppar/carb.rtf` & `crimm-2023.5a4/crimm/Data/toppar/carb.rtf`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/Data/toppar/cgenff.prm` & `crimm-2023.5a4/crimm/Data/toppar/cgenff.prm`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/Data/toppar/cgenff.rtf` & `crimm-2023.5a4/crimm/Data/toppar/cgenff.rtf`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/Data/toppar/ethers.prm` & `crimm-2023.5a4/crimm/Data/toppar/ethers.prm`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/Data/toppar/ethers.rtf` & `crimm-2023.5a4/crimm/Data/toppar/ethers.rtf`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/Data/toppar/lipid.prm` & `crimm-2023.5a4/crimm/Data/toppar/lipid.prm`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/Data/toppar/lipid.rtf` & `crimm-2023.5a4/crimm/Data/toppar/lipid.rtf`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/Data/toppar/na.prm` & `crimm-2023.5a4/crimm/Data/toppar/na.prm`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/Data/toppar/na.rtf` & `crimm-2023.5a4/crimm/Data/toppar/na.rtf`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/Data/toppar/na_orig.rtf` & `crimm-2023.5a4/crimm/Data/toppar/na_orig.rtf`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/Data/toppar/prot.prm` & `crimm-2023.5a4/crimm/Data/toppar/prot.prm`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/Data/toppar/prot.rtf` & `crimm-2023.5a4/crimm/Data/toppar/prot.rtf`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/Data/toppar/prot_orig.rtf` & `crimm-2023.5a4/crimm/Data/toppar/prot_orig.rtf`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/Fetchers.py` & `crimm-2023.5a4/crimm/Fetchers.py`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/IO/MMCIF2Dict.py` & `crimm-2023.5a4/crimm/IO/MMCIF2Dict.py`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/IO/MMCIFParser.py` & `crimm-2023.5a4/crimm/IO/MMCIFParser.py`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/IO/PDBParser.py` & `crimm-2023.5a4/crimm/IO/PDBParser.py`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/IO/PDBString.py` & `crimm-2023.5a4/crimm/IO/PDBString.py`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/IO/PRMParser.py` & `crimm-2023.5a4/crimm/IO/PRMParser.py`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/IO/RTFParser.py` & `crimm-2023.5a4/crimm/IO/RTFParser.py`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/IO/StructureBuilder.py` & `crimm-2023.5a4/crimm/IO/StructureBuilder.py`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/Modeller/CoordManipulator.py` & `crimm-2023.5a4/crimm/Modeller/CoordManipulator.py`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/Modeller/LoopBuilder.py` & `crimm-2023.5a4/crimm/Modeller/LoopBuilder.py`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/Modeller/ParamLoader.py` & `crimm-2023.5a4/crimm/Modeller/ParamLoader.py`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/Modeller/SeqChainGenerator.py` & `crimm-2023.5a4/crimm/Modeller/SeqChainGenerator.py`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/Modeller/TopoFixer.py` & `crimm-2023.5a4/crimm/Modeller/TopoFixer.py`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/Modeller/TopoLoader.py` & `crimm-2023.5a4/crimm/Modeller/TopoLoader.py`

 * *Files 1% similar despite different names*

```diff
@@ -484,17 +484,16 @@
             )
         chain.sort_residues()
         if first is not None:
             self.patch_residue(chain.child_list[0], first, "NTER", QUIET=QUIET)
         if last is not None:
             self.patch_residue(chain.child_list[-1], last, "CTER", QUIET=QUIET)
         if chain.topo_elements is not None:
-            # Update topology elements if they are already definedß
-            topo_elements = TopologyElementContainer()
-            chain.topo_elements = topo_elements.load_chain(chain)
+            # Update topology elements if they are already defined
+            chain.topo_elements.update()
 
     def patch_residue(
             self, residue: Entities.Residue, patch: str,
             patch_loc = 'MIDCHAIN', QUIET = False
         ):
         """Patch the residue with the patch definition"""
         if residue.topo_definition is None:
@@ -530,19 +529,19 @@
         self.impropers = None
         self.cmap = None
         self.atom_lookup = None
         self.missing_param_dict = None
         self.containing_entity = None
 
     def __iter__(self):
-        topo_attrs = [
+        topo_types = [
             'bonds', 'angles', 'dihedrals', 'impropers', 'cmap'
         ]
-        for attr in topo_attrs:
-            yield attr, getattr(self, attr)
+        for topo_type_name in topo_types:
+            yield topo_type_name, getattr(self, topo_type_name)
 
     def __repr__(self) -> str:
         if self.containing_entity is None:
             return "<EmptyTopologyElementContainer>"
         s = f"<TopologyElementContainer for {self.containing_entity} with "
         for attr, value in self:
             if value is None:
@@ -555,15 +554,33 @@
 
     def load_chain(self, chain: Entities.PolymerChain):
         """Find all topology elements from the chain"""
         self.containing_entity = chain
         self.find_topo_elements(chain)
         self.create_atom_lookup_table()
         return self
-    
+
+    def update(self):
+        """Update the topology elements"""
+        self.find_topo_elements(self.containing_entity)
+        self.create_atom_lookup_table()
+        
+    ## Maybe make this a private method?
+    def delete_atom_related_elements(self, atom: Entities.Atom):
+        """Delete all topology elements related to the atom"""
+        for topo_type_name, topo_list in self:
+            if topo_list is None:
+                continue
+            remove_list = []
+            for topo in topo_list:
+                if atom in topo:
+                    remove_list.append(topo)
+            for topo in remove_list:
+                topo_list.remove(topo)
+
     @staticmethod
     def _find_seeding_atom(chain):
         """Find the first atom to start the search"""
         for atom in chain.child_list[0]:
             if len(atom.neighbors) > 0:
                 return atom
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `crimm-2023.5a3/crimm/StructEntities/Atom.py` & `crimm-2023.5a4/crimm/StructEntities/Atom.py`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/StructEntities/Chain.py` & `crimm-2023.5a4/crimm/StructEntities/Chain.py`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/StructEntities/Model.py` & `crimm-2023.5a4/crimm/StructEntities/Model.py`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/StructEntities/Residue.py` & `crimm-2023.5a4/crimm/StructEntities/Residue.py`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/StructEntities/Structure.py` & `crimm-2023.5a4/crimm/StructEntities/Structure.py`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/StructEntities/TopoDefinitions.py` & `crimm-2023.5a4/crimm/StructEntities/TopoDefinitions.py`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/StructEntities/TopoElements.py` & `crimm-2023.5a4/crimm/StructEntities/TopoElements.py`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/StructEntities/Topology.py` & `crimm-2023.5a4/crimm/StructEntities/Topology.py`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/Superimpose/ChainSuperimposer.py` & `crimm-2023.5a4/crimm/Superimpose/ChainSuperimposer.py`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm/Visualization/NGLVisualization.py` & `crimm-2023.5a4/crimm/Visualization/NGLVisualization.py`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/crimm.egg-info/PKG-INFO` & `crimm-2023.5a4/crimm.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 Metadata-Version: 2.1
 Name: crimm
-Version: 2023.5a3
+Version: 2023.5a4
 Summary: Chemistry with the ReInvented Macromolecular
 Author-email: Truman Xu <ziqiaoxu@umich.edu>
 Project-URL: Homepage, https://github.com/Truman-Xu/crimm
 Project-URL: Bug Tracker, https://github.com/Truman-Xu/crimm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# **CRIMM**
-**CRIMM** stands for **Chemistry with the ReInvented Macromolecular Mechanics**. This project aims to integrate and supplement CHARMM with better object handle and APIs
+# **crimm**
+**crimm** stands for **Chemistry with the ReInvented Macromolecular Mechanics**. This project aims to integrate and supplement CHARMM with better object handle and APIs
 
 ## Why *"reinvent the wheel"*
 This is a toolkit that is under active development, where many useful macromolecular modeling routines are selected to be reimplemented. This is an attempt to unify many macromolecular preparation/modeling routine under one platform while offering proper object handles and APIs in python. While currently, we aim to integrate with CHARMM and pyCHARMM, the broader goal is to provide highly usable, integratable, and scriptable python library/platform for simplifying any macromolecular modeling pipelines.
 
+-----------------
+## Installations
+crimm can be installed by `pip install crimm`
+
+crimm requires `python>=3.10`. The main dependencies are biopython, nglview, scipy, and requests. To use the adaptors, the respective packages need to be installed separately (e.g. pyCHARMM, rdkit, etc.)
+
+-----------------
 ## Base Library and Object Handles
 This library is built upon the excellent Biopython library. The macromolecular entity representations are derived from Biopython's entity classes and follow the same hierarchy. As a result, the entities in this library remain fully compatible with all functions and routines provided in Biopython.
 ## Parser Module
 New and improved mmCIF parser is implemented to allow accurate structure representations and more complete information.
 
 ## Looper Module
 For a given PDB structure with gaps or missing loops in the chain, this module provides functions to query PDB for the residue sequence and fill in the gaps or missing loop regions with the residues coordinates from the homology models.
```

### Comparing `crimm-2023.5a3/crimm.egg-info/SOURCES.txt` & `crimm-2023.5a4/crimm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/pyproject.toml` & `crimm-2023.5a4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=59.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "crimm"
-version = "2023.5a3"
+version = "2023.5a4"
 authors = [
   { name="Truman Xu", email="ziqiaoxu@umich.edu" },
 ]
 description = "Chemistry with the ReInvented Macromolecular"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
```

### Comparing `crimm-2023.5a3/src/chatgpt/steepestDescent.py` & `crimm-2023.5a4/src/chatgpt/steepestDescent.py`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/tests/test_pdb.py` & `crimm-2023.5a4/tests/test_pdb.py`

 * *Files identical despite different names*

### Comparing `crimm-2023.5a3/tests/test_pdb_standard.py` & `crimm-2023.5a4/tests/test_pdb_standard.py`

 * *Files identical despite different names*

