# Comparing `tmp/inference_client-0.0.4.tar.gz` & `tmp/inference_client-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inference_client-0.0.4.tar", max compression
+gzip compressed data, was "inference_client-0.0.5.tar", max compression
```

## Comparing `inference_client-0.0.4.tar` & `inference_client-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0    11357 2023-05-19 09:49:28.989063 inference_client-0.0.4/LICENSE
--rw-r--r--   0        0        0     7335 2023-05-19 09:49:28.989063 inference_client-0.0.4/README.md
--rw-r--r--   0        0        0      256 2023-05-19 09:49:29.041063 inference_client-0.0.4/inference_client/__init__.py
--rw-r--r--   0        0        0     2349 2023-05-19 09:49:29.041063 inference_client-0.0.4/inference_client/__version__.py
--rw-r--r--   0        0        0      499 2023-05-19 09:49:29.041063 inference_client-0.0.4/inference_client/base.py
--rw-r--r--   0        0        0     1555 2023-05-19 09:49:29.041063 inference_client-0.0.4/inference_client/client.py
--rw-r--r--   0        0        0      719 2023-05-19 09:49:29.041063 inference_client-0.0.4/inference_client/config.py
--rw-r--r--   0        0        0     3129 2023-05-19 09:49:29.041063 inference_client-0.0.4/inference_client/helper.py
--rw-r--r--   0        0        0      250 2023-05-19 09:49:29.041063 inference_client-0.0.4/inference_client/logging.py
--rw-r--r--   0        0        0     3522 2023-05-19 09:49:29.041063 inference_client-0.0.4/inference_client/tasks/caption.py
--rw-r--r--   0        0        0     5819 2023-05-19 09:49:29.041063 inference_client-0.0.4/inference_client/tasks/encode.py
--rw-r--r--   0        0        0     3642 2023-05-19 09:49:29.041063 inference_client-0.0.4/inference_client/tasks/generate.py
--rw-r--r--   0        0        0     2378 2023-05-19 09:49:29.041063 inference_client-0.0.4/inference_client/tasks/helper.py
--rw-r--r--   0        0        0     6127 2023-05-19 09:49:29.041063 inference_client-0.0.4/inference_client/tasks/rank.py
--rw-r--r--   0        0        0     3904 2023-05-19 09:49:29.041063 inference_client-0.0.4/inference_client/tasks/vqa.py
--rw-r--r--   0        0        0     1355 2023-05-19 09:49:29.041063 inference_client-0.0.4/pyproject.toml
--rw-r--r--   0        0        0    19715 1970-01-01 00:00:00.000000 inference_client-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-01 08:40:10.429325 inference_client-0.0.5/LICENSE
+-rw-r--r--   0        0        0     7312 2023-06-01 08:40:10.429325 inference_client-0.0.5/README.md
+-rw-r--r--   0        0        0      256 2023-06-01 08:40:10.481326 inference_client-0.0.5/inference_client/__init__.py
+-rw-r--r--   0        0        0     2349 2023-06-01 08:40:10.481326 inference_client-0.0.5/inference_client/__version__.py
+-rw-r--r--   0        0        0     1546 2023-06-01 08:40:10.481326 inference_client-0.0.5/inference_client/client.py
+-rw-r--r--   0        0        0      719 2023-06-01 08:40:10.481326 inference_client-0.0.5/inference_client/config.py
+-rw-r--r--   0        0        0     3129 2023-06-01 08:40:10.481326 inference_client-0.0.5/inference_client/helper.py
+-rw-r--r--   0        0        0      250 2023-06-01 08:40:10.481326 inference_client-0.0.5/inference_client/logging.py
+-rw-r--r--   0        0        0      551 2023-06-01 08:40:10.481326 inference_client-0.0.5/inference_client/model.py
+-rw-r--r--   0        0        0     3541 2023-06-01 08:40:10.481326 inference_client-0.0.5/inference_client/tasks/caption.py
+-rw-r--r--   0        0        0     5855 2023-06-01 08:40:10.481326 inference_client-0.0.5/inference_client/tasks/encode.py
+-rw-r--r--   0        0        0     3664 2023-06-01 08:40:10.481326 inference_client-0.0.5/inference_client/tasks/generate.py
+-rw-r--r--   0        0        0     2389 2023-06-01 08:40:10.481326 inference_client-0.0.5/inference_client/tasks/helper.py
+-rw-r--r--   0        0        0     6174 2023-06-01 08:40:10.481326 inference_client-0.0.5/inference_client/tasks/rank.py
+-rw-r--r--   0        0        0    11539 2023-06-01 08:40:10.481326 inference_client-0.0.5/inference_client/tasks/upscale.py
+-rw-r--r--   0        0        0     3929 2023-06-01 08:40:10.481326 inference_client-0.0.5/inference_client/tasks/vqa.py
+-rw-r--r--   0        0        0     1355 2023-06-01 08:40:10.481326 inference_client-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    19692 1970-01-01 00:00:00.000000 inference_client-0.0.5/PKG-INFO
```

### Comparing `inference_client-0.0.4/LICENSE` & `inference_client-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.4/README.md` & `inference_client-0.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,15 @@
 
 ```bash
 the merlion fountain in singapore
 ```
 
 ## Documentation
 
