# Comparing `tmp/pyPhasesML-0.6.1.tar.gz` & `tmp/pyPhasesML-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPhasesML-0.6.1.tar", last modified: Wed May 31 11:33:38 2023, max compression
+gzip compressed data, was "pyPhasesML-0.6.2.tar", last modified: Thu Jun  1 14:28:47 2023, max compression
```

## Comparing `pyPhasesML-0.6.1.tar` & `pyPhasesML-0.6.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:33:38.941336 pyPhasesML-0.6.1/
--rw-rw-rw-   0 root         (0) root         (0)     1065 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3691 2023-05-31 11:33:38.940336 pyPhasesML-0.6.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3184 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:33:38.937336 pyPhasesML-0.6.1/pyPhasesML/
--rw-rw-rw-   0 root         (0) root         (0)     2410 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/DataAugmentation.py
--rw-rw-rw-   0 root         (0) root         (0)      895 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/DataSet.py
--rw-rw-rw-   0 root         (0) root         (0)     3849 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/DataversionManager.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/FeatureExtraction.py
--rw-rw-rw-   0 root         (0) root         (0)     3798 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/Model.py
--rw-rw-rw-   0 root         (0) root         (0)     4491 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/ModelManager.py
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/Plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     4566 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/SignalPreprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)      391 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:33:38.938336 pyPhasesML-0.6.1/pyPhasesML/adapter/
--rw-rw-rw-   0 root         (0) root         (0)    10212 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/adapter/ModelKerasAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)     7116 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/adapter/ModelTf1Adapter.py
--rw-rw-rw-   0 root         (0) root         (0)    18468 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/adapter/ModelTorchAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/adapter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1106 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:33:38.939336 pyPhasesML-0.6.1/pyPhasesML/datapipes/
--rw-rw-rw-   0 root         (0) root         (0)      464 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/datapipes/Augmentor.py
--rw-rw-rw-   0 root         (0) root         (0)      626 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/datapipes/DatasetXY.py
--rw-rw-rw-   0 root         (0) root         (0)      995 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/datapipes/FoldMapper.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/datapipes/RecordMap.py
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/datapipes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:33:38.940336 pyPhasesML-0.6.1/pyPhasesML/exporter/
--rw-rw-rw-   0 root         (0) root         (0)     5385 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/exporter/MemmapRecordExporter.py
--rw-rw-rw-   0 root         (0) root         (0)     3201 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/exporter/ModelExporter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/exporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:33:38.940336 pyPhasesML-0.6.1/pyPhasesML/scorer/
--rw-rw-rw-   0 root         (0) root         (0)    18685 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/scorer/Scorer.py
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/scorer/ScorerTF.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/scorer/ScorerTorch.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/scorer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:33:38.938336 pyPhasesML-0.6.1/pyPhasesML.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3691 2023-05-31 11:33:38.000000 pyPhasesML-0.6.1/pyPhasesML.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1041 2023-05-31 11:33:38.000000 pyPhasesML-0.6.1/pyPhasesML.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 11:33:38.000000 pyPhasesML-0.6.1/pyPhasesML.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-05-31 11:33:38.000000 pyPhasesML-0.6.1/pyPhasesML.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-05-31 11:33:38.000000 pyPhasesML-0.6.1/pyPhasesML.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      484 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 11:33:38.941336 pyPhasesML-0.6.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      842 2023-05-31 11:33:22.000000 pyPhasesML-0.6.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:28:47.873707 pyPhasesML-0.6.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3691 2023-06-01 14:28:47.872707 pyPhasesML-0.6.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3184 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:28:47.869707 pyPhasesML-0.6.2/pyPhasesML/
+-rw-rw-rw-   0 root         (0) root         (0)     2410 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/DataAugmentation.py
+-rw-rw-rw-   0 root         (0) root         (0)      895 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/DataSet.py
+-rw-rw-rw-   0 root         (0) root         (0)     3849 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/DataversionManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/FeatureExtraction.py
+-rw-rw-rw-   0 root         (0) root         (0)     3798 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/Model.py
+-rw-rw-rw-   0 root         (0) root         (0)     4491 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/ModelManager.py
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/Plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4566 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/SignalPreprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:28:47.870707 pyPhasesML-0.6.2/pyPhasesML/adapter/
+-rw-rw-rw-   0 root         (0) root         (0)    10212 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/adapter/ModelKerasAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     7116 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/adapter/ModelTf1Adapter.py
+-rw-rw-rw-   0 root         (0) root         (0)    18506 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/adapter/ModelTorchAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/adapter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:28:47.871707 pyPhasesML-0.6.2/pyPhasesML/datapipes/
+-rw-rw-rw-   0 root         (0) root         (0)      464 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/datapipes/Augmentor.py
+-rw-rw-rw-   0 root         (0) root         (0)      626 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/datapipes/DatasetXY.py
+-rw-rw-rw-   0 root         (0) root         (0)      995 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/datapipes/FoldMapper.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/datapipes/RecordMap.py
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/datapipes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:28:47.872707 pyPhasesML-0.6.2/pyPhasesML/exporter/
+-rw-rw-rw-   0 root         (0) root         (0)     5385 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/exporter/MemmapRecordExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3201 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/exporter/ModelExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/exporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:28:47.872707 pyPhasesML-0.6.2/pyPhasesML/scorer/
+-rw-rw-rw-   0 root         (0) root         (0)    18685 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/scorer/Scorer.py
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/scorer/ScorerTF.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/scorer/ScorerTorch.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/scorer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:28:47.870707 pyPhasesML-0.6.2/pyPhasesML.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3691 2023-06-01 14:28:47.000000 pyPhasesML-0.6.2/pyPhasesML.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-06-01 14:28:47.000000 pyPhasesML-0.6.2/pyPhasesML.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 14:28:47.000000 pyPhasesML-0.6.2/pyPhasesML.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-01 14:28:47.000000 pyPhasesML-0.6.2/pyPhasesML.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-01 14:28:47.000000 pyPhasesML-0.6.2/pyPhasesML.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      484 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 14:28:47.873707 pyPhasesML-0.6.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      842 2023-06-01 14:28:31.000000 pyPhasesML-0.6.2/setup.py
```

### Comparing `pyPhasesML-0.6.1/LICENSE` & `pyPhasesML-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.1/PKG-INFO` & `pyPhasesML-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.6.1
+Version: 0.6.2
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.6.1/README.md` & `pyPhasesML-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.1/pyPhasesML/DataAugmentation.py` & `pyPhasesML-0.6.2/pyPhasesML/DataAugmentation.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.1/pyPhasesML/DataSet.py` & `pyPhasesML-0.6.2/pyPhasesML/DataSet.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.1/pyPhasesML/DataversionManager.py` & `pyPhasesML-0.6.2/pyPhasesML/DataversionManager.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.1/pyPhasesML/FeatureExtraction.py` & `pyPhasesML-0.6.2/pyPhasesML/FeatureExtraction.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.1/pyPhasesML/Model.py` & `pyPhasesML-0.6.2/pyPhasesML/Model.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.1/pyPhasesML/ModelManager.py` & `pyPhasesML-0.6.2/pyPhasesML/ModelManager.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.1/pyPhasesML/Plugin.py` & `pyPhasesML-0.6.2/pyPhasesML/Plugin.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.1/pyPhasesML/SignalPreprocessing.py` & `pyPhasesML-0.6.2/pyPhasesML/SignalPreprocessing.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.1/pyPhasesML/adapter/ModelKerasAdapter.py` & `pyPhasesML-0.6.2/pyPhasesML/adapter/ModelKerasAdapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.1/pyPhasesML/adapter/ModelTf1Adapter.py` & `pyPhasesML-0.6.2/pyPhasesML/adapter/ModelTf1Adapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.1/pyPhasesML/adapter/ModelTorchAdapter.py` & `pyPhasesML-0.6.2/pyPhasesML/adapter/ModelTorchAdapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,16 @@
 
         lastDimension = self.numClasses if self.oneHotDecoded else 1
         for batchIndex in processList:
             validationBatch = batchGenerator.__next__()
             x, y = self.prepareDataAdapter(validationBatch, validation=True)
 
             # Run model
