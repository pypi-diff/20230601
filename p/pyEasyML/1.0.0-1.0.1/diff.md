# Comparing `tmp/pyEasyML-1.0.0.tar.gz` & `tmp/pyEasyML-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyEasyML-1.0.0.tar", last modified: Fri May 26 22:36:14 2023, max compression
+gzip compressed data, was "pyEasyML-1.0.1.tar", last modified: Thu Jun  1 13:41:25 2023, max compression
```

## Comparing `pyEasyML-1.0.0.tar` & `pyEasyML-1.0.1.tar`

### file list

```diff
@@ -1,69 +1,68 @@
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-26 22:36:14.659089 pyEasyML-1.0.0/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1083 2023-05-25 02:51:43.000000 pyEasyML-1.0.0/LICENSE
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      798 2023-05-26 22:36:14.659089 pyEasyML-1.0.0/PKG-INFO
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      166 2023-05-25 03:23:36.000000 pyEasyML-1.0.0/README.md
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-26 22:36:14.655087 pyEasyML-1.0.0/pyEasyML/
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-26 22:36:14.655087 pyEasyML-1.0.0/pyEasyML/Classification/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     5653 2023-05-25 05:16:03.000000 pyEasyML-1.0.0/pyEasyML/Classification/Classifier.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1609 2023-05-25 05:16:03.000000 pyEasyML-1.0.0/pyEasyML/Classification/Factory.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-26 22:36:14.655087 pyEasyML-1.0.0/pyEasyML/Classification/Models/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     4031 2023-05-25 05:16:03.000000 pyEasyML-1.0.0/pyEasyML/Classification/Models/AbstractModel.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      896 2023-05-25 05:16:03.000000 pyEasyML-1.0.0/pyEasyML/Classification/Models/GradientBoostingClassifier.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     3629 2023-05-25 03:30:02.000000 pyEasyML-1.0.0/pyEasyML/Classification/Models/IsolationForest.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1153 2023-05-25 05:10:03.000000 pyEasyML-1.0.0/pyEasyML/Classification/Models/KMeans.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      742 2023-05-25 05:10:03.000000 pyEasyML-1.0.0/pyEasyML/Classification/Models/KNeighborsClassifier.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      817 2023-05-25 05:10:03.000000 pyEasyML-1.0.0/pyEasyML/Classification/Models/LogisticRegression.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     4985 2023-05-25 05:10:03.000000 pyEasyML-1.0.0/pyEasyML/Classification/Models/OneClassSVM.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      845 2023-05-25 05:10:03.000000 pyEasyML-1.0.0/pyEasyML/Classification/Models/RandomForestClassifier.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      623 2023-05-25 05:10:03.000000 pyEasyML-1.0.0/pyEasyML/Classification/Models/SVC.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      844 2023-05-25 05:16:03.000000 pyEasyML-1.0.0/pyEasyML/Classification/Models/XGBClassifier.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-06 00:53:59.000000 pyEasyML-1.0.0/pyEasyML/Classification/Models/__init__.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1675 2023-05-25 05:16:03.000000 pyEasyML-1.0.0/pyEasyML/Classification/SearchModelsBestParams.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-06 00:53:30.000000 pyEasyML-1.0.0/pyEasyML/Classification/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-26 22:36:14.655087 pyEasyML-1.0.0/pyEasyML/Configs/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2427 2023-05-26 22:17:10.000000 pyEasyML-1.0.0/pyEasyML/Configs/Config.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-06 00:55:14.000000 pyEasyML-1.0.0/pyEasyML/Configs/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-26 22:36:14.655087 pyEasyML-1.0.0/pyEasyML/Data/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     6260 2023-05-26 21:49:19.000000 pyEasyML-1.0.0/pyEasyML/Data/DataPreprocessing.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     3692 2023-05-26 22:24:11.000000 pyEasyML-1.0.0/pyEasyML/Data/FeatureSelection.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-06 00:55:09.000000 pyEasyML-1.0.0/pyEasyML/Data/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-26 22:36:14.655087 pyEasyML-1.0.0/pyEasyML/Email/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2802 2023-05-25 05:16:03.000000 pyEasyML-1.0.0/pyEasyML/Email/Email.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-06 00:54:28.000000 pyEasyML-1.0.0/pyEasyML/Email/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-26 22:36:14.655087 pyEasyML-1.0.0/pyEasyML/NeuralNetworks/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2159 2023-05-25 05:16:03.000000 pyEasyML-1.0.0/pyEasyML/NeuralNetworks/AbstractANN.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-26 22:36:14.655087 pyEasyML-1.0.0/pyEasyML/NeuralNetworks/AnomalyDetection/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     5701 2023-05-25 05:16:03.000000 pyEasyML-1.0.0/pyEasyML/NeuralNetworks/AnomalyDetection/AnomalyDetector.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1163 2023-05-25 05:16:03.000000 pyEasyML-1.0.0/pyEasyML/NeuralNetworks/AnomalyDetection/Factory.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-17 21:11:32.000000 pyEasyML-1.0.0/pyEasyML/NeuralNetworks/AnomalyDetection/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-26 22:36:14.659089 pyEasyML-1.0.0/pyEasyML/NeuralNetworks/Autoencoders/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      941 2023-05-25 05:16:03.000000 pyEasyML-1.0.0/pyEasyML/NeuralNetworks/Autoencoders/ConvolutionalAutoencoder.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     5400 2023-05-25 05:16:03.000000 pyEasyML-1.0.0/pyEasyML/NeuralNetworks/Autoencoders/DeepAutoencoder.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-06 00:57:14.000000 pyEasyML-1.0.0/pyEasyML/NeuralNetworks/Autoencoders/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-26 22:36:14.659089 pyEasyML-1.0.0/pyEasyML/NeuralNetworks/Layers/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      383 2023-05-25 05:16:03.000000 pyEasyML-1.0.0/pyEasyML/NeuralNetworks/Layers/ConvolutionalLayers.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      783 2023-05-25 05:16:03.000000 pyEasyML-1.0.0/pyEasyML/NeuralNetworks/Layers/DeepAutoencoderLayers.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2093 2023-05-25 05:16:03.000000 pyEasyML-1.0.0/pyEasyML/NeuralNetworks/Layers/Layers.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-18 03:10:12.000000 pyEasyML-1.0.0/pyEasyML/NeuralNetworks/Layers/__init__.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-06 00:54:16.000000 pyEasyML-1.0.0/pyEasyML/NeuralNetworks/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-26 22:36:14.659089 pyEasyML-1.0.0/pyEasyML/OutlierDetection/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-17 21:11:39.000000 pyEasyML-1.0.0/pyEasyML/OutlierDetection/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-26 22:36:14.659089 pyEasyML-1.0.0/pyEasyML/Regression/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      326 2023-05-25 03:30:02.000000 pyEasyML-1.0.0/pyEasyML/Regression/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-26 22:36:14.659089 pyEasyML-1.0.0/pyEasyML/Utils/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2648 2023-05-25 03:30:02.000000 pyEasyML-1.0.0/pyEasyML/Utils/ColumnsToID.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      816 2023-05-25 04:01:06.000000 pyEasyML-1.0.0/pyEasyML/Utils/Extension.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      727 2023-05-25 06:02:13.000000 pyEasyML-1.0.0/pyEasyML/Utils/Singleton.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2927 2023-05-25 03:30:02.000000 pyEasyML-1.0.0/pyEasyML/Utils/Threshold.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-06 00:53:42.000000 pyEasyML-1.0.0/pyEasyML/Utils/__init__.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1333 2023-05-26 22:22:32.000000 pyEasyML-1.0.0/pyEasyML/__init__.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2174 2023-05-26 22:26:17.000000 pyEasyML-1.0.0/pyEasyML/pyEasyMLcli.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-26 22:36:14.655087 pyEasyML-1.0.0/pyEasyML.egg-info/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      798 2023-05-26 22:36:14.000000 pyEasyML-1.0.0/pyEasyML.egg-info/PKG-INFO
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1981 2023-05-26 22:36:14.000000 pyEasyML-1.0.0/pyEasyML.egg-info/SOURCES.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        1 2023-05-26 22:36:14.000000 pyEasyML-1.0.0/pyEasyML.egg-info/dependency_links.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       55 2023-05-26 22:36:14.000000 pyEasyML-1.0.0/pyEasyML.egg-info/entry_points.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       46 2023-05-26 22:36:14.000000 pyEasyML-1.0.0/pyEasyML.egg-info/requires.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        9 2023-05-26 22:36:14.000000 pyEasyML-1.0.0/pyEasyML.egg-info/top_level.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       38 2023-05-26 22:36:14.659089 pyEasyML-1.0.0/setup.cfg
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1192 2023-05-26 22:36:07.000000 pyEasyML-1.0.0/setup.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 13:41:25.145761 pyEasyML-1.0.1/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1083 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/LICENSE
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      743 2023-06-01 13:41:25.145761 pyEasyML-1.0.1/PKG-INFO
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      276 2023-06-01 13:39:31.000000 pyEasyML-1.0.1/README.md
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 13:41:25.141761 pyEasyML-1.0.1/pyEasyML/
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 13:41:25.141761 pyEasyML-1.0.1/pyEasyML/Classification/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     5653 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Classification/Classifier.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1609 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Classification/Factory.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 13:41:25.141761 pyEasyML-1.0.1/pyEasyML/Classification/Models/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     4031 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Classification/Models/AbstractModel.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      896 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Classification/Models/GradientBoostingClassifier.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     3629 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Classification/Models/IsolationForest.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1153 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Classification/Models/KMeans.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      827 2023-06-01 13:39:31.000000 pyEasyML-1.0.1/pyEasyML/Classification/Models/KNeighborsClassifier.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      817 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Classification/Models/LogisticRegression.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      778 2023-06-01 13:39:31.000000 pyEasyML-1.0.1/pyEasyML/Classification/Models/RandomForestClassifier.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      623 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Classification/Models/SVC.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      844 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Classification/Models/XGBClassifier.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Classification/Models/__init__.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1675 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Classification/SearchModelsBestParams.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Classification/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 13:41:25.141761 pyEasyML-1.0.1/pyEasyML/Configs/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2681 2023-06-01 13:39:31.000000 pyEasyML-1.0.1/pyEasyML/Configs/Config.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Configs/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 13:41:25.141761 pyEasyML-1.0.1/pyEasyML/Data/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     6232 2023-06-01 13:39:31.000000 pyEasyML-1.0.1/pyEasyML/Data/DataPreprocessing.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     3692 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Data/FeatureSelection.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Data/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 13:41:25.141761 pyEasyML-1.0.1/pyEasyML/Email/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2802 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Email/Email.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Email/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 13:41:25.141761 pyEasyML-1.0.1/pyEasyML/NeuralNetworks/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2159 2023-05-31 04:12:00.000000 pyEasyML-1.0.1/pyEasyML/NeuralNetworks/AbstractANN.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 13:41:25.141761 pyEasyML-1.0.1/pyEasyML/NeuralNetworks/AnomalyDetection/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     5595 2023-06-01 13:39:31.000000 pyEasyML-1.0.1/pyEasyML/NeuralNetworks/AnomalyDetection/AnomalyDetector.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1163 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/NeuralNetworks/AnomalyDetection/Factory.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/NeuralNetworks/AnomalyDetection/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 13:41:25.145761 pyEasyML-1.0.1/pyEasyML/NeuralNetworks/Autoencoders/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      941 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/NeuralNetworks/Autoencoders/ConvolutionalAutoencoder.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     6614 2023-06-01 13:39:31.000000 pyEasyML-1.0.1/pyEasyML/NeuralNetworks/Autoencoders/DeepAutoencoder.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/NeuralNetworks/Autoencoders/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 13:41:25.145761 pyEasyML-1.0.1/pyEasyML/NeuralNetworks/Layers/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      383 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/NeuralNetworks/Layers/ConvolutionalLayers.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      783 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/NeuralNetworks/Layers/DeepAutoencoderLayers.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2092 2023-06-01 13:39:31.000000 pyEasyML-1.0.1/pyEasyML/NeuralNetworks/Layers/Layers.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/NeuralNetworks/Layers/__init__.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/NeuralNetworks/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 13:41:25.145761 pyEasyML-1.0.1/pyEasyML/OutlierDetection/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/OutlierDetection/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 13:41:25.145761 pyEasyML-1.0.1/pyEasyML/Regression/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      326 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Regression/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 13:41:25.145761 pyEasyML-1.0.1/pyEasyML/Utils/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2630 2023-06-01 13:39:31.000000 pyEasyML-1.0.1/pyEasyML/Utils/ColumnsToID.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      816 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Utils/Extension.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      727 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Utils/Singleton.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     3018 2023-06-01 13:39:31.000000 pyEasyML-1.0.1/pyEasyML/Utils/Threshold.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.1/pyEasyML/Utils/__init__.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1282 2023-06-01 13:39:31.000000 pyEasyML-1.0.1/pyEasyML/__init__.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2727 2023-06-01 13:39:31.000000 pyEasyML-1.0.1/pyEasyML/pyEasyMLcli.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 13:41:25.141761 pyEasyML-1.0.1/pyEasyML.egg-info/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      743 2023-06-01 13:41:25.000000 pyEasyML-1.0.1/pyEasyML.egg-info/PKG-INFO
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1935 2023-06-01 13:41:25.000000 pyEasyML-1.0.1/pyEasyML.egg-info/SOURCES.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        1 2023-06-01 13:41:25.000000 pyEasyML-1.0.1/pyEasyML.egg-info/dependency_links.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       54 2023-06-01 13:41:25.000000 pyEasyML-1.0.1/pyEasyML.egg-info/entry_points.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       46 2023-06-01 13:41:25.000000 pyEasyML-1.0.1/pyEasyML.egg-info/requires.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        9 2023-06-01 13:41:25.000000 pyEasyML-1.0.1/pyEasyML.egg-info/top_level.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       38 2023-06-01 13:41:25.145761 pyEasyML-1.0.1/setup.cfg
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1192 2023-06-01 13:40:46.000000 pyEasyML-1.0.1/setup.py
```

### Comparing `pyEasyML-1.0.0/LICENSE` & `pyEasyML-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.0/pyEasyML/Classification/Classifier.py` & `pyEasyML-1.0.1/pyEasyML/Classification/Classifier.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.0/pyEasyML/Classification/Factory.py` & `pyEasyML-1.0.1/pyEasyML/Classification/Factory.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.0/pyEasyML/Classification/Models/AbstractModel.py` & `pyEasyML-1.0.1/pyEasyML/Classification/Models/AbstractModel.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.0/pyEasyML/Classification/Models/GradientBoostingClassifier.py` & `pyEasyML-1.0.1/pyEasyML/Classification/Models/GradientBoostingClassifier.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.0/pyEasyML/Classification/Models/IsolationForest.py` & `pyEasyML-1.0.1/pyEasyML/Classification/Models/IsolationForest.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.0/pyEasyML/Classification/Models/KMeans.py` & `pyEasyML-1.0.1/pyEasyML/Classification/Models/KMeans.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.0/pyEasyML/Classification/Models/LogisticRegression.py` & `pyEasyML-1.0.1/pyEasyML/Classification/Models/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.0/pyEasyML/Classification/Models/SVC.py` & `pyEasyML-1.0.1/pyEasyML/Classification/Models/SVC.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.0/pyEasyML/Classification/Models/XGBClassifier.py` & `pyEasyML-1.0.1/pyEasyML/Classification/Models/XGBClassifier.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.0/pyEasyML/Classification/SearchModelsBestParams.py` & `pyEasyML-1.0.1/pyEasyML/Classification/SearchModelsBestParams.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.0/pyEasyML/Configs/Config.py` & `pyEasyML-1.0.1/pyEasyML/Configs/Config.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,27 +24,35 @@
             instances[cls] = cls(*args, **kwargs)
         return instances[cls]
 
     return wrapper
 
 @singleton
 class Config():
