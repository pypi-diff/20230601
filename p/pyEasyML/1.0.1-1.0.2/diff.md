# Comparing `tmp/pyEasyML-1.0.1.tar.gz` & `tmp/pyEasyML-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyEasyML-1.0.1.tar", last modified: Thu Jun  1 13:41:25 2023, max compression
+gzip compressed data, was "pyEasyML-1.0.2.tar", last modified: Thu Jun  1 17:41:19 2023, max compression
```

## Comparing `pyEasyML-1.0.1.tar` & `pyEasyML-1.0.2.tar`

### file list

```diff
@@ -1,68 +1,70 @@
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 13:41:25.145761 pyEasyML-1.0.1/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1083 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/LICENSE
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      743 2023-06-01 13:41:25.145761 pyEasyML-1.0.1/PKG-INFO
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      276 2023-06-01 13:39:31.000000 pyEasyML-1.0.1/README.md
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 13:41:25.141761 pyEasyML-1.0.1/pyEasyML/
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 13:41:25.141761 pyEasyML-1.0.1/pyEasyML/Classification/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     5653 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Classification/Classifier.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1609 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Classification/Factory.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 13:41:25.141761 pyEasyML-1.0.1/pyEasyML/Classification/Models/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     4031 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Classification/Models/AbstractModel.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      896 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Classification/Models/GradientBoostingClassifier.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     3629 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Classification/Models/IsolationForest.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1153 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Classification/Models/KMeans.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      827 2023-06-01 13:39:31.000000 pyEasyML-1.0.1/pyEasyML/Classification/Models/KNeighborsClassifier.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      817 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Classification/Models/LogisticRegression.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      778 2023-06-01 13:39:31.000000 pyEasyML-1.0.1/pyEasyML/Classification/Models/RandomForestClassifier.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      623 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Classification/Models/SVC.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      844 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Classification/Models/XGBClassifier.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Classification/Models/__init__.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1675 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Classification/SearchModelsBestParams.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Classification/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 13:41:25.141761 pyEasyML-1.0.1/pyEasyML/Configs/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2681 2023-06-01 13:39:31.000000 pyEasyML-1.0.1/pyEasyML/Configs/Config.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Configs/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 13:41:25.141761 pyEasyML-1.0.1/pyEasyML/Data/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     6232 2023-06-01 13:39:31.000000 pyEasyML-1.0.1/pyEasyML/Data/DataPreprocessing.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     3692 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Data/FeatureSelection.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Data/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 13:41:25.141761 pyEasyML-1.0.1/pyEasyML/Email/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2802 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Email/Email.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Email/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 13:41:25.141761 pyEasyML-1.0.1/pyEasyML/NeuralNetworks/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2159 2023-05-31 04:12:00.000000 pyEasyML-1.0.1/pyEasyML/NeuralNetworks/AbstractANN.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 13:41:25.141761 pyEasyML-1.0.1/pyEasyML/NeuralNetworks/AnomalyDetection/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     5595 2023-06-01 13:39:31.000000 pyEasyML-1.0.1/pyEasyML/NeuralNetworks/AnomalyDetection/AnomalyDetector.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1163 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/NeuralNetworks/AnomalyDetection/Factory.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/NeuralNetworks/AnomalyDetection/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 13:41:25.145761 pyEasyML-1.0.1/pyEasyML/NeuralNetworks/Autoencoders/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      941 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/NeuralNetworks/Autoencoders/ConvolutionalAutoencoder.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     6614 2023-06-01 13:39:31.000000 pyEasyML-1.0.1/pyEasyML/NeuralNetworks/Autoencoders/DeepAutoencoder.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/NeuralNetworks/Autoencoders/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 13:41:25.145761 pyEasyML-1.0.1/pyEasyML/NeuralNetworks/Layers/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      383 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/NeuralNetworks/Layers/ConvolutionalLayers.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      783 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/NeuralNetworks/Layers/DeepAutoencoderLayers.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2092 2023-06-01 13:39:31.000000 pyEasyML-1.0.1/pyEasyML/NeuralNetworks/Layers/Layers.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/NeuralNetworks/Layers/__init__.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/NeuralNetworks/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 13:41:25.145761 pyEasyML-1.0.1/pyEasyML/OutlierDetection/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/OutlierDetection/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 13:41:25.145761 pyEasyML-1.0.1/pyEasyML/Regression/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      326 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Regression/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 13:41:25.145761 pyEasyML-1.0.1/pyEasyML/Utils/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2630 2023-06-01 13:39:31.000000 pyEasyML-1.0.1/pyEasyML/Utils/ColumnsToID.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      816 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Utils/Extension.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      727 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Utils/Singleton.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     3018 2023-06-01 13:39:31.000000 pyEasyML-1.0.1/pyEasyML/Utils/Threshold.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Utils/__init__.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1282 2023-06-01 13:39:31.000000 pyEasyML-1.0.1/pyEasyML/__init__.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2727 2023-06-01 13:39:31.000000 pyEasyML-1.0.1/pyEasyML/pyEasyMLcli.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 13:41:25.141761 pyEasyML-1.0.1/pyEasyML.egg-info/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      743 2023-06-01 13:41:25.000000 pyEasyML-1.0.1/pyEasyML.egg-info/PKG-INFO
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1935 2023-06-01 13:41:25.000000 pyEasyML-1.0.1/pyEasyML.egg-info/SOURCES.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        1 2023-06-01 13:41:25.000000 pyEasyML-1.0.1/pyEasyML.egg-info/dependency_links.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       54 2023-06-01 13:41:25.000000 pyEasyML-1.0.1/pyEasyML.egg-info/entry_points.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       46 2023-06-01 13:41:25.000000 pyEasyML-1.0.1/pyEasyML.egg-info/requires.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        9 2023-06-01 13:41:25.000000 pyEasyML-1.0.1/pyEasyML.egg-info/top_level.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       38 2023-06-01 13:41:25.145761 pyEasyML-1.0.1/setup.cfg
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1192 2023-06-01 13:40:46.000000 pyEasyML-1.0.1/setup.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:41:19.100227 pyEasyML-1.0.2/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1083 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/LICENSE
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      743 2023-06-01 17:41:19.100227 pyEasyML-1.0.2/PKG-INFO
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      344 2023-06-01 14:11:32.000000 pyEasyML-1.0.2/README.md
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:41:19.096227 pyEasyML-1.0.2/pyEasyML/
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:41:19.096227 pyEasyML-1.0.2/pyEasyML/Classification/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     5653 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Classification/Classifier.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1609 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Classification/Factory.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:41:19.096227 pyEasyML-1.0.2/pyEasyML/Classification/Models/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     4031 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Classification/Models/AbstractModel.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      896 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Classification/Models/GradientBoostingClassifier.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     3629 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Classification/Models/IsolationForest.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1153 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Classification/Models/KMeans.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      827 2023-06-01 13:39:31.000000 pyEasyML-1.0.2/pyEasyML/Classification/Models/KNeighborsClassifier.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      817 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Classification/Models/LogisticRegression.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      778 2023-06-01 13:39:31.000000 pyEasyML-1.0.2/pyEasyML/Classification/Models/RandomForestClassifier.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      623 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Classification/Models/SVC.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      844 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Classification/Models/XGBClassifier.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Classification/Models/__init__.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1675 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Classification/SearchModelsBestParams.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Classification/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:41:19.096227 pyEasyML-1.0.2/pyEasyML/Configs/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2666 2023-06-01 17:37:26.000000 pyEasyML-1.0.2/pyEasyML/Configs/Config.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Configs/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:41:19.096227 pyEasyML-1.0.2/pyEasyML/Customize/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1214 2023-06-01 17:36:14.000000 pyEasyML-1.0.2/pyEasyML/Customize/Extension.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:23:23.000000 pyEasyML-1.0.2/pyEasyML/Customize/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:41:19.096227 pyEasyML-1.0.2/pyEasyML/Data/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     6785 2023-06-01 17:28:13.000000 pyEasyML-1.0.2/pyEasyML/Data/DataPreprocessing.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     3692 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Data/FeatureSelection.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Data/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:41:19.096227 pyEasyML-1.0.2/pyEasyML/Email/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2802 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Email/Email.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Email/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:41:19.096227 pyEasyML-1.0.2/pyEasyML/NeuralNetworks/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2159 2023-05-31 04:12:00.000000 pyEasyML-1.0.2/pyEasyML/NeuralNetworks/AbstractANN.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:41:19.096227 pyEasyML-1.0.2/pyEasyML/NeuralNetworks/AnomalyDetection/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     5595 2023-06-01 13:39:31.000000 pyEasyML-1.0.2/pyEasyML/NeuralNetworks/AnomalyDetection/AnomalyDetector.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1163 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/NeuralNetworks/AnomalyDetection/Factory.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/NeuralNetworks/AnomalyDetection/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:41:19.096227 pyEasyML-1.0.2/pyEasyML/NeuralNetworks/Autoencoders/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      941 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/NeuralNetworks/Autoencoders/ConvolutionalAutoencoder.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     6614 2023-06-01 13:39:31.000000 pyEasyML-1.0.2/pyEasyML/NeuralNetworks/Autoencoders/DeepAutoencoder.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/NeuralNetworks/Autoencoders/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:41:19.096227 pyEasyML-1.0.2/pyEasyML/NeuralNetworks/Layers/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      383 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/NeuralNetworks/Layers/ConvolutionalLayers.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      783 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/NeuralNetworks/Layers/DeepAutoencoderLayers.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2092 2023-06-01 13:39:31.000000 pyEasyML-1.0.2/pyEasyML/NeuralNetworks/Layers/Layers.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/NeuralNetworks/Layers/__init__.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/NeuralNetworks/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:41:19.096227 pyEasyML-1.0.2/pyEasyML/OutlierDetection/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/OutlierDetection/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:41:19.100227 pyEasyML-1.0.2/pyEasyML/Regression/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      326 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Regression/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:41:19.100227 pyEasyML-1.0.2/pyEasyML/Utils/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2623 2023-06-01 17:29:25.000000 pyEasyML-1.0.2/pyEasyML/Utils/ColumnsToID.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      727 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Utils/Singleton.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2979 2023-06-01 17:35:45.000000 pyEasyML-1.0.2/pyEasyML/Utils/Threshold.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.2/pyEasyML/Utils/__init__.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1282 2023-06-01 13:39:31.000000 pyEasyML-1.0.2/pyEasyML/__init__.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2727 2023-06-01 14:03:15.000000 pyEasyML-1.0.2/pyEasyML/pyEasyMLcli.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:41:19.096227 pyEasyML-1.0.2/pyEasyML.egg-info/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      743 2023-06-01 17:41:19.000000 pyEasyML-1.0.2/pyEasyML.egg-info/PKG-INFO
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1970 2023-06-01 17:41:19.000000 pyEasyML-1.0.2/pyEasyML.egg-info/SOURCES.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        1 2023-06-01 17:41:19.000000 pyEasyML-1.0.2/pyEasyML.egg-info/dependency_links.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       54 2023-06-01 17:41:19.000000 pyEasyML-1.0.2/pyEasyML.egg-info/entry_points.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       46 2023-06-01 17:41:19.000000 pyEasyML-1.0.2/pyEasyML.egg-info/requires.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        9 2023-06-01 17:41:19.000000 pyEasyML-1.0.2/pyEasyML.egg-info/top_level.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       38 2023-06-01 17:41:19.100227 pyEasyML-1.0.2/setup.cfg
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1192 2023-06-01 17:41:06.000000 pyEasyML-1.0.2/setup.py
```

### Comparing `pyEasyML-1.0.1/LICENSE` & `pyEasyML-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.1/PKG-INFO` & `pyEasyML-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEasyML
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python machine learning framework.
 Author: Rodrigo Santos de Carvalho
 Author-email: <rodrigosc2401@gmail.com>
 Keywords: python,AI,Machine Learning,Neural Networks
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyEasyML-1.0.1/pyEasyML/Classification/Classifier.py` & `pyEasyML-1.0.2/pyEasyML/Classification/Classifier.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.1/pyEasyML/Classification/Factory.py` & `pyEasyML-1.0.2/pyEasyML/Classification/Factory.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.1/pyEasyML/Classification/Models/AbstractModel.py` & `pyEasyML-1.0.2/pyEasyML/Classification/Models/AbstractModel.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.1/pyEasyML/Classification/Models/GradientBoostingClassifier.py` & `pyEasyML-1.0.2/pyEasyML/Classification/Models/GradientBoostingClassifier.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.1/pyEasyML/Classification/Models/IsolationForest.py` & `pyEasyML-1.0.2/pyEasyML/Classification/Models/IsolationForest.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.1/pyEasyML/Classification/Models/KMeans.py` & `pyEasyML-1.0.2/pyEasyML/Classification/Models/KMeans.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.1/pyEasyML/Classification/Models/KNeighborsClassifier.py` & `pyEasyML-1.0.2/pyEasyML/Classification/Models/KNeighborsClassifier.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.1/pyEasyML/Classification/Models/LogisticRegression.py` & `pyEasyML-1.0.2/pyEasyML/Classification/Models/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.1/pyEasyML/Classification/Models/RandomForestClassifier.py` & `pyEasyML-1.0.2/pyEasyML/Classification/Models/RandomForestClassifier.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.1/pyEasyML/Classification/Models/SVC.py` & `pyEasyML-1.0.2/pyEasyML/Classification/Models/SVC.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.1/pyEasyML/Classification/Models/XGBClassifier.py` & `pyEasyML-1.0.2/pyEasyML/Classification/Models/XGBClassifier.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.1/pyEasyML/Classification/SearchModelsBestParams.py` & `pyEasyML-1.0.2/pyEasyML/Classification/SearchModelsBestParams.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.1/pyEasyML/Configs/Config.py` & `pyEasyML-1.0.2/pyEasyML/Configs/Config.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,19 +25,19 @@
         return instances[cls]
 
     return wrapper
 
 @singleton
 class Config():
     def __init__(self, client:str) -> None:
