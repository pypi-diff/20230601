# Comparing `tmp/netspresso-0.1.0-py3-none-any.whl.zip` & `tmp/netspresso-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 12426 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat       23 b- defN 23-May-29 14:28 netspresso/__init__.py
--rw-rw-rw-  2.0 fat    19555 b- defN 23-May-30 11:05 netspresso/compressor/__init__.py
+Zip file size: 12468 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat       23 b- defN 23-May-31 23:41 netspresso/__init__.py
+-rw-rw-rw-  2.0 fat    19885 b- defN 23-May-31 17:23 netspresso/compressor/__init__.py
 -rw-rw-rw-  2.0 fat     8267 b- defN 23-May-29 15:40 netspresso/compressor/client/__init__.py
 -rw-rw-rw-  2.0 fat      536 b- defN 23-May-26 15:28 netspresso/compressor/client/config.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-23 01:23 netspresso/compressor/core/__init__.py
 -rw-rw-rw-  2.0 fat      563 b- defN 23-May-26 16:47 netspresso/compressor/core/compression.py
 -rw-rw-rw-  2.0 fat      521 b- defN 23-May-29 14:17 netspresso/compressor/core/model.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-May-30 11:08 netspresso-0.1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3790 b- defN 23-May-30 11:08 netspresso-0.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 11:08 netspresso-0.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-May-30 11:08 netspresso-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1041 b- defN 23-May-30 11:08 netspresso-0.1.0.dist-info/RECORD
-12 files, 45957 bytes uncompressed, 10650 bytes compressed:  76.8%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-May-31 23:42 netspresso-0.1.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3790 b- defN 23-May-31 23:42 netspresso-0.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-31 23:42 netspresso-0.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-May-31 23:42 netspresso-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1041 b- defN 23-May-31 23:42 netspresso-0.1.1.dist-info/RECORD
+12 files, 46287 bytes uncompressed, 10692 bytes compressed:  76.9%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: netspresso/compressor/core/compression.py
 Comment: 
 
 Filename: netspresso/compressor/core/model.py
 Comment: 
 
-Filename: netspresso-0.1.0.dist-info/LICENSE
+Filename: netspresso-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: netspresso-0.1.0.dist-info/METADATA
+Filename: netspresso-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: netspresso-0.1.0.dist-info/WHEEL
+Filename: netspresso-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: netspresso-0.1.0.dist-info/top_level.txt
+Filename: netspresso-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: netspresso-0.1.0.dist-info/RECORD
+Filename: netspresso-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## netspresso/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

## netspresso/compressor/__init__.py

