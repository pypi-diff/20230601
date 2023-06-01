# Comparing `tmp/tracebloc_package-dev-0.4.1.tar.gz` & `tmp/tracebloc_package-dev-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracebloc_package-dev-0.4.1.tar", last modified: Fri May 26 10:05:32 2023, max compression
+gzip compressed data, was "tracebloc_package-dev-0.4.2.tar", last modified: Thu Jun  1 09:08:14 2023, max compression
```

## Comparing `tracebloc_package-dev-0.4.1.tar` & `tracebloc_package-dev-0.4.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-05-26 10:05:32.783309 tracebloc_package-dev-0.4.1/
--rw-r--r--   0 divyasingh   (501) staff       (20)     1048 2022-05-03 09:10:47.000000 tracebloc_package-dev-0.4.1/LICENSE.txt
--rw-r--r--   0 divyasingh   (501) staff       (20)      558 2023-05-26 10:05:32.783599 tracebloc_package-dev-0.4.1/PKG-INFO
--rw-r--r--   0 divyasingh   (501) staff       (20)      188 2022-05-03 09:10:47.000000 tracebloc_package-dev-0.4.1/README.md
--rw-r--r--   0 divyasingh   (501) staff       (20)       78 2023-05-26 10:05:32.784241 tracebloc_package-dev-0.4.1/setup.cfg
--rw-r--r--   0 divyasingh   (501) staff       (20)      949 2023-05-26 10:04:20.000000 tracebloc_package-dev-0.4.1/setup.py
-drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-05-26 10:05:32.780567 tracebloc_package-dev-0.4.1/tracebloc_package/
--rw-r--r--   0 divyasingh   (501) staff       (20)       67 2023-03-16 07:45:22.000000 tracebloc_package-dev-0.4.1/tracebloc_package/__init__.py
--rw-r--r--   0 divyasingh   (501) staff       (20)     5669 2023-05-19 09:01:53.000000 tracebloc_package-dev-0.4.1/tracebloc_package/check_parameters.py
--rw-r--r--   0 divyasingh   (501) staff       (20)    20852 2023-05-26 09:12:37.000000 tracebloc_package-dev-0.4.1/tracebloc_package/functional_test.py
--rw-r--r--   0 divyasingh   (501) staff       (20)    59111 2023-05-24 09:14:21.000000 tracebloc_package-dev-0.4.1/tracebloc_package/linkModelDataSet.py
--rw-r--r--   0 divyasingh   (501) staff       (20)     7100 2022-07-01 07:02:58.000000 tracebloc_package-dev-0.4.1/tracebloc_package/messages.py
--rw-r--r--   0 divyasingh   (501) staff       (20)     8594 2023-05-25 06:18:17.000000 tracebloc_package-dev-0.4.1/tracebloc_package/upload.py
--rw-r--r--   0 divyasingh   (501) staff       (20)    10203 2023-05-25 09:39:24.000000 tracebloc_package-dev-0.4.1/tracebloc_package/user.py
--rw-r--r--   0 divyasingh   (501) staff       (20)     5839 2023-05-23 18:03:05.000000 tracebloc_package-dev-0.4.1/tracebloc_package/utils.py
--rw-r--r--   0 divyasingh   (501) staff       (20)     3203 2022-06-09 14:39:28.000000 tracebloc_package-dev-0.4.1/tracebloc_package/weights.py
-drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-05-26 10:05:32.782956 tracebloc_package-dev-0.4.1/tracebloc_package_dev.egg-info/
--rw-r--r--   0 divyasingh   (501) staff       (20)      558 2023-05-26 10:05:32.000000 tracebloc_package-dev-0.4.1/tracebloc_package_dev.egg-info/PKG-INFO
--rw-r--r--   0 divyasingh   (501) staff       (20)      591 2023-05-26 10:05:32.000000 tracebloc_package-dev-0.4.1/tracebloc_package_dev.egg-info/SOURCES.txt
--rw-r--r--   0 divyasingh   (501) staff       (20)        1 2023-05-26 10:05:32.000000 tracebloc_package-dev-0.4.1/tracebloc_package_dev.egg-info/dependency_links.txt
--rw-r--r--   0 divyasingh   (501) staff       (20)        1 2023-05-26 10:05:32.000000 tracebloc_package-dev-0.4.1/tracebloc_package_dev.egg-info/not-zip-safe
--rw-r--r--   0 divyasingh   (501) staff       (20)      119 2023-05-26 10:05:32.000000 tracebloc_package-dev-0.4.1/tracebloc_package_dev.egg-info/requires.txt
--rw-r--r--   0 divyasingh   (501) staff       (20)       18 2023-05-26 10:05:32.000000 tracebloc_package-dev-0.4.1/tracebloc_package_dev.egg-info/top_level.txt
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-01 09:08:14.975252 tracebloc_package-dev-0.4.2/
+-rw-r--r--   0 hasan      (501) staff       (20)     1048 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.4.2/LICENSE.txt
+-rw-r--r--   0 hasan      (501) staff       (20)      577 2023-06-01 09:08:14.975316 tracebloc_package-dev-0.4.2/PKG-INFO
+-rw-r--r--   0 hasan      (501) staff       (20)      188 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.4.2/README.md
+-rw-r--r--   0 hasan      (501) staff       (20)       78 2023-06-01 09:08:14.975553 tracebloc_package-dev-0.4.2/setup.cfg
+-rw-r--r--   0 hasan      (501) staff       (20)      949 2023-06-01 09:07:14.000000 tracebloc_package-dev-0.4.2/setup.py
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-01 09:08:14.974160 tracebloc_package-dev-0.4.2/tracebloc_package/
+-rw-r--r--   0 hasan      (501) staff       (20)       67 2023-03-15 10:59:39.000000 tracebloc_package-dev-0.4.2/tracebloc_package/__init__.py
+-rw-r--r--   0 hasan      (501) staff       (20)     5669 2023-05-18 09:32:19.000000 tracebloc_package-dev-0.4.2/tracebloc_package/check_parameters.py
+-rw-r--r--   0 hasan      (501) staff       (20)    20998 2023-06-01 09:06:49.000000 tracebloc_package-dev-0.4.2/tracebloc_package/functional_test.py
+-rw-r--r--   0 hasan      (501) staff       (20)    60056 2023-06-01 09:06:49.000000 tracebloc_package-dev-0.4.2/tracebloc_package/linkModelDataSet.py
+-rw-r--r--   0 hasan      (501) staff       (20)     7100 2023-03-23 11:28:43.000000 tracebloc_package-dev-0.4.2/tracebloc_package/messages.py
+-rw-r--r--   0 hasan      (501) staff       (20)     9777 2023-06-01 09:06:49.000000 tracebloc_package-dev-0.4.2/tracebloc_package/upload.py
+-rw-r--r--   0 hasan      (501) staff       (20)    10203 2023-06-01 06:15:22.000000 tracebloc_package-dev-0.4.2/tracebloc_package/user.py
+-rw-r--r--   0 hasan      (501) staff       (20)     5840 2023-06-01 09:06:49.000000 tracebloc_package-dev-0.4.2/tracebloc_package/utils.py
+-rw-r--r--   0 hasan      (501) staff       (20)     3203 2022-06-09 05:22:24.000000 tracebloc_package-dev-0.4.2/tracebloc_package/weights.py
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-01 09:08:14.975142 tracebloc_package-dev-0.4.2/tracebloc_package_dev.egg-info/
+-rw-r--r--   0 hasan      (501) staff       (20)      577 2023-06-01 09:08:14.000000 tracebloc_package-dev-0.4.2/tracebloc_package_dev.egg-info/PKG-INFO
+-rw-r--r--   0 hasan      (501) staff       (20)      591 2023-06-01 09:08:14.000000 tracebloc_package-dev-0.4.2/tracebloc_package_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 hasan      (501) staff       (20)        1 2023-06-01 09:08:14.000000 tracebloc_package-dev-0.4.2/tracebloc_package_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 hasan      (501) staff       (20)        1 2023-06-01 09:08:14.000000 tracebloc_package-dev-0.4.2/tracebloc_package_dev.egg-info/not-zip-safe
+-rw-r--r--   0 hasan      (501) staff       (20)      119 2023-06-01 09:08:14.000000 tracebloc_package-dev-0.4.2/tracebloc_package_dev.egg-info/requires.txt
+-rw-r--r--   0 hasan      (501) staff       (20)       18 2023-06-01 09:08:14.000000 tracebloc_package-dev-0.4.2/tracebloc_package_dev.egg-info/top_level.txt
```

### Comparing `tracebloc_package-dev-0.4.1/LICENSE.txt` & `tracebloc_package-dev-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.1/PKG-INFO` & `tracebloc_package-dev-0.4.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: tracebloc_package-dev
-Version: 0.4.1
+Version: 0.4.2
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
+Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Tracebloc package
 This packeg is pre-requiste to run tracebloc jupyter notebook.
 
 
 This package helps to create and start the experiment for training ML models in 
 tracebloc environment.