-            output = model(x)
+            with torch.no_grad():
+                output = model(x)
             batchPredictions = self.mapOutputForPrediction(output)
 
             if len(s.metrics) > 0:
                 y = y.reshape(-1, lastDimension)
                 batchPredictions = batchPredictions.reshape(-1, lastDimension)
 
                 results = s.score(y, batchPredictions, trace=True)
```

### Comparing `pyPhasesML-0.6.1/pyPhasesML/config.yaml` & `pyPhasesML-0.6.2/pyPhasesML/config.yaml`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.1/pyPhasesML/datapipes/DatasetXY.py` & `pyPhasesML-0.6.2/pyPhasesML/datapipes/DatasetXY.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.1/pyPhasesML/datapipes/FoldMapper.py` & `pyPhasesML-0.6.2/pyPhasesML/datapipes/FoldMapper.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.1/pyPhasesML/exporter/MemmapRecordExporter.py` & `pyPhasesML-0.6.2/pyPhasesML/exporter/MemmapRecordExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.1/pyPhasesML/exporter/ModelExporter.py` & `pyPhasesML-0.6.2/pyPhasesML/exporter/ModelExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.1/pyPhasesML/scorer/Scorer.py` & `pyPhasesML-0.6.2/pyPhasesML/scorer/Scorer.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.1/pyPhasesML.egg-info/PKG-INFO` & `pyPhasesML-0.6.2/pyPhasesML.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.6.1
+Version: 0.6.2
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.6.1/pyPhasesML.egg-info/SOURCES.txt` & `pyPhasesML-0.6.2/pyPhasesML.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.1/setup.py` & `pyPhasesML-0.6.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyPhasesML",
-    version="v0.6.1"[1:],
+    version="v0.6.2"[1:],
     author="Franz Ehrlich",
     author_email="fehrlichd@gmail.com",
     description="A Framework for creating a boilerplate template for ai projects that are ready for MLOps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/",
     packages=setuptools.find_packages(),
```

