# Comparing `tmp/drillvision-0.0.2.tar.gz` & `tmp/drillvision-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/drillvision-0.0.2.tar", last modified: Mon May 29 04:04:59 2023, max compression
+gzip compressed data, was "dist/drillvision-0.0.3.tar", last modified: Thu Jun  1 21:28:04 2023, max compression
```

## Comparing `drillvision-0.0.2.tar` & `drillvision-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 amin       (501) staff       (20)        0 2023-05-29 04:04:59.273536 drillvision-0.0.2/
--rw-r--r--   0 amin       (501) staff       (20)      305 2023-05-21 20:38:44.000000 drillvision-0.0.2/MANIFEST.in
--rw-r--r--   0 amin       (501) staff       (20)     6322 2023-05-29 04:04:59.272381 drillvision-0.0.2/PKG-INFO
--rw-r--r--   0 amin       (501) staff       (20)     5699 2023-05-22 03:34:53.000000 drillvision-0.0.2/README.md
-drwxr-xr-x   0 amin       (501) staff       (20)        0 2023-05-29 04:04:59.269879 drillvision-0.0.2/drillvision.egg-info/
--rw-r--r--   0 amin       (501) staff       (20)     6322 2023-05-29 04:04:59.000000 drillvision-0.0.2/drillvision.egg-info/PKG-INFO
--rw-r--r--   0 amin       (501) staff       (20)      747 2023-05-29 04:04:59.000000 drillvision-0.0.2/drillvision.egg-info/SOURCES.txt
--rw-r--r--   0 amin       (501) staff       (20)        1 2023-05-29 04:04:59.000000 drillvision-0.0.2/drillvision.egg-info/dependency_links.txt
--rw-r--r--   0 amin       (501) staff       (20)      227 2023-05-29 04:04:59.000000 drillvision-0.0.2/drillvision.egg-info/requires.txt
--rw-r--r--   0 amin       (501) staff       (20)       21 2023-05-29 04:04:59.000000 drillvision-0.0.2/drillvision.egg-info/top_level.txt
-drwxr-xr-x   0 amin       (501) staff       (20)        0 2023-05-29 04:04:59.267434 drillvision-0.0.2/neural_network_model/
--rw-r--r--   0 amin       (501) staff       (20)        5 2023-05-29 04:04:29.000000 drillvision-0.0.2/neural_network_model/VERSION
--rw-r--r--   0 amin       (501) staff       (20)        0 2023-05-16 02:02:49.000000 drillvision-0.0.2/neural_network_model/__init__.py
--rw-r--r--   0 amin       (501) staff       (20)    21716 2023-05-29 03:59:31.000000 drillvision-0.0.2/neural_network_model/bit_vision.py
--rw-r--r--   0 amin       (501) staff       (20)     5962 2023-05-29 03:59:31.000000 drillvision-0.0.2/neural_network_model/model.py
--rw-r--r--   0 amin       (501) staff       (20)    14713 2023-05-25 23:15:08.000000 drillvision-0.0.2/neural_network_model/process_data.py
--rw-r--r--   0 amin       (501) staff       (20)     2843 2023-05-20 18:27:45.000000 drillvision-0.0.2/neural_network_model/s3.py
--rw-r--r--   0 amin       (501) staff       (20)     1913 2023-05-21 20:09:15.000000 drillvision-0.0.2/pyproject.toml
--rw-r--r--   0 amin       (501) staff       (20)       97 2023-05-13 20:20:47.000000 drillvision-0.0.2/requirements-test.txt
--rw-r--r--   0 amin       (501) staff       (20)      228 2023-05-24 01:47:09.000000 drillvision-0.0.2/requirements.txt
--rw-r--r--   0 amin       (501) staff       (20)       38 2023-05-29 04:04:59.273931 drillvision-0.0.2/setup.cfg
--rw-r--r--   0 amin       (501) staff       (20)     2128 2023-05-29 03:58:58.000000 drillvision-0.0.2/setup.py
-drwxr-xr-x   0 amin       (501) staff       (20)        0 2023-05-29 04:04:59.271494 drillvision-0.0.2/tests/
--rw-r--r--   0 amin       (501) staff       (20)      346 2023-05-20 18:27:45.000000 drillvision-0.0.2/tests/test_bitvision.py
--rw-r--r--   0 amin       (501) staff       (20)     3023 2023-05-20 18:27:45.000000 drillvision-0.0.2/tests/test_preprocessing.py
+drwxr-xr-x   0 amin       (501) staff       (20)        0 2023-06-01 21:28:04.109699 drillvision-0.0.3/
+-rw-r--r--   0 amin       (501) staff       (20)      305 2023-05-21 20:38:44.000000 drillvision-0.0.3/MANIFEST.in
+-rw-r--r--   0 amin       (501) staff       (20)     8260 2023-06-01 21:28:04.109397 drillvision-0.0.3/PKG-INFO
+-rw-r--r--   0 amin       (501) staff       (20)     7638 2023-06-01 21:22:00.000000 drillvision-0.0.3/README.md
+drwxr-xr-x   0 amin       (501) staff       (20)        0 2023-06-01 21:28:04.107316 drillvision-0.0.3/drillvision.egg-info/
+-rw-r--r--   0 amin       (501) staff       (20)     8260 2023-06-01 21:28:03.000000 drillvision-0.0.3/drillvision.egg-info/PKG-INFO
+-rw-r--r--   0 amin       (501) staff       (20)      747 2023-06-01 21:28:03.000000 drillvision-0.0.3/drillvision.egg-info/SOURCES.txt
+-rw-r--r--   0 amin       (501) staff       (20)        1 2023-06-01 21:28:03.000000 drillvision-0.0.3/drillvision.egg-info/dependency_links.txt
+-rw-r--r--   0 amin       (501) staff       (20)      248 2023-06-01 21:28:03.000000 drillvision-0.0.3/drillvision.egg-info/requires.txt
+-rw-r--r--   0 amin       (501) staff       (20)       21 2023-06-01 21:28:03.000000 drillvision-0.0.3/drillvision.egg-info/top_level.txt
+drwxr-xr-x   0 amin       (501) staff       (20)        0 2023-06-01 21:28:04.105081 drillvision-0.0.3/neural_network_model/
+-rw-r--r--   0 amin       (501) staff       (20)        5 2023-06-01 21:24:02.000000 drillvision-0.0.3/neural_network_model/VERSION
+-rw-r--r--   0 amin       (501) staff       (20)        0 2023-05-16 02:02:49.000000 drillvision-0.0.3/neural_network_model/__init__.py
+-rw-r--r--   0 amin       (501) staff       (20)    22291 2023-06-01 20:54:29.000000 drillvision-0.0.3/neural_network_model/bit_vision.py
+-rw-r--r--   0 amin       (501) staff       (20)     5962 2023-05-29 03:59:31.000000 drillvision-0.0.3/neural_network_model/model.py
+-rw-r--r--   0 amin       (501) staff       (20)    14713 2023-05-25 23:15:08.000000 drillvision-0.0.3/neural_network_model/process_data.py
+-rw-r--r--   0 amin       (501) staff       (20)     2843 2023-05-20 18:27:45.000000 drillvision-0.0.3/neural_network_model/s3.py
+-rw-r--r--   0 amin       (501) staff       (20)     1913 2023-05-21 20:09:15.000000 drillvision-0.0.3/pyproject.toml
+-rw-r--r--   0 amin       (501) staff       (20)       97 2023-05-13 20:20:47.000000 drillvision-0.0.3/requirements-test.txt
+-rw-r--r--   0 amin       (501) staff       (20)      248 2023-05-31 01:33:26.000000 drillvision-0.0.3/requirements.txt
+-rw-r--r--   0 amin       (501) staff       (20)       38 2023-06-01 21:28:04.109812 drillvision-0.0.3/setup.cfg
+-rw-r--r--   0 amin       (501) staff       (20)     2128 2023-05-29 03:58:58.000000 drillvision-0.0.3/setup.py
+drwxr-xr-x   0 amin       (501) staff       (20)        0 2023-06-01 21:28:04.108722 drillvision-0.0.3/tests/
+-rw-r--r--   0 amin       (501) staff       (20)      346 2023-05-20 18:27:45.000000 drillvision-0.0.3/tests/test_bitvision.py
+-rw-r--r--   0 amin       (501) staff       (20)     3023 2023-05-20 18:27:45.000000 drillvision-0.0.3/tests/test_preprocessing.py
```

### Comparing `drillvision-0.0.2/PKG-INFO` & `drillvision-0.0.3/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: drillvision
-Version: 0.0.2
-Summary: # Drill Bit Classifier
-Home-page: https://github.com/Atashnezhad/DrillBitVision
-Author: Amin Atashnezhad
-Author-email: atashnezhad2@gmail.com
-License: BSD-3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
-
 # Drill Bit Classifier
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-360/)
 [![PyPI version](https://badge.fury.io/py/drillvision.svg)](https://badge.fury.io/py/drillvision)
 
 The Drill Bit Classifier is an app that uses a Convolutional Neural Network (CNN) to 
 classify images of drill bits. The app can be used by machinists and engineers to 
 quickly and accurately identify the type of drill bit required for a particular job.
@@ -85,7 +68,58 @@
 
 
 ## Grad Cam Heatmap - Rollercone Bit
 ![alt text](figures/grad_cam_rc_1.png "Logo Title Text 1")
 
 ## Grad Cam Heatmap - PDC Bit
 ![alt text](figures/grad_cam_pdc_1.png "Logo Title Text 1")
+
+
+# How to use the Drill Bit Classifier Example
+## Installation
+```bash
+pip install drillvision
+```
+## Usage
+```python
+from pathlib import Path
+from neural_network_model.process_data import Preprocessing
+from neural_network_model.bit_vision import BitVision
+
+if __name__ == "__main__":
+    # download the images
+    obj = Preprocessing(dataset_address=Path(__file__).parent / "dataset")
+    obj.download_images()
+    print(obj.image_dict)
+    obj.augment_data(
+        number_of_images_tobe_gen=10,
+        augment_data_address=Path(__file__).parent / "augmented_dataset"
+    )
+    obj.train_test_split(
+        augmented_data_address=Path(__file__).parent / "augmented_dataset",
+        train_test_val_split_dir_address=Path(__file__).parent / "dataset_train_test_val"
+    )
+
+    obj = BitVision(train_test_val_dir=Path(__file__).parent / "dataset_train_test_val")
+    print(obj.categories)
+    print(obj.data_details)
+    obj.plot_image_category()
+    obj.compile_model()
+    model_name = "model_test_1.h5"
+    obj.train_model(model_save_address=Path(__file__).parent / "deep_model" / model_name)
+    obj.plot_history(fig_folder_address=Path(__file__).parent / "figures")
+
+    obj.predict(
+        fig_save_address=Path(__file__).parent / "figures",
+        model_path=Path(__file__).parent / "deep_model" / model_name,
+        test_folder_address=Path(__file__).parent / "dataset_train_test_val" / "test"
+    )
+
+    # find list of images in the Path(__file__).parent / "dataset_train_test_val" / "test" / "pdc_bit"
+    directory_path = Path(__file__).parent / "dataset_train_test_val" / "test" / "pdc_bit"
+    list_of_images = [str(x) for x in directory_path.glob("*.jpeg")]
+    obj.grad_cam_viz(
+        fig_to_save_address=Path(__file__).parent / "figures",
+        img_to_be_applied_path=Path(__file__).parent / "dataset_train_test_val" / "test" / "pdc_bit" / list_of_images[0],
+        output_gradcam_fig_name="gradcam.png"
+    )
+
```

### Comparing `drillvision-0.0.2/drillvision.egg-info/SOURCES.txt` & `drillvision-0.0.3/drillvision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drillvision-0.0.2/neural_network_model/bit_vision.py` & `drillvision-0.0.3/neural_network_model/bit_vision.py`

 * *Files 4% similar despite different names*

```diff
@@ -262,14 +262,17 @@
         This function is used to plot the history of the model.
         :param fig_folder_address: the address of the folder to save the figure
         :return:
         """
         fig_folder_address = kwargs.get(
             "fig_folder_address", SETTING.FIGURE_SETTING.FIG_PRED_OUT_DIR_ADDRESS
         )
+        # if the folder does not exist, create it
+        if not os.path.exists(fig_folder_address):
+            os.makedirs(fig_folder_address)
         logger.info(self.model_history.history.keys())
         keys_plot = ["loss", "accuracy"]
         # make two plots side by side and have train and val for loss and accuracy
         fig, axs = plt.subplots(
             SETTING.FIGURE_SETTING.NUM_ROWS_IN_PLOT_HIST,
             SETTING.FIGURE_SETTING.NUM_COLS_IN_PLOT_HIST,
             figsize=SETTING.FIGURE_SETTING.FIGURE_SIZE_IN_PLOT_HIST,
@@ -295,25 +298,32 @@
                 list_to_be_edited.remove(case)
         return list_to_be_edited
 
     def predict(self, *args, **kwargs):
         """
         This function is used to predict the test data.
         :param args:
-        :param kwargs: fid_save_address: the address of the folder to save the figure,
+        :param kwargs: fig_save_address: the address of the folder to save the figure,
         model_path: the path of the model to be used for prediction
         :return:
         """
-        fid_save_address = kwargs.get(
-            "fid_save_address", SETTING.FIGURE_SETTING.FIG_PRED_OUT_DIR_ADDRESS
+        fig_save_address = kwargs.get(
+            "fig_save_address", SETTING.FIGURE_SETTING.FIG_PRED_OUT_DIR_ADDRESS
         )
+        # if the folder does not exist, create it
+        if not os.path.exists(fig_save_address):
+            os.makedirs(fig_save_address)
         model_path = kwargs.get("model_path", SETTING.MODEL_SETTING.MODEL_PATH)
         if model_path is None:
             raise ValueError("model_path is None")
 
+        test_folder_address = kwargs.get("test_folder_address", SETTING.DATA_ADDRESS_SETTING.TEST_DIR_ADDRESS)
+        if test_folder_address is None:
+            raise ValueError("test_folder_address is None")
+
         model = keras.models.load_model(model_path)
         logger.info(f"Model loaded from {model_path}")
 
         for category in self.categories:
             plt.figure(figsize=SETTING.FIGURE_SETTING.FIGURE_SIZE_IN_PRED_MODEL)
             number_of_cols = SETTING.FIGURE_SETTING.NUM_COLS_IN_PRED_MODEL
             number_of_rows = SETTING.FIGURE_SETTING.NUM_ROWS_IN_PRED_MODEL
@@ -365,24 +375,24 @@
                     ax.set_title(
                         f"{self.model_class_indices.get(prediction[0])}",
                         color="red",
                     )
 
             # save the figure in the figures folder
             fig_name = f"prediction_{category}.png"
-            fig_path = (fid_save_address / fig_name).resolve()
+            fig_path = (fig_save_address / fig_name).resolve()
             if not os.path.exists(fig_path.parent):
                 os.makedirs(fig_path.parent)
             plt.savefig(fig_path)
             plt.show()
             plt.tight_layout()
 
         datagen = image.ImageDataGenerator(SETTING.DATA_GEN_SETTING.RESCALE)
         DoubleCheck_generator = datagen.flow_from_directory(
-            directory=SETTING.DATA_ADDRESS_SETTING.TEST_DIR_ADDRESS,
+            directory=test_folder_address,
             target_size=SETTING.FLOW_FROM_DIRECTORY_SETTING.TARGET_SIZE,
             color_mode=SETTING.FLOW_FROM_DIRECTORY_SETTING.COLOR_MODE,
             classes=None,
             class_mode=SETTING.FLOW_FROM_DIRECTORY_SETTING.CLASS_MODE,
             batch_size=SETTING.FLOW_FROM_DIRECTORY_SETTING.BATCH_SIZE,
             shuffle=SETTING.FLOW_FROM_DIRECTORY_SETTING.SHUFFLE,
             seed=SETTING.FLOW_FROM_DIRECTORY_SETTING.SEED,
@@ -399,16 +409,19 @@
     # TODO: check the addresses and add as kwargs if needed
     def grad_cam_viz(self, *args, **kwargs):
         model_path = kwargs.get("model_path", SETTING.MODEL_SETTING.MODEL_PATH)
         fig_to_save_address = kwargs.get(
             "fig_to_save_address", SETTING.GRAD_CAM_SETTING.IMAGE_NEW_NAME
         )
         gradcam_fig_name = kwargs.get(
-            "gradcam_fig_name", SETTING.GRAD_CAM_SETTING.GRAD_CAM_FIG_NAME
+            "output_gradcam_fig_name", SETTING.GRAD_CAM_SETTING.GRAD_CAM_FIG_NAME
         )
+
+        img_to_be_applied_path = kwargs.get("img_to_be_applied_path", SETTING.GRAD_CAM_SETTING.IMG_PATH)
+
         fig_address = fig_to_save_address / gradcam_fig_name
         if model_path is None:
             raise ValueError("model_path is None")
 
         model = keras.models.load_model(model_path)
         logger.info(f"Model loaded from {model_path}")
 
@@ -419,15 +432,15 @@
         # model_builder = keras.applications.xception.Xception
         preprocess_input = keras.applications.xception.preprocess_input
         # decode_predictions = keras.applications.xception.decode_predictions
 
         last_conv_layer_name = SETTING.GRAD_CAM_SETTING.LAST_CONV_LAYER_NAME
 
         # The local path to our target image
-        img_path = SETTING.GRAD_CAM_SETTING.IMG_PATH
+        img_path = img_to_be_applied_path
 
         # load the image and show it
         img = load_img(
             img_path, target_size=SETTING.FLOW_FROM_DIRECTORY_SETTING.TARGET_SIZE
         )
         plt.imshow(img)
         plt.show()
```

### Comparing `drillvision-0.0.2/neural_network_model/model.py` & `drillvision-0.0.3/neural_network_model/model.py`

 * *Files identical despite different names*

### Comparing `drillvision-0.0.2/neural_network_model/process_data.py` & `drillvision-0.0.3/neural_network_model/process_data.py`

 * *Files identical despite different names*

### Comparing `drillvision-0.0.2/neural_network_model/s3.py` & `drillvision-0.0.3/neural_network_model/s3.py`

 * *Files identical despite different names*

### Comparing `drillvision-0.0.2/pyproject.toml` & `drillvision-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `drillvision-0.0.2/setup.py` & `drillvision-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `drillvision-0.0.2/tests/test_preprocessing.py` & `drillvision-0.0.3/tests/test_preprocessing.py`

 * *Files identical despite different names*