+
```

### Comparing `tracebloc_package-dev-0.4.1/setup.py` & `tracebloc_package-dev-0.4.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="tracebloc_package-dev",
-    version="0.4.1",
+    version="0.4.2",
     description="Package required to run Tracebloc jupyter notebook to create experiment",
     url="https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev",
     license="MIT",
     python_requires=">=3",
     packages=["tracebloc_package"],
     author="Tracebloc",
     author_email="info@tracebloc.io",
```

### Comparing `tracebloc_package-dev-0.4.1/tracebloc_package/check_parameters.py` & `tracebloc_package-dev-0.4.2/tracebloc_package/check_parameters.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.1/tracebloc_package/functional_test.py` & `tracebloc_package-dev-0.4.2/tracebloc_package/functional_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     notallowed = ["__MACOSX", "__pycache__"]
     input_shape_patt = re.compile("(^input_shape\s{0,}[=]\s{0,}[a-zA-Z_\-0-9'\"])")
     out_classes_patt = re.compile("(^output_classes\s{0,}[=]\s{0,}[a-zA-Z_\-0-9'\"])")
     main_method_patt = re.compile("(^main_method\s{0,}[=]\s{0,}[a-zA-Z_\-0-9'\"])")
     main_class_patt = re.compile("(^main_class\s{0,}[=]\s{0,}[a-zA-Z_\-0-9'\"])")
     framework_patt = re.compile("(^framework\s{0,}[=]\s{0,}[a-zA-Z_\-0-9'\"])")
 