```diff
@@ -7,15 +7,15 @@
 from netspresso.compressor.client import (
     ModelCompressorAPIClient,
     Task,
     Framework,
     CompressionMethod,
     RecommendationMethod,
 )
-from netspresso.compressor.client.schemas.auth import CreditResponse, LoginRequest, RefreshTokenRequest
+from netspresso.compressor.client.schemas.auth import LoginRequest, RefreshTokenRequest
 from netspresso.compressor.client.schemas.model import UploadModelRequest
 from netspresso.compressor.client.schemas.compression import (
     AutoCompressionRequest,
     CompressionRequest,
     GetAvailableLayersRequest,
     CreateCompressionRequest,
     RecommendationRequest,
@@ -23,14 +23,20 @@
 from netspresso.compressor.core.model import CompressedModel, Model
 from netspresso.compressor.core.compression import CompressionBase, CompressionInfo
 from netspresso.compressor.utils.token import check_jwt_exp
 
 
 class ModelCompressor:
     def __init__(self, email: str, password: str):
+        """Initialize the Model Compressor.
+
+        Args:
+            email (str): The email address for the user's account.
+            password (str): The password for the user's account.
+        """
         self.email = email
         self.password = password
         self.client = ModelCompressorAPIClient()
         self.__login()
 
     def __login(self) -> None:
         try:
@@ -60,80 +66,80 @@
             self.access_token = response.access_token
             self.refresh_token = response.refresh_token
 
         except Exception as e:
             raise e
 
     @validate_token
-    def get_credit(self) -> CreditResponse:
-        """Retrieve credit information.
+    def get_credit(self) -> int:
+        """Get the available NetsPresso credits.
 
         Raises:
-            e: An exception that occurred while retrieving credit information.
+            e: If an error occurs while getting credit information.
 
         Returns:
-            CreditResponse: Credit information response.
+            int: The total amount of available NetsPresso credits.
         """
         try:
             credit = self.client.get_credit(access_token=self.access_token)
             logger.info(f"Get Credit successful. Credit: {credit.total}")
 
-            return credit
+            return credit.total
 
         except Exception as e:
             logger.error(f"Get Credit failed. Error: {e}")
             raise e
 
     @validate_token
     def upload_model(
-        self, model_name: str, task: Task, framework: Framework, file_path: str, input_layers: List = []
+        self, model_name: str, task: Task, framework: Framework, file_path: str, input_shape: List = []
     ) -> Model:
-        """Upload a model.
+        """Upload a model for compression.
 
         Args:
-            model_name (str): Name of the model.
-            task (Task): Task type of the model.
-            framework (Framework): Framework used for the model.
-            file_path (str): File path of the model.
-            input_layers (List, optional): List of input layers for the model. Defaults to [].
+            model_name (str): The name of the model.
+            task (Task): The task of the model.
+            framework (Framework): The framework of the model.
+            file_path (str): The file path where the model is located.
+            input_shape (List[str], optional): Input shape of the model. Defaults to [].
 
         Raises:
             e: If an error occurs while uploading the model.
 
         Returns:
             Model: Uploaded model object.
         """
         try:
             logger.info("Uploading Model...")
             data = UploadModelRequest(
                 model_name=model_name,
                 task=task.value,
                 framework=framework.value,
                 file_path=file_path,
-                input_layers=input_layers,
+                input_layers=input_shape,
             )
             model_info = self.client.upload_model(data=data, access_token=self.access_token)
             model = Model(model_info)
             logger.info(f"Upload model successful. Model ID: {model.model_id}")
 
             return model
 
         except Exception as e:
             logger.error(f"Upload model failed. Error: {e}")
             raise e
 
     @validate_token
     def get_models(self) -> List[Dict[str, Any]]:
-        """Retrieve the list of models.
+        """Get the list of uploaded & compressed models.
 
         Raises:
-            e: An exception occurred while retrieving the model list.
+            e: If an error occurs while getting the model list.
 
         Returns:
-            List[Dict[str, Any]]: The list of models.
+            List[Dict[str, Any]]: The list of uploaded & compressed models.
         """
         try:
             logger.info("Getting model list...")
             models = []
             parent_models = self.client.get_parent_models(is_simple=True, access_token=self.access_token)
             uploaded_models = [
                 vars(Model(parent_model)) for parent_model in parent_models if parent_model.origin_from == "custom"
@@ -152,18 +158,18 @@
 
         except Exception as e:
             logger.error(f"Get model list failed. Error: {e}")
             raise e
 
     @validate_token
     def get_uploaded_models(self) -> List[Dict[str, Any]]:
-        """Retrieve the list of uploaded models.
+        """Get the list of uploaded models.
 
         Raises:
-            e: An exception occurred while retrieving the uploaded model list.
+            e: If an error occurs while getting the uploaded model list.
 
         Returns:
             List[Dict[str, Any]]: The list of uploaded models.
         """
         try:
             logger.info("Getting uploaded model list...")
             parent_models = self.client.get_parent_models(is_simple=True, access_token=self.access_token)
@@ -176,24 +182,24 @@
 
         except Exception as e:
             logger.error(f"Get uploaded model list failed. Error: {e}")
             raise e
 
     @validate_token
     def get_compressed_models(self, model_id: str) -> List[Dict[str, Any]]:
-        """Retrieve the list of compressed models for a given model.
+        """Get the list of compressed models for a given model ID.
 
         Args:
             model_id (str): The ID of the model.
 
         Raises:
-            e: An exception occurred while retrieving the compressed model list.
+            e: If an error occurs while getting the compressed model list.
 
         Returns:
-            List[Dict[str, Any]]: The list of compressed models.
+            List[Dict[str, Any]]: The list of compressed models for a given model ID.
         """
         try:
             logger.info("Getting compressed model list...")
             children_models = self.client.get_children_models(model_id=model_id, access_token=self.access_token)
             compressed_models = [vars(CompressedModel(children_model)) for children_model in children_models]
             logger.info("Get compressed model list successful.")
 
@@ -201,24 +207,25 @@
 
         except Exception as e:
             logger.error(f"Get compressed model list failed. Error: {e}")
             raise e
 
     @validate_token
     def get_model(self, model_id: str) -> Union[Model, CompressedModel]:
-        """Retrieve a specific model by its ID.
+        """Get the model for a given model ID.
 
         Args:
             model_id (str): The ID of the model.
 
         Raises:
-            e: An exception occurred while retrieving the model.
+            e: If an error occurs while getting the model.
 
         Returns:
-            Union[Model, CompressedModel]: The retrieved model.
+            Union[Model, CompressedModel]: The retrieved model. If the model is compressed,
+            `CompressedModel` will be returned. Otherwise, `Model` will be returned.
         """
         try:
             logger.info("Getting model...")
             model_info = self.client.get_model_info(model_id=model_id, access_token=self.access_token)
             if model_info.status.is_compressed:
                 model = CompressedModel(model_info)
             else:
@@ -229,43 +236,43 @@
 
         except Exception as e:
             logger.error(f"Get model failed. Error: {e}")
             raise e
 
     @validate_token
     def download_model(self, model_id: str, local_path: str) -> None:
-        """Download a specific model to the local file system.
+        """Download the model for a given model ID to the local path.
 
         Args:
             model_id (str): The ID of the model.
             local_path (str): The local path to save the downloaded model.
 
         Raises:
-            e: An exception occurred while downloading the model.
+            e: If an error occurs while downloading the model.
         """
         try:
             logger.info("Downloading model...")
             download_link = self.client.get_download_model_link(model_id=model_id, access_token=self.access_token)
             request.urlretrieve(download_link.url, local_path)
             logger.info(f"Download model successful. Local Path: {local_path}")
 
         except Exception as e:
             logger.error(f"Download model failed. Error: {e}")
             raise e
 
     @validate_token
     def delete_model(self, model_id: str, recursive: bool = False) -> None:
-        """Delete a model.
+        """Delete the model for a given model ID.
 
         Args:
-            model_id (str): The ID of the model to delete.
-            recursive (bool, optional): Whether to delete the compressed model for that model. Defaults to False.
+            model_id (str): The ID of the model.
+            recursive (bool, optional): Whether to also delete the compressed model for that model. Defaults to False.
 
         Raises:
-            e: An exception occurred while deleting the model.
+            e: If an error occurs while deleting the model.
         """
         try:
             logger.info("Deleting model...")
             children_models = self.client.get_children_models(model_id=model_id, access_token=self.access_token)
             if len(children_models) != 0:
                 if not recursive:
                     logger.warning(
@@ -286,18 +293,18 @@
 
     @validate_token
     def select_compression_method(self, model_id: str, compression_method: CompressionMethod) -> CompressionBase:
         """Select a compression method for a model.
 
         Args:
             model_id (str): The ID of the model.
-            compression_method (CompressionMethod): The compression method to use.
+            compression_method (CompressionMethod): The selected compression method.
 
         Raises:
-            e: An exception occurred while selecting the compression method.
+            e: If an error occurs while selecting the compression method.
 
         Returns:
             CompressionBase: The compression information for the selected compression method.
         """
         try:
             logger.info("Selecting compression method...")
             data = GetAvailableLayersRequest(model_id=model_id, compression_method=compression_method.value)
@@ -315,15 +322,15 @@
     def get_compression(self, compression_id: str) -> CompressionInfo:
         """Get information about a compression.
 
         Args:
             compression_id (str): The ID of the compression.
 
         Raises:
-            e: An exception occurred while getting the compression information.
+            e: If an error occurs while getting the compression information.
 
         Returns:
             CompressionInfo: The information about the compression.
         """
         try:
             logger.info("Getting compression...")
             compression_info = CompressionInfo(
@@ -338,20 +345,20 @@
             raise e
 
     @validate_token
     def compress_model(self, compression: CompressionInfo, model_name: str, output_path: str) -> CompressedModel:
         """Compress a model using the provided compression information.
 
         Args:
-            compression (CompressionInfo): Information about the compression.
-            model_name (str): Name of the compressed model.
-            output_path (str): Local path to save the compressed model.
+            compression (CompressionInfo): The information about the compression.
+            model_name (str): The name of the compressed model.
+            output_path (str): The local path to save the compressed model.
 
         Raises:
-            e: An exception occurred while compressing the model.
+            e: If an error occurs while compressing the model.
 
         Returns:
             CompressedModel: The compressed model.
         """
         try:
             logger.info("Compressing model...")
             data = CreateCompressionRequest(
@@ -389,26 +396,26 @@
         model_id: str,
         model_name: str,
         compression_method: CompressionMethod,
         recommendation_method: RecommendationMethod,
         recommendation_ratio: float,
         output_path: str,
     ) -> CompressedModel:
-        """Compress a recommendation-based model using the specified compression and recommendation methods.
+        """Compress a recommendation-based model using the given compression and recommendation methods.
 
         Args:
-            model_id (str): The ID of the model to be compressed.
+            model_id (str): The ID of the model.
             model_name (str): The name of the compressed model.
-            compression_method (CompressionMethod): The compression method to be used.
-            recommendation_method (RecommendationMethod): The recommendation method to be used.
+            compression_method (CompressionMethod): The selected compression method.
+            recommendation_method (RecommendationMethod): The selected recommendation method.
             recommendation_ratio (float): The compression ratio recommended by the recommendation method.
             output_path (str): The local path to save the compressed model.
 
         Raises:
-            e: An exception occurred while performing recommendation compression.
+            e: If an error occurs while performing recommendation compression.
 
         Returns:
             CompressedModel: The compressed model.
         """
         try:
             logger.info("Compressing recommendation-based model...")
             data = CreateCompressionRequest(
@@ -450,24 +457,24 @@
             logger.error(f"Recommendation compression failed. Error: {e}")
             raise e
 
     @validate_token
     def automatic_compression(
         self, model_id: str, model_name: str, compression_ratio: float, output_path: str
     ) -> CompressedModel:
-        """Compress a model automatically based on the specified compression ratio.
+        """Compress a model automatically based on the given compression ratio.
 
         Args:
-            model_id (str): The ID of the model to be compressed.
+            model_id (str): The ID of the model.
             model_name (str): The name of the compressed model.
-            compression_ratio (float): The target compression ratio for automatic compression.
+            compression_ratio (float): The compression ratio for automatic compression.
             output_path (str): The local path to save the compressed model.
 
         Raises:
-            e: An exception occurred while performing automatic compression.
+            e: If an error occurs while performing automatic compression.
 
         Returns:
             CompressedModel: The compressed model.
         """
         try:
             logger.info("Compressing automatic-based model...")
             data = AutoCompressionRequest(
```

