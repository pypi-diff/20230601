# Comparing `tmp/pyEasyML-1.0.2.tar.gz` & `tmp/pyEasyML-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyEasyML-1.0.2.tar", last modified: Thu Jun  1 17:41:19 2023, max compression
+gzip compressed data, was "pyEasyML-1.0.3.tar", last modified: Thu Jun  1 20:42:23 2023, max compression
```

## Comparing `pyEasyML-1.0.2.tar` & `pyEasyML-1.0.3.tar`

### file list

```diff
@@ -1,70 +1,73 @@
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:41:19.100227 pyEasyML-1.0.2/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1083 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/LICENSE
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      743 2023-06-01 17:41:19.100227 pyEasyML-1.0.2/PKG-INFO
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      344 2023-06-01 14:11:32.000000 pyEasyML-1.0.2/README.md
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:41:19.096227 pyEasyML-1.0.2/pyEasyML/
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:41:19.096227 pyEasyML-1.0.2/pyEasyML/Classification/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     5653 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Classification/Classifier.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1609 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Classification/Factory.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:41:19.096227 pyEasyML-1.0.2/pyEasyML/Classification/Models/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     4031 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Classification/Models/AbstractModel.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      896 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Classification/Models/GradientBoostingClassifier.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     3629 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Classification/Models/IsolationForest.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1153 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Classification/Models/KMeans.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      827 2023-06-01 13:39:31.000000 pyEasyML-1.0.2/pyEasyML/Classification/Models/KNeighborsClassifier.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      817 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Classification/Models/LogisticRegression.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      778 2023-06-01 13:39:31.000000 pyEasyML-1.0.2/pyEasyML/Classification/Models/RandomForestClassifier.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      623 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Classification/Models/SVC.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      844 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Classification/Models/XGBClassifier.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Classification/Models/__init__.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1675 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Classification/SearchModelsBestParams.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Classification/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:41:19.096227 pyEasyML-1.0.2/pyEasyML/Configs/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2666 2023-06-01 17:37:26.000000 pyEasyML-1.0.2/pyEasyML/Configs/Config.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Configs/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:41:19.096227 pyEasyML-1.0.2/pyEasyML/Customize/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1214 2023-06-01 17:36:14.000000 pyEasyML-1.0.2/pyEasyML/Customize/Extension.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:23:23.000000 pyEasyML-1.0.2/pyEasyML/Customize/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:41:19.096227 pyEasyML-1.0.2/pyEasyML/Data/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     6785 2023-06-01 17:28:13.000000 pyEasyML-1.0.2/pyEasyML/Data/DataPreprocessing.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     3692 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Data/FeatureSelection.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Data/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:41:19.096227 pyEasyML-1.0.2/pyEasyML/Email/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2802 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Email/Email.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Email/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:41:19.096227 pyEasyML-1.0.2/pyEasyML/NeuralNetworks/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2159 2023-05-31 04:12:00.000000 pyEasyML-1.0.2/pyEasyML/NeuralNetworks/AbstractANN.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:41:19.096227 pyEasyML-1.0.2/pyEasyML/NeuralNetworks/AnomalyDetection/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     5595 2023-06-01 13:39:31.000000 pyEasyML-1.0.2/pyEasyML/NeuralNetworks/AnomalyDetection/AnomalyDetector.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1163 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/NeuralNetworks/AnomalyDetection/Factory.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/NeuralNetworks/AnomalyDetection/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:41:19.096227 pyEasyML-1.0.2/pyEasyML/NeuralNetworks/Autoencoders/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      941 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/NeuralNetworks/Autoencoders/ConvolutionalAutoencoder.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     6614 2023-06-01 13:39:31.000000 pyEasyML-1.0.2/pyEasyML/NeuralNetworks/Autoencoders/DeepAutoencoder.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/NeuralNetworks/Autoencoders/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:41:19.096227 pyEasyML-1.0.2/pyEasyML/NeuralNetworks/Layers/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      383 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/NeuralNetworks/Layers/ConvolutionalLayers.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      783 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/NeuralNetworks/Layers/DeepAutoencoderLayers.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2092 2023-06-01 13:39:31.000000 pyEasyML-1.0.2/pyEasyML/NeuralNetworks/Layers/Layers.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/NeuralNetworks/Layers/__init__.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/NeuralNetworks/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:41:19.096227 pyEasyML-1.0.2/pyEasyML/OutlierDetection/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/OutlierDetection/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:41:19.100227 pyEasyML-1.0.2/pyEasyML/Regression/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      326 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Regression/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:41:19.100227 pyEasyML-1.0.2/pyEasyML/Utils/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2623 2023-06-01 17:29:25.000000 pyEasyML-1.0.2/pyEasyML/Utils/ColumnsToID.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      727 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Utils/Singleton.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2979 2023-06-01 17:35:45.000000 pyEasyML-1.0.2/pyEasyML/Utils/Threshold.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Utils/__init__.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1282 2023-06-01 13:39:31.000000 pyEasyML-1.0.2/pyEasyML/__init__.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2727 2023-06-01 14:03:15.000000 pyEasyML-1.0.2/pyEasyML/pyEasyMLcli.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:41:19.096227 pyEasyML-1.0.2/pyEasyML.egg-info/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      743 2023-06-01 17:41:19.000000 pyEasyML-1.0.2/pyEasyML.egg-info/PKG-INFO
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1970 2023-06-01 17:41:19.000000 pyEasyML-1.0.2/pyEasyML.egg-info/SOURCES.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        1 2023-06-01 17:41:19.000000 pyEasyML-1.0.2/pyEasyML.egg-info/dependency_links.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       54 2023-06-01 17:41:19.000000 pyEasyML-1.0.2/pyEasyML.egg-info/entry_points.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       46 2023-06-01 17:41:19.000000 pyEasyML-1.0.2/pyEasyML.egg-info/requires.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        9 2023-06-01 17:41:19.000000 pyEasyML-1.0.2/pyEasyML.egg-info/top_level.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       38 2023-06-01 17:41:19.100227 pyEasyML-1.0.2/setup.cfg
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1192 2023-06-01 17:41:06.000000 pyEasyML-1.0.2/setup.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.185946 pyEasyML-1.0.3/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1083 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/LICENSE
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      743 2023-06-01 20:42:23.185946 pyEasyML-1.0.3/PKG-INFO
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      344 2023-06-01 17:42:38.000000 pyEasyML-1.0.3/README.md
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.181947 pyEasyML-1.0.3/pyEasyML/
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.181947 pyEasyML-1.0.3/pyEasyML/Classification/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     5653 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Classification/Classifier.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1609 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Classification/Factory.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.185946 pyEasyML-1.0.3/pyEasyML/Classification/Models/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     4031 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Classification/Models/AbstractModel.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      896 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Classification/Models/GradientBoostingClassifier.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     3629 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Classification/Models/IsolationForest.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1153 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Classification/Models/KMeans.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      827 2023-06-01 13:39:31.000000 pyEasyML-1.0.3/pyEasyML/Classification/Models/KNeighborsClassifier.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      817 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Classification/Models/LogisticRegression.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      778 2023-06-01 13:39:31.000000 pyEasyML-1.0.3/pyEasyML/Classification/Models/RandomForestClassifier.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      623 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Classification/Models/SVC.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      844 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Classification/Models/XGBClassifier.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Classification/Models/__init__.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1675 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Classification/SearchModelsBestParams.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Classification/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.185946 pyEasyML-1.0.3/pyEasyML/Configs/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2666 2023-06-01 17:42:38.000000 pyEasyML-1.0.3/pyEasyML/Configs/Config.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Configs/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.185946 pyEasyML-1.0.3/pyEasyML/Customize/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      858 2023-06-01 20:39:47.000000 pyEasyML-1.0.3/pyEasyML/Customize/Extension.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.185946 pyEasyML-1.0.3/pyEasyML/Customize/InPlace/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      687 2023-06-01 20:34:10.000000 pyEasyML-1.0.3/pyEasyML/Customize/InPlace/Extension.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:33:28.000000 pyEasyML-1.0.3/pyEasyML/Customize/InPlace/__init__.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:42:38.000000 pyEasyML-1.0.3/pyEasyML/Customize/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.185946 pyEasyML-1.0.3/pyEasyML/Data/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     6785 2023-06-01 17:42:38.000000 pyEasyML-1.0.3/pyEasyML/Data/DataPreprocessing.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     3692 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Data/FeatureSelection.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Data/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.185946 pyEasyML-1.0.3/pyEasyML/Email/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2802 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Email/Email.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Email/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.185946 pyEasyML-1.0.3/pyEasyML/NeuralNetworks/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2159 2023-05-31 04:12:00.000000 pyEasyML-1.0.3/pyEasyML/NeuralNetworks/AbstractANN.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.185946 pyEasyML-1.0.3/pyEasyML/NeuralNetworks/AnomalyDetection/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     5595 2023-06-01 13:39:31.000000 pyEasyML-1.0.3/pyEasyML/NeuralNetworks/AnomalyDetection/AnomalyDetector.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1163 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/NeuralNetworks/AnomalyDetection/Factory.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/NeuralNetworks/AnomalyDetection/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.185946 pyEasyML-1.0.3/pyEasyML/NeuralNetworks/Autoencoders/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      941 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/NeuralNetworks/Autoencoders/ConvolutionalAutoencoder.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     6614 2023-06-01 13:39:31.000000 pyEasyML-1.0.3/pyEasyML/NeuralNetworks/Autoencoders/DeepAutoencoder.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/NeuralNetworks/Autoencoders/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.185946 pyEasyML-1.0.3/pyEasyML/NeuralNetworks/Layers/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      383 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/NeuralNetworks/Layers/ConvolutionalLayers.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      783 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/NeuralNetworks/Layers/DeepAutoencoderLayers.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2092 2023-06-01 13:39:31.000000 pyEasyML-1.0.3/pyEasyML/NeuralNetworks/Layers/Layers.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/NeuralNetworks/Layers/__init__.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/NeuralNetworks/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.185946 pyEasyML-1.0.3/pyEasyML/OutlierDetection/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/OutlierDetection/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.185946 pyEasyML-1.0.3/pyEasyML/Regression/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      326 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Regression/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.185946 pyEasyML-1.0.3/pyEasyML/Utils/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2623 2023-06-01 17:42:38.000000 pyEasyML-1.0.3/pyEasyML/Utils/ColumnsToID.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      727 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Utils/Singleton.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2979 2023-06-01 17:42:38.000000 pyEasyML-1.0.3/pyEasyML/Utils/Threshold.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Utils/__init__.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1282 2023-06-01 13:39:31.000000 pyEasyML-1.0.3/pyEasyML/__init__.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2727 2023-06-01 17:42:38.000000 pyEasyML-1.0.3/pyEasyML/pyEasyMLcli.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.181947 pyEasyML-1.0.3/pyEasyML.egg-info/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      743 2023-06-01 20:42:23.000000 pyEasyML-1.0.3/pyEasyML.egg-info/PKG-INFO
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2049 2023-06-01 20:42:23.000000 pyEasyML-1.0.3/pyEasyML.egg-info/SOURCES.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        1 2023-06-01 20:42:23.000000 pyEasyML-1.0.3/pyEasyML.egg-info/dependency_links.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       54 2023-06-01 20:42:23.000000 pyEasyML-1.0.3/pyEasyML.egg-info/entry_points.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       46 2023-06-01 20:42:23.000000 pyEasyML-1.0.3/pyEasyML.egg-info/requires.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        9 2023-06-01 20:42:23.000000 pyEasyML-1.0.3/pyEasyML.egg-info/top_level.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       38 2023-06-01 20:42:23.185946 pyEasyML-1.0.3/setup.cfg
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1192 2023-06-01 20:41:50.000000 pyEasyML-1.0.3/setup.py
```

### Comparing `pyEasyML-1.0.2/LICENSE` & `pyEasyML-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.2/PKG-INFO` & `pyEasyML-1.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEasyML
-Version: 1.0.2
+Version: 1.0.3
 Summary: A python machine learning framework.
 Author: Rodrigo Santos de Carvalho
 Author-email: <rodrigosc2401@gmail.com>
 Keywords: python,AI,Machine Learning,Neural Networks
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyEasyML-1.0.2/pyEasyML/Classification/Classifier.py` & `pyEasyML-1.0.3/pyEasyML/Classification/Classifier.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.2/pyEasyML/Classification/Factory.py` & `pyEasyML-1.0.3/pyEasyML/Classification/Factory.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.2/pyEasyML/Classification/Models/AbstractModel.py` & `pyEasyML-1.0.3/pyEasyML/Classification/Models/AbstractModel.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.2/pyEasyML/Classification/Models/GradientBoostingClassifier.py` & `pyEasyML-1.0.3/pyEasyML/Classification/Models/GradientBoostingClassifier.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.2/pyEasyML/Classification/Models/IsolationForest.py` & `pyEasyML-1.0.3/pyEasyML/Classification/Models/IsolationForest.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.2/pyEasyML/Classification/Models/KMeans.py` & `pyEasyML-1.0.3/pyEasyML/Classification/Models/KMeans.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.2/pyEasyML/Classification/Models/KNeighborsClassifier.py` & `pyEasyML-1.0.3/pyEasyML/Classification/Models/KNeighborsClassifier.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.2/pyEasyML/Classification/Models/LogisticRegression.py` & `pyEasyML-1.0.3/pyEasyML/Classification/Models/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.2/pyEasyML/Classification/Models/RandomForestClassifier.py` & `pyEasyML-1.0.3/pyEasyML/Classification/Models/RandomForestClassifier.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.2/pyEasyML/Classification/Models/SVC.py` & `pyEasyML-1.0.3/pyEasyML/Classification/Models/SVC.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.2/pyEasyML/Classification/Models/XGBClassifier.py` & `pyEasyML-1.0.3/pyEasyML/Classification/Models/XGBClassifier.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.2/pyEasyML/Classification/SearchModelsBestParams.py` & `pyEasyML-1.0.3/pyEasyML/Classification/SearchModelsBestParams.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.2/pyEasyML/Configs/Config.py` & `pyEasyML-1.0.3/pyEasyML/Configs/Config.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.2/pyEasyML/Customize/Extension.py` & `pyEasyML-1.0.3/pyEasyML/Customize/Extension.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# https://stackoverflow.com/questions/7139111/python-extension-methods
-
 import os, sys, re
 from typing import Any
 
 # Evitando a criação de arquivos .pyc
 sys.dont_write_bytecode = True
 
 script_dir = os.path.abspath(__file__)