-For more information about advanced usage of Inference Client, please refer to the [documentation](https://docs.jina.ai/advanced/experimental/inference-client/).
+For more information about advanced usage of Inference Client, please refer to the [documentation](https://jina.readme.io/docs/inference).
 
 ## Support
 
 - Join our [Slack community](https://slack.jina.ai) and chat with other community members about ideas.
 - Watch our [Engineering All Hands](https://youtube.com/playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) to learn Jina's new features and stay up-to-date with the latest AI techniques.
 - Subscribe to the latest video tutorials on our [YouTube channel](https://youtube.com/c/jina-ai)
```

#### html2text {}

```diff
@@ -78,15 +78,15 @@
 either a DocumentArray of images and questions, or a single plain image and
 question. ```python # Initialize model model = client.get_model('Salesforce/
 blip2-opt-2.7b') image = 'singapore.jpg' question = 'Question: What is this
 photo about? Answer:' response = model.vqa(image=image, question=question) #
 Access the answers print(response[0].tags['response']) ``` ```bash the merlion
 fountain in singapore ``` ## Documentation For more information about advanced
 usage of Inference Client, please refer to the [documentation](https://
-docs.jina.ai/advanced/experimental/inference-client/). ## Support - Join our
-[Slack community](https://slack.jina.ai) and chat with other community members
-about ideas. - Watch our [Engineering All Hands](https://youtube.com/
+jina.readme.io/docs/inference). ## Support - Join our [Slack community](https:/
+/slack.jina.ai) and chat with other community members about ideas. - Watch our
+[Engineering All Hands](https://youtube.com/
 playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) to learn Jina's new features
 and stay up-to-date with the latest AI techniques. - Subscribe to the latest
 video tutorials on our [YouTube channel](https://youtube.com/c/jina-ai) ##
 License Inference Client is backed by [Jina AI](https://jina.ai) and licensed
 under [Apache-2.0](./LICENSE).
```

### Comparing `inference_client-0.0.4/inference_client/__version__.py` & `inference_client-0.0.5/inference_client/__version__.py`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.4/inference_client/client.py` & `inference_client-0.0.5/inference_client/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from functools import lru_cache
 from typing import Optional
 
-from .base import BaseClient
 from .helper import get_model_spec, login
+from .model import Model
 
 
 class Client:
     """
     A Python client for accessing models that are hosted on Jina Cloud.
     """
 
@@ -45,12 +45,12 @@
                 'Please provide an endpoint or a valid user token to access the model.'
             )
 
         if model_name:
             spec = get_model_spec(model_name, self._auth_token)
             endpoint = spec['endpoints']['grpc']
 
-        return BaseClient(
+        return Model(
             model_name=model_name,
             token=self._auth_token,
             host=endpoint,
         )
```

### Comparing `inference_client-0.0.4/inference_client/config.py` & `inference_client-0.0.5/inference_client/config.py`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.4/inference_client/helper.py` & `inference_client-0.0.5/inference_client/helper.py`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.4/inference_client/tasks/caption.py` & `inference_client-0.0.5/inference_client/tasks/caption.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,36 +15,37 @@
     Mixin class for captioning documents.
     """
 
     token: str
     client: Client
 
     @overload
-    def caption(self, image: Union[str, bytes, 'ArrayType'], **kwargs):
+    def caption(self, *, image: Union[str, bytes, 'ArrayType'], **kwargs):
         """
         caption image # TODO: add image type
 
         :param image: the image to caption, can be a `ndarray`, 'bytes' or uri of the image
         :param kwargs: additional arguments to pass to the model
         """
         ...
 
     @overload
-    def caption(self, docs: Union[Iterable['Document'], 'DocumentArray'], **kwargs):
+    def caption(self, *, docs: Union[Iterable['Document'], 'DocumentArray'], **kwargs):
         """
         caption documents
 
         :param docs: the documents to caption
         :param kwargs: additional arguments to pass to the model
         """
         ...
 
     @overload
     def caption(
         self,
+        *,
         docs: Optional[Union[Iterable['Document'], 'DocumentArray']] = None,
         image: Optional[Union[str, bytes, 'ArrayType']] = None,
         **kwargs,
     ):
         """
         Generate a caption for an image or a set of documents using a pre-trained model.
 
@@ -54,16 +55,16 @@
         """
         ...
 
     def caption(self, **kwargs):
         """
         Caption the documents using the model.
 
-        :param kwargs: additional arguments to pass to the model
-        :return: captioned content
+        :param kwargs: additional arguments to pass to the model.
+        :return: captioned content.
         """
         payload, content_type = self._get_caption_payload(**kwargs)
         result = self.client.post(**payload)
         return self._unbox_caption_result(
             result=result,
             content_type=content_type,
         )
```

### Comparing `inference_client-0.0.4/inference_client/tasks/encode.py` & `inference_client-0.0.5/inference_client/tasks/encode.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,57 +15,59 @@
     Mixin class for encoding documents.
     """
 
     token: str
     client: Client
 
     @overload
-    def encode(self, text: Union[str, Iterable[str]], **kwargs):
+    def encode(self, *, text: Union[str, Iterable[str]], **kwargs):
         """
-        Encode plain text
+        Encode plain text.
 
-        :param text: the text to encode
-        :param kwargs: additional arguments to pass to the model
+        :param text: the text to encode.
+        :param kwargs: additional arguments to pass to the model.
         """
         ...
 
     @overload
     def encode(
         self,
+        *,
         image: Union[
             str,
             bytes,
             'ArrayType',
             Iterable[str],
             Iterable[bytes],
             Iterable['ArrayType'],
         ],
         **kwargs,
     ):
         """
-        Encode image
+        Encode image.
 
-        :param image: the image to encode, can be a `ndarray`, 'bytes' or uri of the image
-        :param kwargs: additional arguments to pass to the model
+        :param image: the image to encode, can be a `ndarray`, 'bytes' or uri of the image.
+        :param kwargs: additional arguments to pass to the model.
         """
         ...
 
     @overload
-    def encode(self, docs: Union[Iterable['Document'], 'DocumentArray'], **kwargs):
+    def encode(self, *, docs: Union[Iterable['Document'], 'DocumentArray'], **kwargs):
         """
         Encode documents
 
         :param docs: the documents to encode
         :param kwargs: additional arguments to pass to the model
         """
         ...
 
     @overload
     def encode(
         self,
+        *,
         docs: Optional[Union[Iterable['Document'], 'DocumentArray']] = None,
         text: Optional[Union[str, Iterable[str]]] = None,
         image: Optional[
             Union[
                 str,
                 bytes,
                 'ArrayType',
@@ -86,16 +88,16 @@
         """
         ...
 
     def encode(self, **kwargs):
         """
         Encode the documents using the model.
 
-        :param kwargs: additional arguments to pass to the model
-        :return: encoded content
+        :param kwargs: additional arguments to pass to the model.
+        :return: encoded content.
         """
         payload, content_type, is_list = self._get_enocde_payload(**kwargs)
         result = self.client.post(**payload)
         return self._unbox_encode_result(
             result=result,
             content_type=content_type,
             is_list=is_list,
```

### Comparing `inference_client-0.0.4/inference_client/tasks/generate.py` & `inference_client-0.0.5/inference_client/tasks/generate.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,34 +17,35 @@
     client: 'Client'
 
     @overload
     def generate(self, prompts: Union[str, List[str]], **kwargs):
         """
         Generate text from prompts using the model.
 
-        :param prompts: the prompts to generate text from
-        :param kwargs: additional arguments to pass to the model
+        :param prompts: the prompts to generate text from.
+        :param kwargs: additional arguments to pass to the model.
         """
         ...
 
     @overload
-    def generate(self, prompt: str, inplace_images: List = [], **kwargs):
+    def generate(self, prompts: str, *, inplace_images: List = [], **kwargs):
         """
         Generate text from prompts using the model.
 
-        :param prompt: the prompt to generate text from
-        :param inplace_images: the images to generate text from
-        :param kwargs: additional arguments to pass to the model
+        :param prompts: the prompt to generate text from.
+        :param inplace_images: the images to generate text from.
+        :param kwargs: additional arguments to pass to the model.
         """
         ...
 
     @overload
     def generate(
         self,
         prompts: Union[str, List[str]],
+        *,
         max_new_tokens: Optional[int] = None,
         num_beams: int = 1,
         do_sample: bool = False,
         temperature: float = 1.0,
         top_k: int = 1,
         top_p: float = 0.9,
         repetition_penalty: float = 1.0,
@@ -63,15 +64,15 @@
         :param top_p: The cumulative probability of parameter highest probability vocabulary tokens to keep for nucleus sampling. Only relevant if do_sample is True.
         :param repetition_penalty: The parameter for repetition penalty. 1.0 means no penalty.
         :param length_penalty: Exponential penalty to the length that is used with beam-based generation.
                 It is applied as an exponent to the sequence length, which in turn is used to divide the score of the sequence.
                 Since the score is the log likelihood of the sequence (i.e. negative), length_penalty > 0.0 promotes longer sequences,
                 while length_penalty < 0.0 encourages shorter sequences.
         :param no_repeat_ngram_size: If set to int > 0, all ngrams of that size can only occur once.
-        :param kwargs: additional arguments to pass to the model
+        :param kwargs: additional arguments to pass to the model.
         """
         ...
 
     def generate(self, prompts: Union[str, List[str]], **kwargs):
         """Generate text from the given prompt.
 
         :param prompts: The prompt(s) to generate from.
```

### Comparing `inference_client-0.0.4/inference_client/tasks/helper.py` & `inference_client-0.0.5/inference_client/tasks/helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional
+from typing import Callable, Optional
 
 from docarray import Document
 
 
 def load_plain_into_document(content, mime_type: Optional[str] = None):
     """
     Load plain input into document. If the raw input is a str, it will automatically load into text or image Document
@@ -35,27 +35,27 @@
         raise TypeError(f"Cannot convert content to Document")
 
 
 def iter_doc(content):
     """
     Iterate over the input content and yield Document.
 
-    :param content: input content to be converted/loaded to Document
+    :param content: input content to be converted/loaded to Document.
     :yield: a Document
     """
     for c in content:
         if c.content_type in ('text', 'blob'):
             d = c
         elif not c.blob and c.uri:
             c.load_uri_to_blob()
             d = c
         elif c.tensor is not None:
             d = c
         else:
-            raise TypeError(f'unsupported input type {c!r} {c.content_type}')
+            raise TypeError(f'Unsupported input type {c!r} {c.content_type}')
         yield d
 
 
 def get_base_payload(endpoint, token, **kwargs):
     """
     Get the base payload for the request.
```

### Comparing `inference_client-0.0.4/inference_client/tasks/rank.py` & `inference_client-0.0.5/inference_client/tasks/rank.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,79 +17,82 @@
 
     token: str
     client: Client
 
     @overload
     def rank(
         self,
+        *,
         text: str,
         candidates: Iterable[Union[str, bytes, 'ArrayType']],
         **kwargs,
     ):
         """
         Rank the documents using the model.
 
-        :param text: the reference text
-        :param candidates: the candidates to be ranked, can be either a list of strings or a list of images
-        :param kwargs: additional arguments to pass to the model
+        :param text: the reference text.
+        :param candidates: the candidates to be ranked, can be either a list of strings or a list of images.
+        :param kwargs: additional arguments to pass to the model.
         """
         ...
 
     @overload
     def rank(
         self,
+        *,
         image: Union[str, bytes, 'ArrayType'],
         candidates: Iterable[Union[str, bytes, 'ArrayType']],
         **kwargs,
     ):
         """
         Rank the documents using the model.
 
-        :param image: the reference image, can be a `ndarray`, 'bytes' or uri of the image
-        :param candidates: the candidates to be ranked, can be either a list of strings or a list of images
-        :param kwargs: additional arguments to pass to the model
+        :param image: the reference image, can be a `ndarray`, 'bytes' or uri of the image.
+        :param candidates: the candidates to be ranked, can be either a list of strings or a list of images.
+        :param kwargs: additional arguments to pass to the model.
         """
         ...
 
     @overload
-    def rank(self, docs: Union[Iterable['Document'], 'DocumentArray'], **kwargs):
+    def rank(self, *, docs: Union[Iterable['Document'], 'DocumentArray'], **kwargs):
         """
         Rank the documents using the model.
 
-        :param docs: the documents to be ranked with candidates stored in the matches
-        :param kwargs: additional arguments to pass to the model
+        :param docs: the documents to be ranked with candidates stored in the matches.
+        :param kwargs: additional arguments to pass to the model.
         """
         ...
 
     @overload
     def rank(
         self,
+        *,
         docs: Optional[Union[Iterable['Document'], 'DocumentArray']] = None,
         text: Optional[str] = None,
         image: Optional[Union[str, bytes, 'ArrayType']] = None,
         candidates: Optional[Iterable[Union[str, bytes, 'ArrayType']]] = None,
         **kwargs,
     ):
         """
         Rank the documents using the model.
 
         :param docs: the documents to be ranked with candidates stored in the matches. Default: None.
         :param text: the reference text. Default: None.
         :param image: the reference image, can be a `ndarray`, 'bytes' or uri of the image. Default: None.
         :param candidates: the candidates to be ranked, can be either a list of strings or a list of images. Default: None.
-        :param kwargs: additional arguments to pass to the model
+        :param kwargs: additional arguments to pass to the model.
         """
         ...
 
     def rank(self, **kwargs):
         """
         Rank the documents using the model.
 
-        :param kwargs: additional arguments to pass to the model
-        :return: ranked content
+        :param kwargs: additional arguments to pass to the model.
+        :return: ranked content.
         """
         payload, content_type = self._get_rank_payload(**kwargs)
         result = self.client.post(**payload)
         return self._unbox_rank_result(
             result=result,
             content_type=content_type,
         )
```

### Comparing `inference_client-0.0.4/inference_client/tasks/vqa.py` & `inference_client-0.0.5/inference_client/tasks/vqa.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,58 +15,59 @@
     Mixin class for VQA documents.
     """
 
     token: str
     client: Client
 
     @overload
-    def vqa(self, image: Union[str, bytes, 'ArrayType'], question: str, **kwargs):
+    def vqa(self, *, image: Union[str, bytes, 'ArrayType'], question: str, **kwargs):
         """
         Answer the question using the model.
 
-        :param image: the image that the question is about
-        :param question: the question to be answered
-        :param kwargs: additional arguments to pass to the model
+        :param image: the image that the question is about.
+        :param question: the question to be answered.
+        :param kwargs: additional arguments to pass to the model.
         """
         ...
 
     @overload
-    def vqa(self, docs: Union[Iterable['Document'], 'DocumentArray'], **kwargs):
+    def vqa(self, *, docs: Union[Iterable['Document'], 'DocumentArray'], **kwargs):
         """
         Answer the question using the model.
 
-        :param docs: the documents to be answered with image as root and question stored in the tags
-        :param kwargs: additional arguments to pass to the model
+        :param docs: the documents to be answered with image as root and question stored in the tags.
+        :param kwargs: additional arguments to pass to the model.
         """
         ...
 
     @overload
     def vqa(
         self,
+        *,
         docs: Optional[Union[Iterable['Document'], 'DocumentArray']] = None,
         image: Optional[Union[str, bytes, 'ArrayType']] = None,
         question: Optional[str] = None,
         **kwargs,
     ):
         """
         Answer the question using the model.
 
         :param docs: the documents to be answered with image as root and question stored in the tags. Default: None.
         :param image: the image that the question is about. Default: None.
         :param question: the question to be answered. Default: None.
-        :param kwargs: additional arguments to pass to the model
+        :param kwargs: additional arguments to pass to the model.
         """
         ...
 
     def vqa(self, **kwargs):
         """
         Answer the question using the model.
 
-        :param kwargs: additional arguments to pass to the model
-        :return: answered content
+        :param kwargs: additional arguments to pass to the model.
+        :return: answered content.
         """
         payload, content_type = self._get_vqa_payload(**kwargs)
         result = self.client.post(**payload)
         return self._unbox_vqa_result(
             result=result,
             content_type=content_type,
         )
```

### Comparing `inference_client-0.0.4/pyproject.toml` & `inference_client-0.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inference_client"
-version = "0.0.4"
+version = "0.0.5"
 description = "Python Client for Jina Inference API"
 
 license = "Apache-2.0"
 
 authors = [
     "Jina AI <hello@jina.ai>"
 ]
```

### Comparing `inference_client-0.0.4/PKG-INFO` & `inference_client-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inference-client
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python Client for Jina Inference API
 Home-page: https://inference-api.jina.ai
 License: Apache-2.0
 Keywords: jina,inference,api,client
 Author: Jina AI
 Author-email: hello@jina.ai
 Requires-Python: >=3.8,<4.0.0
@@ -220,15 +220,15 @@
 
 ```bash
 the merlion fountain in singapore
 ```
 
 ## Documentation
 
-For more information about advanced usage of Inference Client, please refer to the [documentation](https://docs.jina.ai/advanced/experimental/inference-client/).
+For more information about advanced usage of Inference Client, please refer to the [documentation](https://jina.readme.io/docs/inference).
 
 ## Support
 
 - Join our [Slack community](https://slack.jina.ai) and chat with other community members about ideas.
 - Watch our [Engineering All Hands](https://youtube.com/playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) to learn Jina's new features and stay up-to-date with the latest AI techniques.
 - Subscribe to the latest video tutorials on our [YouTube channel](https://youtube.com/c/jina-ai)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: inference-client Version: 0.0.4 Summary: Python
+Metadata-Version: 2.1 Name: inference-client Version: 0.0.5 Summary: Python
 Client for Jina Inference API Home-page: https://inference-api.jina.ai License:
 Apache-2.0 Keywords: jina,inference,api,client Author: Jina AI Author-email:
 hello@jina.ai Requires-Python: >=3.8,<4.0.0 Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Provides-Extra: pytorch
@@ -92,17 +92,17 @@
 either a DocumentArray of images and questions, or a single plain image and
 question. ```python # Initialize model model = client.get_model('Salesforce/
 blip2-opt-2.7b') image = 'singapore.jpg' question = 'Question: What is this
 photo about? Answer:' response = model.vqa(image=image, question=question) #
 Access the answers print(response[0].tags['response']) ``` ```bash the merlion
 fountain in singapore ``` ## Documentation For more information about advanced
 usage of Inference Client, please refer to the [documentation](https://
-docs.jina.ai/advanced/experimental/inference-client/). ## Support - Join our
-[Slack community](https://slack.jina.ai) and chat with other community members
-about ideas. - Watch our [Engineering All Hands](https://youtube.com/
+jina.readme.io/docs/inference). ## Support - Join our [Slack community](https:/
+/slack.jina.ai) and chat with other community members about ideas. - Watch our
+[Engineering All Hands](https://youtube.com/
 playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) to learn Jina's new features
 and stay up-to-date with the latest AI techniques. - Subscribe to the latest
 video tutorials on our [YouTube channel](https://youtube.com/c/jina-ai) ##
 License Inference Client is backed by [Jina AI](https://jina.ai) and licensed
 under [Apache-2.0](./LICENSE). Apache License Version 2.0, January 2004 http://
 www.apache.org/licenses/ TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND
 DISTRIBUTION 1. Definitions. "License" shall mean the terms and conditions for
```