## Comparing `netspresso-0.1.0.dist-info/LICENSE` & `netspresso-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `netspresso-0.1.0.dist-info/METADATA` & `netspresso-0.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netspresso
-Version: 0.1.0
+Version: 0.1.1
 Summary: python client for the NetsPresso
 Home-page: https://github.com/nota-github/netspresso-python
 Author: NetsPresso
 Author-email: bmlee@nota.ai
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

## Comparing `netspresso-0.1.0.dist-info/RECORD` & `netspresso-0.1.1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-netspresso/__init__.py,sha256=QTYqXqSTHFRkM9TEgpDFcHvwLbvqHDqvqfQ9EiXkcAM,23
-netspresso/compressor/__init__.py,sha256=rKvjTK4LR3a4_D_p7LakYyuRceoq-simptp52K25sps,19555
+netspresso/__init__.py,sha256=5xvN_gb61nKeq5TER5dSfcArTP3DVasZGN_MQq5dNpA,23
+netspresso/compressor/__init__.py,sha256=Cb4EYVhLrf2tp9nzz0U44yGcd3PzjpZEJdjeptr1AwA,19885
 netspresso/compressor/client/__init__.py,sha256=n0BXqB6A54qDrAx2lpoxOqMxdLNM2-BeKmPoaWymK4o,8267
 netspresso/compressor/client/config.py,sha256=i3EZTWDZJEq527YY1hiyiSN-DIVQyjE7zgOI7_kLY9Y,536
 netspresso/compressor/core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 netspresso/compressor/core/compression.py,sha256=XzLukrfHTYEJQPF0A01iYbVZEjKRfgweIMEmGsfpfXc,563
 netspresso/compressor/core/model.py,sha256=bDK_y5dtUxS3_uFEMhSbmv851hglfsA9w5YSLf9RhZE,521
-netspresso-0.1.0.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-netspresso-0.1.0.dist-info/METADATA,sha256=RTPbXOIBkk1-5ycY2Ps1g4JLbKzzgSbd_JzRzH2Fatw,3790
-netspresso-0.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-netspresso-0.1.0.dist-info/top_level.txt,sha256=aHBNCm2tepEeTCUHu2_PVIlFG6iGuQReNl0js5hzjdU,11
-netspresso-0.1.0.dist-info/RECORD,,
+netspresso-0.1.1.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+netspresso-0.1.1.dist-info/METADATA,sha256=00DLsHyQd152eWEdbSvU1XFim_xzHxURj17HrlOd4co,3790
+netspresso-0.1.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+netspresso-0.1.1.dist-info/top_level.txt,sha256=aHBNCm2tepEeTCUHu2_PVIlFG6iGuQReNl0js5hzjdU,11
+netspresso-0.1.1.dist-info/RECORD,,
```