@@ -11,41 +9,29 @@
 # Apagando o nome do arquivo e deixando apenas o diretorio.
 script_dir = re.sub(pattern="pyEasyML.*", repl = "pyEasyML/", string = script_dir)
 
 os.chdir(script_dir)
 
 sys.path.append(script_dir)
 
-from Data.DataPreprocessing import DataPreprocessor
-
 class Extend:
-    def __init__(self, obj, method):
+    def __init__(self, cls, method):
         method_name = method.__name__
-        setattr(obj, method_name, method)
-        self.obj = obj
-        self.method_name = method_name
-
-    def __enter__(self):
-        return self.obj
-
-    def __exit__(self, type, value, traceback):
-        delattr(self.obj, self.method_name)
-
+        setattr(cls, method_name, method)
+        self.cls = cls
 
-if __name__ == "__main__":    
-    def get_class_name(self):   
-        return (self._a)
-
-    def test(self):
-        return "modified test"
+    def __call__(self, *args, **kwargs):
+        return self.cls(*args, **kwargs)
 
+if __name__ == "__main__":
     class C:
-        def __init__(self) -> None:
-            self._a = "a"
-            
+        def __init__(self, a) -> None:
+            self._a = a
+
         def test(self):
             return "TEST"
 
-    with Extend(C, get_class_name):
-        c = C()
-        print(c.get_class_name()) # prints 'modified test'
-        
+    def test(self):
+        return "TEST" + str(self._a)
+
+    c = Extend(C, test)(a=6)
+    print(c.test()) # TEST6
```

### Comparing `pyEasyML-1.0.2/pyEasyML/Data/DataPreprocessing.py` & `pyEasyML-1.0.3/pyEasyML/Data/DataPreprocessing.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.2/pyEasyML/Data/FeatureSelection.py` & `pyEasyML-1.0.3/pyEasyML/Data/FeatureSelection.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.2/pyEasyML/Email/Email.py` & `pyEasyML-1.0.3/pyEasyML/Email/Email.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.2/pyEasyML/NeuralNetworks/AbstractANN.py` & `pyEasyML-1.0.3/pyEasyML/NeuralNetworks/AbstractANN.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.2/pyEasyML/NeuralNetworks/AnomalyDetection/AnomalyDetector.py` & `pyEasyML-1.0.3/pyEasyML/NeuralNetworks/AnomalyDetection/AnomalyDetector.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.2/pyEasyML/NeuralNetworks/AnomalyDetection/Factory.py` & `pyEasyML-1.0.3/pyEasyML/NeuralNetworks/AnomalyDetection/Factory.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.2/pyEasyML/NeuralNetworks/Autoencoders/ConvolutionalAutoencoder.py` & `pyEasyML-1.0.3/pyEasyML/NeuralNetworks/Autoencoders/ConvolutionalAutoencoder.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.2/pyEasyML/NeuralNetworks/Autoencoders/DeepAutoencoder.py` & `pyEasyML-1.0.3/pyEasyML/NeuralNetworks/Autoencoders/DeepAutoencoder.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.2/pyEasyML/NeuralNetworks/Layers/DeepAutoencoderLayers.py` & `pyEasyML-1.0.3/pyEasyML/NeuralNetworks/Layers/DeepAutoencoderLayers.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.2/pyEasyML/NeuralNetworks/Layers/Layers.py` & `pyEasyML-1.0.3/pyEasyML/NeuralNetworks/Layers/Layers.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.2/pyEasyML/Utils/ColumnsToID.py` & `pyEasyML-1.0.3/pyEasyML/Utils/ColumnsToID.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.2/pyEasyML/Utils/Singleton.py` & `pyEasyML-1.0.3/pyEasyML/Utils/Singleton.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.2/pyEasyML/Utils/Threshold.py` & `pyEasyML-1.0.3/pyEasyML/Utils/Threshold.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.2/pyEasyML/__init__.py` & `pyEasyML-1.0.3/pyEasyML/__init__.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.2/pyEasyML/pyEasyMLcli.py` & `pyEasyML-1.0.3/pyEasyML/pyEasyMLcli.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.2/pyEasyML.egg-info/PKG-INFO` & `pyEasyML-1.0.3/pyEasyML.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEasyML
-Version: 1.0.2
+Version: 1.0.3
 Summary: A python machine learning framework.
 Author: Rodrigo Santos de Carvalho
 Author-email: <rodrigosc2401@gmail.com>
 Keywords: python,AI,Machine Learning,Neural Networks
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyEasyML-1.0.2/pyEasyML.egg-info/SOURCES.txt` & `pyEasyML-1.0.3/pyEasyML.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 pyEasyML/Classification/Models/SVC.py
 pyEasyML/Classification/Models/XGBClassifier.py
 pyEasyML/Classification/Models/__init__.py
 pyEasyML/Configs/Config.py
 pyEasyML/Configs/__init__.py
 pyEasyML/Customize/Extension.py
 pyEasyML/Customize/__init__.py
+pyEasyML/Customize/InPlace/Extension.py
+pyEasyML/Customize/InPlace/__init__.py
 pyEasyML/Data/DataPreprocessing.py
 pyEasyML/Data/FeatureSelection.py
 pyEasyML/Data/__init__.py
 pyEasyML/Email/Email.py
 pyEasyML/Email/__init__.py
 pyEasyML/NeuralNetworks/AbstractANN.py
 pyEasyML/NeuralNetworks/__init__.py
```

### Comparing `pyEasyML-1.0.2/setup.py` & `pyEasyML-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '1.0.2'
+VERSION = '1.0.3'
 DESCRIPTION = 'A python machine learning framework.'
 LONG_DESCRIPTION = 'A framework made to aid in the development of end-to-end machine learning projects, with data preprocessing, ml models, feature selection, hyperparameter tuning and much more.'
 
 # Setting up
 setup(
     name="pyEasyML",
     version=VERSION,
```