-        self.__configs:dict[str, str] = self.__load_configs(client)
-        self.__client:str = self.__configs['client']
-        self.__SELECTED_FEATURES:list[str] = []
-        self.__TARGET_FEATURE:str = "NOT DEFINED"
-        self.__RANDOM_STATE:int = 0
+        self._configs:dict[str, str] = self.__load_configs(client)
+        self._client:str = self._configs['client']
+        self._SELECTED_FEATURES:list[str] = []
+        self._TARGET_FEATURE:str = "NOT DEFINED"
+        self._RANDOM_STATE:int = 0
 
     def __load_configs(self, client: str) -> dict[str, str]:
         start = client
 
         for tries in range(100):
             json_path = os.path.join(start, 'configs.json')
             if os.path.exists(json_path):
@@ -48,43 +48,43 @@
                 parent_dir = os.path.dirname(os.path.dirname(start))
                 start = parent_dir
 
         return {'client': 'NOT DEFINED'}
 
     @property
     def SELECTED_FEATURES(self) -> list[str]:
-        return self.__SELECTED_FEATURES
+        return self._SELECTED_FEATURES
 
     @SELECTED_FEATURES.setter
     def SELECTED_FEATURES(self, selected_features:list[str]) -> None:
-        self.__SELECTED_FEATURES = selected_features
+        self._SELECTED_FEATURES = selected_features
 
     @property
     def TARGET_FEATURE(self) -> str:
-        return self.__TARGET_FEATURE
+        return self._TARGET_FEATURE
     
     @TARGET_FEATURE.setter
     def TARGET_FEATURE(self, target_feature:str) -> None:
-        self.__TARGET_FEATURE = target_feature
+        self._TARGET_FEATURE = target_feature
 
     @property
     def RANDOM_STATE(self) -> int:
-        return self.__RANDOM_STATE
+        return self._RANDOM_STATE
 
     def get_data_path(self) -> str:
-        return os.path.join(self.__client, 'dataset/')
+        return os.path.join(self._client, 'dataset/')
 
     def get_trained_models_path(self) -> str:
-        return os.path.join(self.__client, 'models/')
+        return os.path.join(self._client, 'models/')
 
     def get_normalization_model_path(self) -> str:
-        return os.path.join(self.__client, 'models/', 'normalizationModel/')
+        return os.path.join(self._client, 'models/', 'normalizationModel/')
 
     def get_utils_path(self) -> str:
-        return os.path.join(self.__client, 'Utils/')
+        return os.path.join(self._client, 'Utils/')
     
 
 if __name__ == '__main__':
     definitions = Config()
     print(definitions.TARGET_FEATURE)
     definitions.TARGET_FEATURE = 'target'
```

### Comparing `pyEasyML-1.0.1/pyEasyML/Data/DataPreprocessing.py` & `pyEasyML-1.0.2/pyEasyML/Data/DataPreprocessing.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,44 +19,60 @@
 import numpy as np
 import sklearn.model_selection, sklearn.preprocessing
 from Utils.ColumnsToID import ColumnsToID 
 from Utils.Singleton import Singleton
 from Configs.Config import Config
 import pickle
 from os.path import exists
