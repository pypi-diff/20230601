# Comparing `tmp/stabilityai-1.0.1.tar.gz` & `tmp/stabilityai-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stabilityai-1.0.1.tar", last modified: Fri May 26 19:16:33 2023, max compression
+gzip compressed data, was "stabilityai-1.0.2.tar", last modified: Thu Jun  1 14:32:04 2023, max compression
```

## Comparing `stabilityai-1.0.1.tar` & `stabilityai-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:16:33.181263 stabilityai-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:16:33.177263 stabilityai-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:16:33.177263 stabilityai-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-26 19:16:22.000000 stabilityai-1.0.1/.github/workflows/build-and-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-26 19:16:22.000000 stabilityai-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 19:16:22.000000 stabilityai-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-26 19:16:33.181263 stabilityai-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-26 19:16:22.000000 stabilityai-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-26 19:16:22.000000 stabilityai-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-26 19:16:22.000000 stabilityai-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 19:16:33.181263 stabilityai-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:16:33.177263 stabilityai-1.0.1/stabilityai/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 19:16:22.000000 stabilityai-1.0.1/stabilityai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8889 2023-05-26 19:16:22.000000 stabilityai-1.0.1/stabilityai/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-26 19:16:22.000000 stabilityai-1.0.1/stabilityai/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-26 19:16:22.000000 stabilityai-1.0.1/stabilityai/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-26 19:16:22.000000 stabilityai-1.0.1/stabilityai/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-26 19:16:22.000000 stabilityai-1.0.1/stabilityai/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:16:33.181263 stabilityai-1.0.1/stabilityai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-26 19:16:33.000000 stabilityai-1.0.1/stabilityai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-26 19:16:33.000000 stabilityai-1.0.1/stabilityai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 19:16:33.000000 stabilityai-1.0.1/stabilityai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-26 19:16:33.000000 stabilityai-1.0.1/stabilityai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 19:16:33.000000 stabilityai-1.0.1/stabilityai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:04.107526 stabilityai-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:04.103526 stabilityai-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:04.103526 stabilityai-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-01 14:31:47.000000 stabilityai-1.0.2/.github/workflows/build-and-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-01 14:31:47.000000 stabilityai-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-01 14:31:47.000000 stabilityai-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-01 14:32:04.107526 stabilityai-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-01 14:31:47.000000 stabilityai-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-01 14:31:47.000000 stabilityai-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-01 14:31:47.000000 stabilityai-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:32:04.107526 stabilityai-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:04.107526 stabilityai-1.0.2/stabilityai/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 14:31:47.000000 stabilityai-1.0.2/stabilityai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-06-01 14:31:47.000000 stabilityai-1.0.2/stabilityai/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-01 14:31:47.000000 stabilityai-1.0.2/stabilityai/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-01 14:31:47.000000 stabilityai-1.0.2/stabilityai/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-06-01 14:31:47.000000 stabilityai-1.0.2/stabilityai/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-01 14:31:47.000000 stabilityai-1.0.2/stabilityai/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:04.107526 stabilityai-1.0.2/stabilityai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-01 14:32:04.000000 stabilityai-1.0.2/stabilityai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-01 14:32:04.000000 stabilityai-1.0.2/stabilityai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:32:04.000000 stabilityai-1.0.2/stabilityai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-01 14:32:04.000000 stabilityai-1.0.2/stabilityai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 14:32:04.000000 stabilityai-1.0.2/stabilityai.egg-info/top_level.txt
```

### Comparing `stabilityai-1.0.1/.github/workflows/build-and-publish.yml` & `stabilityai-1.0.2/.github/workflows/build-and-publish.yml`

 * *Files identical despite different names*

### Comparing `stabilityai-1.0.1/.gitignore` & `stabilityai-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `stabilityai-1.0.1/LICENSE` & `stabilityai-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stabilityai-1.0.1/PKG-INFO` & `stabilityai-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stabilityai
-Version: 1.0.1
+Version: 1.0.2
 Summary: *Unofficial* client for the Stability REST API
 Author-email: Estelle Poulin <dev@inspiredby.es>
 License: GPLv3
 Project-URL: homepage, https://github.com/estheruary/stabilityai
 Project-URL: repository, https://github.com/estheruary/stabilityai
 Project-URL: changelog, https://github.com/estheruary/stabilityai/-/blob/main/CHANGELOG.md
 Keywords: stabilityai,bot
```

### Comparing `stabilityai-1.0.1/README.md` & `stabilityai-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `stabilityai-1.0.1/pyproject.toml` & `stabilityai-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stabilityai-1.0.1/stabilityai/client.py` & `stabilityai-1.0.2/stabilityai/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from stabilityai.constants import (
     DEFAULT_GENERATION_ENGINE,
     DEFAULT_STABILITY_API_HOST,
     DEFAULT_STABILITY_CLIENT_ID,
     DEFAULT_STABILITY_CLIENT_VERSION,
     DEFAULT_UPSCALE_ENGINE,
 )
-from stabilityai.exceptions import YouNeedToUseAContextManager
+from stabilityai.exceptions import ThisFunctionRequiresAPrompt, YouNeedToUseAContextManager
 from stabilityai.models import (
     AccountResponseBody,
     BalanceResponseBody,
     CfgScale,
     ClipGuidancePreset,
     DiffuseImageHeight,
     DiffuseImageWidth,
@@ -123,15 +123,15 @@
 
     def _normalize_text_prompts(
         self,
         text_prompts: Optional[TextPrompts],
         text_prompt: Optional[SingleTextPrompt]
     ):
         if not bool(text_prompt) ^ bool(text_prompts):
-            raise RuntimeError(
+            raise ThisFunctionRequiresAPrompt(
                 textwrap.dedent(
                     f"""\
                     You must provide one of text_prompt and text_prompts.
 
                     Do this
 
                         stability.text_to_image(
@@ -199,14 +199,35 @@
             f"/v1/generation/{engine_id}/text-to-image",
             data=json.dumps(omit_none(json.loads(request_body.json()))),
         )
         Sampler.K_DPMPP_2M
 
         return TextToImageResponseBody.parse_obj(await res.json())
 
+    async def text_to_image_simple(
+        self,
+        prompt: str,
+        style_preset: Optional[StylePreset] = StylePreset.digital_art,
+        n: int = 1,
+        size: str = "512x512",
+    ):
+        """
+        An OpenAI SDK style call that makes it easy to migrate.
+        """
+
+        dim = int(size.split("x")[0])
+
+        return await self.text_to_image(
+            text_prompts=[TextPrompt(text=prompt)],
+            style_preset=style_preset,
+            samples=n,
+            width=dim,
+            height=dim,
+        )
+
     @validate_arguments
     async def image_to_image(
         self,
         text_prompts: TextPrompts,
         text_prompt: SingleTextPrompt,
         init_image: InitImage,
         *,
```

### Comparing `stabilityai-1.0.1/stabilityai/models.py` & `stabilityai-1.0.2/stabilityai/models.py`

 * *Files identical despite different names*

### Comparing `stabilityai-1.0.1/stabilityai.egg-info/PKG-INFO` & `stabilityai-1.0.2/stabilityai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stabilityai
-Version: 1.0.1
+Version: 1.0.2
 Summary: *Unofficial* client for the Stability REST API
 Author-email: Estelle Poulin <dev@inspiredby.es>
 License: GPLv3
 Project-URL: homepage, https://github.com/estheruary/stabilityai
 Project-URL: repository, https://github.com/estheruary/stabilityai
 Project-URL: changelog, https://github.com/estheruary/stabilityai/-/blob/main/CHANGELOG.md
 Keywords: stabilityai,bot
```