-
     def __init__(
         self, progress_bar, model_name=None, model_path=None
     ):  # pragma: no cover
         self.model_name = model_name
         self.model_path = model_path
         self.progress_bar = progress_bar
 
@@ -52,15 +51,15 @@
                     self.add_method(temp_file, remove_lines)
                 else:
                     self.edit_file(temp_file, filelines, remove_lines)
             elif self.framework == PYTORCH_FRAMEWORK:
                 self.tmp_file = os.path.join(self.tmp_file_path, self.file_name)
                 self.edit_file(temp_file, filelines, remove_lines)
             else:
-                raise Exception("Framework argument missing in file")
+                raise Exception("\nFramework argument missing in file")
         except Exception as e:
             raise e
 
     def get_variables(self, temp_file):
         main_file = False
         remove_lines = []
         with open(temp_file, "r") as tmp_fp:
@@ -152,15 +151,17 @@
         with open(temp_file, "w") as tmp_fp:
             for linenum, fileline in enumerate(filelines):
                 if linenum in remove_lines:
                     continue
                 else:
                     if self.framework == TENSORFLOW_FRAMEWORK:
                         if re.search(f"def {self.method_name}\(.*\)", fileline):
-                            fileline = fileline.replace(str(self.method_name), "MyModel")
+                            fileline = fileline.replace(
+                                str(self.method_name), "MyModel"
+                            )
                         fileline = self.replace_vars(fileline)
                     elif self.framework == PYTORCH_FRAMEWORK:
                         if re.search(f"class {self.class_name}\(.*\)", fileline):
                             fileline = fileline.replace(str(self.class_name), "MyModel")
                     edited_data.append(fileline)
             tmp_fp.writelines("\n".join(edited_data))
         tmp_fp.close()