+from typing import Any
+import glob
 from pandas.core.indexes.base import Index as pdIndexes
 
 class DataPreprocessor(Singleton):
     def __init__(self) -> None:
         if not super().created:
             self._config = Config()
             self._columns_to_id = ColumnsToID()
-            self.__DATASET_PATH:str = ""
-            self.__DATA_FOLDER_PATH:str = self._config.get_data_path()
+            self._DATASET_PATH:str = ""
+            self._DATA_FOLDER_PATH:str = self._config.get_data_path()
 
     @property
     def DATASET_PATH(self) -> str:
-        return self.__DATASET_PATH
+        return self._DATASET_PATH
 
     @DATASET_PATH.setter
     def DATASET_PATH(self, dataset_file_name:str) -> None:
-        self.__DATASET_PATH = os.path.join(self.__DATA_FOLDER_PATH, dataset_file_name)
+        self._DATASET_PATH = os.path.join(self._DATA_FOLDER_PATH, dataset_file_name)
+
+    def read_dataset(self, path: str) -> pd.DataFrame:
+        file_extension = os.path.splitext(path)[1].lower()
+    
+        if file_extension == ".csv":
+            return pd.read_csv(path)
+        elif file_extension == ".parquet":
+            return pd.read_parquet(path)
+        elif file_extension == ".xlsx":
+            return pd.read_excel(path)
+        # Add more conditions for other file formats if needed
+        else:
+            raise ValueError("Unsupported file extension: " + file_extension)    
 
     def read_all_data(self) -> pd.DataFrame:
-        all_data_path = os.path.join(self.__DATA_FOLDER_PATH, "all_data.parquet")
+        all_data_path = glob.glob(os.path.join(self._DATA_FOLDER_PATH, "all_data.*"))[0]
+
         if exists(all_data_path):
-            print("Reading all_data.parquet")
-            return pd.read_parquet(all_data_path)
+            print("Reading all_data.")
+            return self.read_dataset(all_data_path)
         else:
-            dataset_files = os.listdir(self.__DATA_FOLDER_PATH)
-            dataset_paths = [os.path.join(self.__DATA_FOLDER_PATH, dataset_file) for dataset_file in dataset_files]
+            dataset_files = os.listdir(self._DATA_FOLDER_PATH)
+            dataset_paths = [os.path.join(self._DATA_FOLDER_PATH, dataset_file) for dataset_file in dataset_files]
             
             datasets = []
             for dataset_path in dataset_paths:
-                dataset = pd.read_parquet(dataset_path)
+                dataset = self.read_dataset(dataset_path)
                 datasets.append(dataset)
             
             datasets = tuple(datasets)
             
             dataset = self.concat_datasets(*datasets)
 
             dataset, = self.clean_dataset(dataset)
@@ -66,15 +82,15 @@
         return dataset
 
     def concat_datasets(self, *datasets:pd.DataFrame) -> pd.DataFrame:
 
         return pd.concat(datasets, ignore_index=True)
 
     def get_train_val_test_datasets(self) -> tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame]:
-        raw_dataset = pd.read_parquet(self.DATASET_PATH)
+        raw_dataset = self.read_dataset(self.DATASET_PATH)
         cleaned_dataset, = self.clean_dataset(raw_dataset)
 
         #Shuffle the dataframe
         cleaned_dataset = cleaned_dataset.sample(frac=1, random_state=self._config.RANDOM_STATE)
 
         len_data = len(cleaned_dataset)
 