-    def __init__(self) -> None:
-        self.__configs:dict[str, str] = {"client": "/home/rodrigo/Documents/Personal/test"}
+    def __init__(self, client:str) -> None:
+        self.__configs:dict[str, str] = self.__load_configs(client)
         self.__client:str = self.__configs['client']
         self.__SELECTED_FEATURES:list[str] = []
         self.__TARGET_FEATURE:str = "NOT DEFINED"
         self.__RANDOM_STATE:int = 0
 
-    def __load_configs(self) -> dict[str, str]:
-        json_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'configs.json')
-        with open(json_path, 'r') as file:
-            configs = json.load(file)
-    
-        return configs
+    def __load_configs(self, client: str) -> dict[str, str]:
+        start = client
+
+        for tries in range(100):
+            json_path = os.path.join(start, 'configs.json')
+            if os.path.exists(json_path):
+                with open(json_path, 'r') as file:
+                    configs = json.load(file)
+                    return configs
+            else:
+                parent_dir = os.path.dirname(os.path.dirname(start))
+                start = parent_dir
+
+        return {'client': 'NOT DEFINED'}
 
     @property
     def SELECTED_FEATURES(self) -> list[str]:
         return self.__SELECTED_FEATURES
 
     @SELECTED_FEATURES.setter
     def SELECTED_FEATURES(self, selected_features:list[str]) -> None:
```

### Comparing `pyEasyML-1.0.0/pyEasyML/Data/DataPreprocessing.py` & `pyEasyML-1.0.1/pyEasyML/Data/DataPreprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,14 @@
             target_column = self._config.TARGET_FEATURE
 
         if target_column in columns:
             X = dataset[columns].drop(labels=[self._config.TARGET_FEATURE], axis=1)
             columns.remove(self._config.TARGET_FEATURE)
         else:
             X = dataset[columns]
-        print(self._config)
         Y = dataset[target_column]
 
         X_train, X_test, Y_train, Y_test = sklearn.model_selection.train_test_split(
             X.to_numpy(), 
             Y.to_numpy(), 
             test_size=0.3, 
             #shuffle=True, #Shuffle is already done in the clean_dataset function.
```

### Comparing `pyEasyML-1.0.0/pyEasyML/Data/FeatureSelection.py` & `pyEasyML-1.0.1/pyEasyML/Data/FeatureSelection.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.0/pyEasyML/Email/Email.py` & `pyEasyML-1.0.1/pyEasyML/Email/Email.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.0/pyEasyML/NeuralNetworks/AbstractANN.py` & `pyEasyML-1.0.1/pyEasyML/NeuralNetworks/AbstractANN.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.0/pyEasyML/NeuralNetworks/AnomalyDetection/AnomalyDetector.py` & `pyEasyML-1.0.1/pyEasyML/NeuralNetworks/AnomalyDetection/AnomalyDetector.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,16 +52,15 @@
             columns = self._config.SELECTED_FEATURES
 
         columns_id = ColumnsToID().convert_columns_to_id(*columns)
 
         return columns_id
 
     def __get_model(self, model_name:str, **params:dict[str, Any]) -> AbstractANN:
-        model = Factory().create(model_name, **params)
-        model.columns_id = self._columns_id
+        model = Factory().create(model_name, columns_id=self._columns_id, **params)
         
         return model
 
     def __get_thresholds(self, model_name:str) -> list[Threshold]:
         thresholds = []
         columns_id = [ColumnsToID().column_id(column) for column in self._columns]
         for column_id in columns_id:
@@ -84,31 +83,30 @@
     @thresholds.setter
     def thresholds(self, thresholds:list[float]) -> None:
         for threshold, new_value in zip(self._thresholds, thresholds):
             threshold.value = new_value
 
     def train(self, X_train:np.ndarray, re_train:bool=False, **fit_params:dict[str, Any]) -> bool:
         model_is_trained = self._verify_if_model_trained()
-        
-        if model_is_trained and not re_train:
-            return True
-        elif not model_is_trained and not re_train:
-            raise Exception("Model not trained and re_train is False.")
 
-        self._model.fit(X_train, **fit_params)
+        if not model_is_trained or re_train:
+            self._model.fit(X_train, **fit_params)
 
-        healthy_reconstrution = self._model.predict(X_train)
-        for column_index in range(len(self._thresholds)):
-            self._thresholds[column_index].value = self.__reconstruction_mae_loss(original=X_train[:,column_index], reconstructed=healthy_reconstrution[:,column_index])
+            healthy_reconstrution = self._model.predict(X_train)
+            
+            for column_index in range(len(self._thresholds)):
+                self._thresholds[column_index].value = self.__reconstruction_mae_loss(original=X_train[:,column_index], reconstructed=healthy_reconstrution[:,column_index])
+        
+        return True
         
     def _verify_if_model_trained(self) -> bool:
         columns_id_str = ColumnsToID().convert_columns_to_id(*self._columns)
         target_id_str = '0'
 
-        if exists(self._config.get_trained_models_path() + f'{self._model.__class__.__name__}_{columns_id_str}_{target_id_str}_model.sav'):
+        if exists(self._config.get_trained_models_path() + f'{self._model.__class__.__name__}{columns_id_str}{target_id_str}.h5'):
             return True
         else:
             False
 
     def __reconstruction_mae_loss(self, original:np.ndarray, reconstructed:np.ndarray) -> float:
         loss = self.__reconstruction_loss(original, reconstructed)
         mae_loss = np.mean(loss)
@@ -116,25 +114,25 @@
         return mae_loss
 
     def __reconstruction_loss(self, original:np.ndarray, reconstructed:np.ndarray) -> np.ndarray:
         loss = np.abs(original - reconstructed)
         
         return loss
 
-    def detect(self, dataset:np.ndarray, minimum_anomalous_vars:int=1) -> np.ndarray:
+    def detect(self, dataset:np.ndarray, minimum_anomalous_vars:int=1, threshold_factor:float=1.0) -> np.ndarray:
         reconstructed = self._model.predict(dataset)
 
         losses = []
         for var in range(dataset.shape[1]):
             losses.append(self.__reconstruction_loss(original=dataset[:,var], reconstructed=reconstructed[:,var]))
 
         vectorized_verify_if_is_anomaly = np.vectorize(self.__verify_if_is_anomaly)
         detections = []
         for loss, threshold in zip(losses, self._thresholds):
-            detection = vectorized_verify_if_is_anomaly(loss=loss, threshold=threshold)
+            detection = vectorized_verify_if_is_anomaly(loss=loss, threshold=threshold*threshold_factor)
             detections.append(detection)
 
         detections = np.column_stack(detections)
         detections = np.apply_along_axis(self.__verify_minimum_anomalous_vars, axis=1, arr=detections, minimum_anomalous_vars=minimum_anomalous_vars)
 
         return detections
 
@@ -146,15 +144,13 @@
 
     def __verify_minimum_anomalous_vars(self, row:Any, minimum_anomalous_vars:int) -> np.ndarray:
         if np.sum(row) >= minimum_anomalous_vars:
             return 1.0
         else:
             return 0.0
 
-    def evaluate(self, X_test:np.ndarray, Y_test:np.ndarray) -> np.ndarray:
-        detections = self.detect(dataset=X_test)
-
+    def evaluate(self, X_test:np.ndarray, Y_test:np.ndarray, detections:np.ndarray) -> np.ndarray:
         cm = confusion_matrix(y_true=Y_test, y_pred=detections)
         report = classification_report(y_true=Y_test, y_pred=detections)
         print(report)
 
         return cm
```

### Comparing `pyEasyML-1.0.0/pyEasyML/NeuralNetworks/AnomalyDetection/Factory.py` & `pyEasyML-1.0.1/pyEasyML/NeuralNetworks/AnomalyDetection/Factory.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.0/pyEasyML/NeuralNetworks/Autoencoders/ConvolutionalAutoencoder.py` & `pyEasyML-1.0.1/pyEasyML/NeuralNetworks/Autoencoders/ConvolutionalAutoencoder.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.0/pyEasyML/NeuralNetworks/Layers/DeepAutoencoderLayers.py` & `pyEasyML-1.0.1/pyEasyML/NeuralNetworks/Layers/DeepAutoencoderLayers.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.0/pyEasyML/NeuralNetworks/Layers/Layers.py` & `pyEasyML-1.0.1/pyEasyML/NeuralNetworks/Layers/Layers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os, sys, re
 
 # Evitando a criação de arquivos .pyc
 sys.dont_write_bytecode = True
 
 script_dir = os.path.abspath(__file__)
 
-
 # Apagando o nome do arquivo e deixando apenas o diretorio.
 script_dir = re.sub(pattern="pyEasyML.*", repl = "pyEasyML/", string = script_dir)
 
 script_dir = os.path.abspath(script_dir)
 
 os.chdir(script_dir)
```

### Comparing `pyEasyML-1.0.0/pyEasyML/Utils/ColumnsToID.py` & `pyEasyML-1.0.1/pyEasyML/Utils/ColumnsToID.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 script_dir = os.path.abspath(__file__)
 
 # Apagando o nome do arquivo e deixando apenas o diretorio.
 script_dir = re.sub(pattern="pyEasyML.*", repl = "pyEasyML/", string = script_dir)
 
 os.chdir(script_dir)
-print(script_dir)
 sys.path.append(script_dir)
 
 import pandas as pd
 from Utils.Singleton import Singleton
 from Configs.Config import Config
 from os.path import exists
```

### Comparing `pyEasyML-1.0.0/pyEasyML/Utils/Extension.py` & `pyEasyML-1.0.1/pyEasyML/Utils/Extension.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.0/pyEasyML/Utils/Singleton.py` & `pyEasyML-1.0.1/pyEasyML/Utils/Singleton.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.0/pyEasyML/Utils/Threshold.py` & `pyEasyML-1.0.1/pyEasyML/Utils/Threshold.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         self.__model = model
         self.__column_id = column_id
 
         if value is not None:
             self.__value = value
         else:
             self.__value = self.__get()
-
+            
     def __load(self) -> pd.DataFrame:
         if exists(self.__THRESHOLD_DF_PATH):
             return pd.read_csv(self.__THRESHOLD_DF_PATH, index_col=0)
         else:
             df = pd.DataFrame(columns=['model', 'column_id', 'threshold'])
             df.to_csv(self.__THRESHOLD_DF_PATH, index=True)
             return df 
@@ -48,29 +48,34 @@
             threshold = self.__df[(self.__df['model'] == self.__model) & (self.__df['column_id'] == self.__column_id)]['threshold']
             if threshold.empty:
                 return 0
             else:
                 return threshold.values[0]
 
     def __set(self, value: float) -> None:
+        self.__df = self.__load()
+        
         df = self.__df[(self.__df['model'] == self.__model) & (self.__df['column_id'] == self.__column_id)]
         if df.empty:
-            new_row = {'model': self.__model, 'column_id': self.__column_id, 'threshold': value}
-            self.__df = self.__df.append(new_row, ignore_index=True)
+            new_row = pd.DataFrame({'model': [self.__model], 'column_id': [self.__column_id], 'threshold': [value]})
+            self.__df = pd.concat([self.__df, new_row], ignore_index=True)
         else:
-            row = df[['threshold']]
-            threshold = row.values[0]
-            if threshold != value:
-                self.__df.loc[(self.__df['model'] == self.__model) & (self.__df['column_id'] == self.__column_id), 'threshold'] = value
+            row_index = df.index[0]
+            if self.__df.at[row_index, 'threshold'] != value:
+                self.__df.at[row_index, 'threshold'] = value
             else:
                 return
 
         self.__value = value
         self.__save()
 
+    def __mul__(self, value: float) -> None:
+        self.__value *= value
+        return self
+
     def __str__(self) -> str:
         return f'Threshold: {self.__value}'
 
     def __repr__(self) -> str:
         return f'Threshold: {self.__value}'
 
     @property
```

### Comparing `pyEasyML-1.0.0/pyEasyML/__init__.py` & `pyEasyML-1.0.1/pyEasyML/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,39 +13,34 @@
 os.chdir(script_dir)
 
 sys.path.append(os.path.join(script_dir))
 
 from Configs.Config import Config
 
 class Settings:
-    config = Config()
+    def __init__(self, client:str) -> None:
+        self._config = Config(client)
 
-    @staticmethod
-    def set_target_feature(target_feature:str) -> None:
-        config = Settings.config
+    def set_target_feature(self,target_feature:str) -> None:
+        config = self._config
         config.TARGET_FEATURE = target_feature
 
-    @staticmethod    
-    def set_selected_features(selected_features:list[str]) -> None:
-        config = Settings.config
+    def set_selected_features(self,selected_features:list[str]) -> None:
+        config = self._config
         config.SELECTED_FEATURES = selected_features
 
-    @staticmethod    
-    def set_random_state(random_state:int) -> None:
-        config = Settings.config
+    def set_random_state(self,random_state:int) -> None:
+        config = self._config
         config.RANDOM_STATE = random_state
 
-    @staticmethod    
-    def get_target_feature() -> str:
-        config = Settings.config
+    def get_target_feature(self) -> str:
+        config = self._config
         return config.TARGET_FEATURE
 
-    @staticmethod
-    def get_selected_features() -> list[str]:
-        config = Settings.config
+    def get_selected_features(self) -> list[str]:
+        config = self._config
         return config.SELECTED_FEATURES
 
-    @staticmethod
-    def get_random_state() -> int:
-        config = Settings.config
+    def get_random_state(self) -> int:
+        config = self._config
         return config.RANDOM_STATE
```

### Comparing `pyEasyML-1.0.0/pyEasyML/pyEasyMLcli.py` & `pyEasyML-1.0.1/pyEasyML/pyEasyMLcli.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,66 +1,80 @@
 
 # Evitando a criação de arquivos .pyc
 import sys
 sys.dont_write_bytecode = True
 # pyEasyMLcli.py
 import os
-import re
 import click
 import json
 
 @click.group()
 def cli():
     pass
 
 @cli.command()
-def start():
+@click.argument('current_dir', default='.', type=click.Path(exists=True))
+def start(current_dir):
     click.echo("Seting framework up...")
-    script_dir = os.path.abspath(__file__)
-    script_dir = re.sub(pattern="pyEasyML.*", repl = "pyEasyML/", string = script_dir)
-    script_dir = os.path.abspath(script_dir)
-    
     # dir from where the script is being executed
-    current_dir = os.getcwd()
+    current_dir = os.path.abspath(current_dir)
+    
+    proj_name = input("Project name: ")
     
     # folders important to the framework
-    models_dir = os.path.join(current_dir, 'models')
-    utils_dir = os.path.join(current_dir, 'Utils')
-    dataset_dir = os.path.join(current_dir, 'dataset')
+    models_dir = os.path.join(current_dir, proj_name, 'models')
+    utils_dir = os.path.join(current_dir, proj_name, 'Utils')
+    dataset_dir = os.path.join(current_dir, proj_name, 'dataset')
     normalization_model_dir = os.path.join(models_dir, 'normalizationModel')
     
     # Create directories if they don't exist
     os.makedirs(models_dir, exist_ok=True)
     os.makedirs(utils_dir, exist_ok=True)
     os.makedirs(dataset_dir, exist_ok=True)
     os.makedirs(normalization_model_dir, exist_ok=True)
 
     # config data that'll save the client's folder
     config_data = {
-        'client': current_dir
+        'client': os.path.join(current_dir, proj_name)
     }
-    config_file_path = os.path.join(script_dir, 'Configs', 'configs.json')
+    config_file_path = os.path.join(current_dir, proj_name, 'configs.json')
     with open(config_file_path, 'w') as config_file:
         json.dump(config_data, config_file, indent=4)
+    
+    # Create src folder
+    src_dir = os.path.join(current_dir, proj_name, 'src')
+    os.makedirs(src_dir, exist_ok=True)
+
+    # Create main file
+    main_file_path = os.path.join(src_dir, 'main.py')
+    with open(main_file_path, 'w') as main_file:
+        main_file.write("import pyEasyML\n")
+        main_file.write("import os\n")
+        main_file.write("from pyEasyML import Settings\n")
+        main_file.write("settings = Settings(os.path.abspath(__file__))\n")
 
     click.echo("framework set up successfully!")
-    
+
 @cli.command()
 def clean_normalization_models():
+    current_dir = os.getcwd()
+    
     click.echo("Cleaning normalization model...")
-    normalization_model_dir = os.path.join(script_dir, 'models', 'normalizationModel')
+    normalization_model_dir = os.path.join(current_dir, 'models', 'normalizationModel')
     for file in os.listdir(normalization_model_dir):
         file_path = os.path.join(normalization_model_dir, file)
         os.remove(file_path)
     click.echo("Normalization model cleaned successfully!")
-    
+
 @cli.command()
 def clean_models():
+    current_dir = os.getcwd()
+    
     click.echo("Cleaning models...")
-    models_dir = os.path.join(script_dir, 'models')
+    models_dir = os.path.join(current_dir, 'models')
     for file in os.listdir(models_dir):
         file_path = os.path.join(models_dir, file)
         if os.path.isfile(file_path) and file != 'normalizationModel':
             os.remove(file_path)
     click.echo("Models cleaned successfully!")
 
 if __name__ == '__main__':
```

### Comparing `pyEasyML-1.0.0/pyEasyML.egg-info/SOURCES.txt` & `pyEasyML-1.0.1/pyEasyML.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 pyEasyML/Classification/__init__.py
 pyEasyML/Classification/Models/AbstractModel.py
 pyEasyML/Classification/Models/GradientBoostingClassifier.py
 pyEasyML/Classification/Models/IsolationForest.py
 pyEasyML/Classification/Models/KMeans.py
 pyEasyML/Classification/Models/KNeighborsClassifier.py
 pyEasyML/Classification/Models/LogisticRegression.py
-pyEasyML/Classification/Models/OneClassSVM.py
 pyEasyML/Classification/Models/RandomForestClassifier.py
 pyEasyML/Classification/Models/SVC.py
 pyEasyML/Classification/Models/XGBClassifier.py
 pyEasyML/Classification/Models/__init__.py
 pyEasyML/Configs/Config.py
 pyEasyML/Configs/__init__.py
 pyEasyML/Data/DataPreprocessing.py
```

### Comparing `pyEasyML-1.0.0/setup.py` & `pyEasyML-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = 'A python machine learning framework.'
 LONG_DESCRIPTION = 'A framework made to aid in the development of end-to-end machine learning projects, with data preprocessing, ml models, feature selection, hyperparameter tuning and much more.'
 
 # Setting up
 setup(
     name="pyEasyML",
     version=VERSION,
```