@@ -250,15 +251,17 @@
         try:
             getmembers(self.model.MyModel, isfunction)
             self.progress_bar.update(1)
         except Exception:  # pragma: no cover
             self.message = "Please upload file as per docs"
             raise
 
-    def load_model(self, filename, update_progress_bar=False):
+    def load_model(self, filename="", update_progress_bar=False):
+        if filename == "":
+            filename = self.file_name
         try:
             sys.path.append(self.tmp_file_path)
             self.model = SourceFileLoader(
                 f"{filename}", f"{self.tmp_file}"
             ).load_module()
             if self.framework == PYTORCH_FRAMEWORK:
                 self.model = self.model.MyModel()
@@ -292,25 +295,25 @@
             else:
                 self.tmp_file = os.path.join(self.tmp_file_path, str(file))
                 self.file_name = str(file)
                 shutil.copy2(self.model_path, self.tmp_file_path)
             for tmp_f in os.listdir(self.tmp_file_path):
                 if not (os.path.isdir(tmp_f) or tmp_f in self.notallowed):
                     self.prepare_file(os.path.join(self.tmp_file_path, tmp_f))
-            self.load_model(self.file_name, update_progress_bar=True)
+            self.load_model(filename=self.file_name)
             if self.framework == TENSORFLOW_FRAMEWORK:
                 self.check_MyModel()
                 self.check_model_arguments()
             else:
                 self.progress_bar.update(2)
         except Exception as e:  # pragma: no cover
             if os.path.exists(self.tmp_file_path):
                 shutil.rmtree(self.tmp_file_path)
             if self.message == "":
-                self.message = f"\nError loading the model file"
+                self.message = f"\nError loading the model file as {e}"
             raise
 
     def check_model_arguments(self):
         """
         Check if MyModel contains:
             - input_shape
             - classes
@@ -341,17 +344,18 @@
             if self.message == "":
                 self.message = f"Model checks failed with error as {e}"
             eligible = False
         if not eligible:
             return eligible, self.message, None, self.progress_bar  # pragma: no cover
         return True, self.message, self.model_name, self.progress_bar
 
+
 class TensorflowChecks:
-    def __init__(self, model, model_name, progress_bar):
-        self.message = None
+    def __init__(self, model, model_name, message, progress_bar):
+        self.message = message
         self.model = model
         self.model_name = model_name
         self.progress_bar = progress_bar
 
     def progress_bar_update(self):
         if self.progress_bar is not None:
             self.progress_bar.update(1)
@@ -435,16 +439,16 @@
         eligible, message = self.is_model_eligible()
         if not eligible:
             return eligible, message, None, self.progress_bar  # pragma: no cover
         return True, self.message, self.model_name, self.progress_bar
 
 
 class TorchChecks:
-    def __init__(self, model, model_name, progress_bar):
-        self.message = None
+    def __init__(self, model, model_name, message, progress_bar):
+        self.message = message
         self.model = model
         self.model_name = model_name
         self.progress_bar = progress_bar
 
     def is_model_supported(self):
         """
         Check if model contains:
```

### Comparing `tracebloc_package-dev-0.4.1/tracebloc_package/linkModelDataSet.py` & `tracebloc_package-dev-0.4.2/tracebloc_package/linkModelDataSet.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import base64
 from termcolor import colored
 from tracebloc_package import check_parameters
 from .utils import *
 from .functional_test import CheckModel, TensorflowChecks, TorchChecks
 
 
-
 class LinkModelDataSet:
     """
     creating a training plan and assign data set
     parameters: modelId, datasetId, token
 
     methods:get_parameters, get_trainingplan
     """
@@ -53,15 +52,15 @@
         self.__image_shape = 224
         self.__image_type = "rgb"
         self.__optimizer = "sgd"
         self.__totalDatasetSize = totalDatasetSize
         self.__trainingDatasetSize = totalDatasetSize
         self.__trainingClasses = class_names
         self.__subdataset = {}