@@ -151,15 +167,15 @@
             scaler = pickle.load(open(scaler_path, 'rb'))
         else:
             scaler = self.fit_standard_scaler(columns)
 
         return scaler
 
     def fit_standard_scaler(self, columns:list[str]) -> sklearn.preprocessing.StandardScaler:
-        raw_dataset = pd.read_parquet(self.DATASET_PATH)
+        raw_dataset = self.read_dataset(self.DATASET_PATH)
         cleaned_dataset, = self.clean_dataset(raw_dataset)
 
         cleaned_dataset = cleaned_dataset[columns]
         cleaned_dataset = cleaned_dataset.to_numpy()
 
         scaler = sklearn.preprocessing.StandardScaler()
         scaler.fit(cleaned_dataset)
```

### Comparing `pyEasyML-1.0.1/pyEasyML/Data/FeatureSelection.py` & `pyEasyML-1.0.2/pyEasyML/Data/FeatureSelection.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.1/pyEasyML/Email/Email.py` & `pyEasyML-1.0.2/pyEasyML/Email/Email.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.1/pyEasyML/NeuralNetworks/AbstractANN.py` & `pyEasyML-1.0.2/pyEasyML/NeuralNetworks/AbstractANN.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.1/pyEasyML/NeuralNetworks/AnomalyDetection/AnomalyDetector.py` & `pyEasyML-1.0.2/pyEasyML/NeuralNetworks/AnomalyDetection/AnomalyDetector.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.1/pyEasyML/NeuralNetworks/AnomalyDetection/Factory.py` & `pyEasyML-1.0.2/pyEasyML/NeuralNetworks/AnomalyDetection/Factory.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.1/pyEasyML/NeuralNetworks/Autoencoders/ConvolutionalAutoencoder.py` & `pyEasyML-1.0.2/pyEasyML/NeuralNetworks/Autoencoders/ConvolutionalAutoencoder.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.1/pyEasyML/NeuralNetworks/Autoencoders/DeepAutoencoder.py` & `pyEasyML-1.0.2/pyEasyML/NeuralNetworks/Autoencoders/DeepAutoencoder.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.1/pyEasyML/NeuralNetworks/Layers/DeepAutoencoderLayers.py` & `pyEasyML-1.0.2/pyEasyML/NeuralNetworks/Layers/DeepAutoencoderLayers.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.1/pyEasyML/NeuralNetworks/Layers/Layers.py` & `pyEasyML-1.0.2/pyEasyML/NeuralNetworks/Layers/Layers.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.1/pyEasyML/Utils/ColumnsToID.py` & `pyEasyML-1.0.2/pyEasyML/Utils/ColumnsToID.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,44 +15,44 @@
 from Utils.Singleton import Singleton
 from Configs.Config import Config
 from os.path import exists
 
 class ColumnsToID(Singleton):
     def __init__(self) -> None:
         if not super().created:
-            self.__config = Config()
-            self.__CONVERT_DF_PATH = os.path.join(self.__config.get_utils_path(), 'columnsToID.csv')
+            self._config = Config()
+            self._CONVERT_DF_PATH = os.path.join(self._config.get_utils_path(), 'columnsToID.csv')
 
     def __load(self) -> pd.DataFrame:
-        if exists(self.__CONVERT_DF_PATH):
-            return pd.read_csv(self.__CONVERT_DF_PATH, index_col=0)
+        if exists(self._CONVERT_DF_PATH):
+            return pd.read_csv(self._CONVERT_DF_PATH, index_col=0)
         else:
             return pd.DataFrame(columns=['column', 'id'])
     
     def convert_columns_to_id(self, *columns) -> int:
         df = self.__load()
         converted_columns = []
         for column in columns:
             if column not in df['column'].values:
                 new_row = pd.DataFrame({'column': [column], 'id': [len(df)+1]})
                 df = pd.concat([df, new_row], ignore_index=True)
                 #df = df.append({'column': column, 'id': len(df)}, ignore_index=True)
-                df.to_csv(self.__CONVERT_DF_PATH)
+                df.to_csv(self._CONVERT_DF_PATH)
                 converted_columns.append(len(df) - 1)
             else:
                 column_id = df[df['column'] == column]['id'].values[0]
                 if column_id not in converted_columns:
                     converted_columns.append(column_id)
 
         converted_columns = sorted(converted_columns)
 
         return hash(int(''.join([str(column) for column in converted_columns])))
 
     def get_id(self, model_name:str) -> tuple[str]:
-        models_path = self.__config.get_trained_models_path()
+        models_path = self._config.get_trained_models_path()
         trained_models = os.listdir(models_path)
 
         for trained_model in trained_models:
             if model_name in trained_model:
                 splitted_file_name = trained_model.split('_')
                 columns_id, target_id, _ = tuple(splitted_file_name[1:])
```

### Comparing `pyEasyML-1.0.1/pyEasyML/Utils/Singleton.py` & `pyEasyML-1.0.2/pyEasyML/Utils/Singleton.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.1/pyEasyML/__init__.py` & `pyEasyML-1.0.2/pyEasyML/__init__.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.1/pyEasyML/pyEasyMLcli.py` & `pyEasyML-1.0.2/pyEasyML/pyEasyMLcli.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -44,16 +44,16 @@
     src_dir = os.path.join(current_dir, proj_name, 'src')
     os.makedirs(src_dir, exist_ok=True)
 
     # Create main file
     main_file_path = os.path.join(src_dir, 'main.py')
     with open(main_file_path, 'w') as main_file:
         main_file.write("import pyEasyML\n")
-        main_file.write("import os\n")
         main_file.write("from pyEasyML import Settings\n")
+        main_file.write("import os\n")
         main_file.write("settings = Settings(os.path.abspath(__file__))\n")
 
     click.echo("framework set up successfully!")
 
 @cli.command()
 def clean_normalization_models():
     current_dir = os.getcwd()
```

### Comparing `pyEasyML-1.0.1/pyEasyML.egg-info/PKG-INFO` & `pyEasyML-1.0.2/pyEasyML.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEasyML
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python machine learning framework.
 Author: Rodrigo Santos de Carvalho
 Author-email: <rodrigosc2401@gmail.com>
 Keywords: python,AI,Machine Learning,Neural Networks
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyEasyML-1.0.1/pyEasyML.egg-info/SOURCES.txt` & `pyEasyML-1.0.2/pyEasyML.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 pyEasyML/Classification/Models/LogisticRegression.py
 pyEasyML/Classification/Models/RandomForestClassifier.py
 pyEasyML/Classification/Models/SVC.py
 pyEasyML/Classification/Models/XGBClassifier.py
 pyEasyML/Classification/Models/__init__.py
 pyEasyML/Configs/Config.py
 pyEasyML/Configs/__init__.py
+pyEasyML/Customize/Extension.py
+pyEasyML/Customize/__init__.py
 pyEasyML/Data/DataPreprocessing.py
 pyEasyML/Data/FeatureSelection.py
 pyEasyML/Data/__init__.py
 pyEasyML/Email/Email.py
 pyEasyML/Email/__init__.py
 pyEasyML/NeuralNetworks/AbstractANN.py
 pyEasyML/NeuralNetworks/__init__.py
@@ -41,11 +43,10 @@
 pyEasyML/NeuralNetworks/Layers/ConvolutionalLayers.py
 pyEasyML/NeuralNetworks/Layers/DeepAutoencoderLayers.py
 pyEasyML/NeuralNetworks/Layers/Layers.py
 pyEasyML/NeuralNetworks/Layers/__init__.py
 pyEasyML/OutlierDetection/__init__.py
 pyEasyML/Regression/__init__.py
 pyEasyML/Utils/ColumnsToID.py
-pyEasyML/Utils/Extension.py
 pyEasyML/Utils/Singleton.py
 pyEasyML/Utils/Threshold.py
 pyEasyML/Utils/__init__.py
```

### Comparing `pyEasyML-1.0.1/setup.py` & `pyEasyML-1.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 DESCRIPTION = 'A python machine learning framework.'
 LONG_DESCRIPTION = 'A framework made to aid in the development of end-to-end machine learning projects, with data preprocessing, ml models, feature selection, hyperparameter tuning and much more.'
 
 # Setting up
 setup(
     name="pyEasyML",
     version=VERSION,
```