-        self.__lossFunction = {TYPE: STANDARD, VALUE: "categorical_crossentropy"}
+        self.__lossFunction = {TYPE: STANDARD, VALUE: "mse"}
         self.__learningRate = {TYPE: CONSTANT, VALUE: 0.001}
         self.__seed = False
         self.__total_images = total_images
         self.__num_classes = num_classes
         self.__class_names = class_names
         self.__batchSize = self.__default_batchSize()
         self.__featurewise_center = False
@@ -114,15 +113,15 @@
         self.__epochs = 10
         self.__cycles = 1
         self.__image_shape = 224
         self.__image_type = "rgb"
         self.__optimizer = "sgd"
         self.__trainingDatasetSize = self.__totalDatasetSize
         self.__trainingClasses = self.__class_names
-        self.__lossFunction = {TYPE: STANDARD, VALUE: "categorical_crossentropy"}
+        self.__lossFunction = {TYPE: STANDARD, VALUE: "mse"}
         self.__learningRate = {TYPE: CONSTANT, VALUE: 0.001}
         self.__seed = False
         self.__batchSize = self.__default_batchSize()
         self.__featurewise_center = False
         self.__samplewise_center = False
         self.__featurewise_std_normalization = False
         self.__samplewise_std_normalization = False
@@ -391,15 +390,15 @@
         """
         # get edge with lowest images
         edge_min = min(self.__total_images, key=self.__total_images.get)
         # get images count for selected edge
         images = int(self.__total_images[edge_min])
         # check for no of batches
         if type(batchSize) == int:
-            if images // batchSize < 3:
+            if images // batchSize < 3 and self.__framework == TENSORFLOW_FRAMEWORK:
                 error_msg = "Please choose smaller batch size as dataset selected have less images\n"
                 self.__print_error(error_msg)
                 return
             self.__batchSize = batchSize
             self.__remove_error_method()
         else:
             error_msg = "Invalid input type given for batchSize\n"
@@ -441,15 +440,24 @@
         """
         String (name of optimizer)
         example: trainingObject.optimizer('rmsprop')
         supported optimizers: ['adam','rmsprop','sgd','adadelta', 'adagrad', 'adamax','nadam', 'ftrl']
         default: 'sgd'
         """
         if self.__framework == TENSORFLOW_FRAMEWORK:
-            o = ["adam", "rmsprop", "sgd", "adadelta", "adagrad", "adamax", "nadam", "ftrl"]
+            o = [
+                "adam",
+                "rmsprop",
+                "sgd",
+                "adadelta",
+                "adagrad",
+                "adamax",
+                "nadam",
+                "ftrl",
+            ]
             optlrrateflag = True
             error = None
             optimizer = optimizer.lower()
             try:
                 o.index(optimizer)
                 if self.__learningRateSet:
                     optlrrateflag, error = check_parameters.get_optimizer(
@@ -462,15 +470,24 @@
                     self.__optimizer = optimizer
                     self.__optimizerSet = True
                     self.__remove_error_method()
             except Exception as e:
                 error_msg = f"Please provide supported optimizers: {o}\n"
                 self.__print_error(error_msg)
         else:
-            o = ["adam", "rmsprop", "sgd", "adadelta", "adagrad", "adamax", "nadam", "ftrl"]
+            o = [
+                "adam",
+                "rmsprop",
+                "sgd",
+                "adadelta",
+                "adagrad",
+                "adamax",
+                "nadam",
+                "ftrl",
+            ]
             try:
                 o.index(optimizer)
                 self.__optimizer = optimizer
                 self.__remove_error_method()
             except:
                 error_msg = f"Please provide supported optimizers: {o}\n"
                 self.__print_error(error_msg)
@@ -511,27 +528,35 @@
                     self.__print_error(error_msg)
                 else:
                     if learningRate[TYPE] == CUSTOM and callable(learningRate[VALUE]):
                         try:
                             # Serialize the loss function
                             serialized_data = learningRate
                             # Encode the binary data as text
-                            encoded_data = base64.b64encode(serialized_data).decode("utf-8")
+                            encoded_data = base64.b64encode(serialized_data).decode(
+                                "utf-8"
+                            )
                             self.__learningRate = {TYPE: CUSTOM, VALUE: encoded_data}
                             self.__learningRateSet = True
                             self.__remove_error_method()
                         except Exception as e:
-                            error_msg = f"Error while setting custom learning rate : {e}\n"
+                            error_msg = (
+                                f"Error while setting custom learning rate : {e}\n"
+                            )
                             self.__print_error(error_msg)
-                    elif learningRate[TYPE] == CONSTANT or learningRate[TYPE] == ADAPTIVE:
+                    elif (
+                        learningRate[TYPE] == CONSTANT or learningRate[TYPE] == ADAPTIVE
+                    ):
                         self.__learningRate = learningRate
                         self.__learningRateSet = True
                         self.__remove_error_method()
                     else:
-                        error_msg = "Input not as per given convention for learningRate\n"
+                        error_msg = (
+                            "Input not as per given convention for learningRate\n"
+                        )
                         self.__print_error(error_msg)
             else:
                 error_msg = "Input not as per given convention for learningRate\n"
                 self.__print_error(error_msg)
         else:
             if learningRate[TYPE] == CONSTANT:
                 self.__learningRate = learningRate
@@ -579,20 +604,28 @@
                         self.__print_error(error_msg)
                 elif lossFunction[TYPE] == CUSTOM:
                     if callable(lossFunction[VALUE]):
                         try:
                             # Serialize the loss function
                             serialized_data = dill.dumps(lossFunction[VALUE])
                             # Encode the binary data as text
-                            encoded_data = base64.b64encode(serialized_data).decode("utf-8")
+                            encoded_data = base64.b64encode(serialized_data).decode(
+                                "utf-8"
+                            )
 
                             try:
                                 # TODO: change the check model class according to framework used
-                                model_checks = TensorflowChecks(model=self.__model, model_name=self.__modelName, progress_bar=None)
-                                model_checks.small_training_loop(custom_loss=lossFunction)
+                                model_checks = TensorflowChecks(
+                                    model=self.__model,
+                                    model_name=self.__modelName,
+                                    progress_bar=None,
+                                )
+                                model_checks.small_training_loop(
+                                    custom_loss=lossFunction
+                                )
 
                                 lossFunction[VALUE] = encoded_data
                                 self.__lossFunction = lossFunction
                                 self.__remove_error_method()
                             except Exception as e:
                                 error_msg = f"custom loss provided give error as {e}\n"
                                 self.__print_error(error_msg)
@@ -606,16 +639,20 @@
                 else:
                     error_msg = "Invalid input function given for loss function\n"
                     self.__print_error(error_msg)
             else:
                 error_msg = "type missing in lossfunction"
                 self.__print_error(error_msg)
         else:
-            l = ["binary_crossentropy", "categorical_crossentropy", "mse"]
-            if TYPE in lossFunction.keys() and VALUE in lossFunction.keys() and lossFunction[TYPE] == STANDARD:
+            l = ["crossentropy", "binarycrossentropy", "mse", "l1", "nll"]
+            if (
+                TYPE in lossFunction.keys()
+                and VALUE in lossFunction.keys()
+                and lossFunction[TYPE] == STANDARD
+            ):
                 try:
                     l.index(lossFunction[VALUE].lower())
                     self.__lossFunction = lossFunction
                     self.__remove_error_method()
                 except:
                     error_msg = f"Please provide tensorflow supported default loss functions losses: {l}\n"
                     self.__print_error(error_msg)
@@ -682,15 +719,17 @@
             try:
                 f.index(monitor.lower())
                 if type(save_best_only) == bool:
                     c = [monitor, save_best_only]
                     self.__modelCheckpointCallback["modelCheckpoint"] = c
                     self.__remove_error_method()
                 else:
-                    error_msg = "Invalid datatype for arguments given for save_best_only\n"
+                    error_msg = (
+                        "Invalid datatype for arguments given for save_best_only\n"
+                    )
                     self.__print_error(error_msg)
             except:
                 error_msg = f"Please provide supported monitor values: {f}\n"
                 self.__print_error(error_msg)
         else:
             self.__not_supported_parameters("modelCheckpointCallback")
 
@@ -794,15 +833,17 @@
         default: False
         """
         if self.__framework == TENSORFLOW_FRAMEWORK:
             if type(samplewise_std_normalization) == bool:
                 self.__samplewise_std_normalization = samplewise_std_normalization
                 self.__remove_error_method()
             else:
-                error_msg = "Invalid input type given for samplewise_std_normalization\n"
+                error_msg = (
+                    "Invalid input type given for samplewise_std_normalization\n"
+                )
                 self.__print_error(error_msg)
         else:
             self.__not_supported_parameters("samplewise_std_normalization")
 
     def rotation_range(self, rotation_range: int):
         """
         Int. Degree range for random rotations.
```

### Comparing `tracebloc_package-dev-0.4.1/tracebloc_package/messages.py` & `tracebloc_package-dev-0.4.2/tracebloc_package/messages.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.1/tracebloc_package/upload.py` & `tracebloc_package-dev-0.4.2/tracebloc_package/upload.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import pickletools
 import sys
 import torch
 import requests, json, pickle
 from importlib.machinery import SourceFileLoader
 from termcolor import colored
 import os
 import rich
@@ -51,24 +52,30 @@
         root, ext = os.path.splitext(path)
         if ext:
             if ext != self.__ext:
                 self.__ext = ".zip"
             # assign the provided path to model's path
             self.__model_path = path
             # get weights path --> remove .py from the given path and add _weights.pkl after it
-            self.__weights_path = path.rsplit(".", 1)[0] + "_weights.pkl"
+            if os.path.exists(path.rsplit(".", 1)[0] + "_weights.pkl"):
+                self.__weights_path = path.rsplit(".", 1)[0] + "_weights.pkl"
+            else:
+                self.__weights_path = path.rsplit(".", 1)[0] + "_weights.pth"
             # get model name --> get model name from given path
             self.__modelname = path.rsplit(".", 1)[0].split("/")[-1]
         else:
             # get models path --> add .py at the end of given path
             if os.path.exists(path + ".zip"):
                 self.__ext = ".zip"
             self.__model_path = path + self.__ext
             # get weights path --> add _weights.pkl after given path
-            self.__weights_path = path + "_weights.pkl"
+            if os.path.exists(path + "_weights.pkl"):
+                self.__weights_path = path + "_weights.pkl"
+            else:
+                self.__weights_path = path + "_weights.pth"
             # get model name --> get filename from given path
             self.__modelname = path.split("/")[-1]
 
     def getNewModelId(self):
         if self.__recievedModelname is not None:
             return (
                 self.__recievedModelname,
@@ -112,14 +119,15 @@
             if self.__framework == PYTORCH_FRAMEWORK:
                 model_check_class = TorchChecks
             elif self.__framework == TENSORFLOW_FRAMEWORK:
                 model_check_class = TensorflowChecks
             model_checks = model_check_class(
                 model=loaded_model,
                 model_name=model_name,
+                message=message,
                 progress_bar=self.progress_bar,
             )
             (
                 status,
                 message,
                 model_name,
                 progress_bar,
@@ -130,16 +138,20 @@
                     message,
                     "red",
                 )
                 print(text, "\n")
                 self.progress_bar.close()
                 return None
             self.progress_bar.update(1)
+            model_checks_generic.load_model(update_progress_bar=True)
+            if self.__framework == TENSORFLOW_FRAMEWORK:
+                self.model = model_checks_generic.model.MyModel()
+            else:
+                self.model = model_checks_generic.model
             model_checks_generic.remove_tmp_file(update_progress_bar=True)
-            self.model = model_checks.model
             updated_model_name = self.__upload_model()
             self.progress_bar.close()
             return updated_model_name
         except FileNotFoundError:
             text = colored(
                 f"\nUpload failed. There is no model with the name '{self.__modelname}' in your folder '{os.getcwd()}'.",
                 "red",
@@ -162,19 +174,18 @@
                 )
             self.progress_bar.close()
             return None
 
     def __upload_model(self):
         model_file = open(self.__model_path, "rb")
         if self.weights:
-            w = self.checkWeights()
-            if not w:
+            weights_valid, weights = self.checkWeights()
+            if not weights_valid:
                 return None
-            weights_file = open(self.__weights_path, "rb")
-            files = {"upload_file": model_file, "upload_weights": weights_file}
+            files = {"upload_file": model_file, "upload_weights": weights}
             values = {
                 "model_name": self.__modelname,
                 "setWeights": True,
                 "type": "functional_test",
             }
         else:
             files = {"upload_file": model_file}
@@ -197,14 +208,15 @@
             tex = colored(
                 text,
                 "red",
             )
             print(tex, "\n")
             return None
         self.progress_bar.update(1)
+        weights.close()
         return content["model_name"]
 
     def checkWeights(self):
         # load model weights from current directory
         try:
             weights_file = open(self.__weights_path, "rb")
         except FileNotFoundError:
@@ -215,26 +227,41 @@
             print(text, "\n")
             rich.print(
                 "For more information check the [link=https://docs.tracebloc.io/user-uploadModel]docs[/link]"
             )
             return False
         # Load weights to check if it works
         try:
-            we = pickle.load(weights_file)
-            model = SourceFileLoader(
-                self.__modelname, f"{self.__model_path}"
-            ).load_module()
-            model = model.MyModel()
-            model.set_weights(we)
-            weights_file.close()
-            return True
+            if self.__framework == TENSORFLOW_FRAMEWORK:
+                we = pickle.load(weights_file)
+                self.model.set_weights(we)
+                return True, weights_file
+            elif self.__framework == PYTORCH_FRAMEWORK:
+                try:
+                    self.model.load_state_dict(torch.load(self.__weights_path))
+                    return True, weights_file
+                except:
+                    return False, []
+            else:
+                raise Exception("\nFramework not valid")
         except ValueError:
             weights_file.close()
             text = colored(
                 "Weights upload failed. Provide weights compatible with provided model.",
                 "red",
             )
             print(text, "\n")
             print(
                 "For more information check the docs 'https://docs.tracebloc.io/weights'"
             )
-            return False
+            return False, []
+        except Exception as e:
+            weights_file.close()
+            text = colored(
+                f"Weights upload failed with error {e}",
+                "red",
+            )
+            print(text, "\n")
+            print(
+                "For more information check the docs 'https://docs.tracebloc.io/weights'"
+            )
+            return False, []
```

### Comparing `tracebloc_package-dev-0.4.1/tracebloc_package/user.py` & `tracebloc_package-dev-0.4.2/tracebloc_package/user.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.1/tracebloc_package/utils.py` & `tracebloc_package-dev-0.4.2/tracebloc_package/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 STANDARD = "standard"
 ADAPTIVE = "adaptive"
 CUSTOM = "custom"
 TYPE = "type"
 FUNCTION = "function"
 VALUE = "value"
 
+
 def check_MyModel(filename, path):
     try:
         # check if file contains the MyModel function
         model = SourceFileLoader(filename, f"{path}").load_module()
         model.MyModel(input_shape=(500, 500, 3), classes=10)
         return True, model
```

### Comparing `tracebloc_package-dev-0.4.1/tracebloc_package/weights.py` & `tracebloc_package-dev-0.4.2/tracebloc_package/weights.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.1/tracebloc_package_dev.egg-info/PKG-INFO` & `tracebloc_package-dev-0.4.2/tracebloc_package_dev.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: tracebloc-package-dev
-Version: 0.4.1
+Version: 0.4.2
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
+Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Tracebloc package
 This packeg is pre-requiste to run tracebloc jupyter notebook.
 
 
 This package helps to create and start the experiment for training ML models in 
 tracebloc environment.
+
```

### Comparing `tracebloc_package-dev-0.4.1/tracebloc_package_dev.egg-info/SOURCES.txt` & `tracebloc_package-dev-0.4.2/tracebloc_package_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

