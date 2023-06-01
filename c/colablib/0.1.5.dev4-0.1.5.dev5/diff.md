# Comparing `tmp/colablib-0.1.5.dev4.tar.gz` & `tmp/colablib-0.1.5.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colablib-0.1.5.dev4.tar", last modified: Thu Jun  1 14:06:00 2023, max compression
+gzip compressed data, was "colablib-0.1.5.dev5.tar", last modified: Thu Jun  1 14:18:06 2023, max compression
```

## Comparing `colablib-0.1.5.dev4.tar` & `colablib-0.1.5.dev5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 14:06:00.619721 colablib-0.1.5.dev4/
--rw-rw-rw-   0        0        0      218 2023-06-01 14:06:00.618667 colablib-0.1.5.dev4/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-06-01 08:34:56.000000 colablib-0.1.5.dev4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 14:06:00.604750 colablib-0.1.5.dev4/colablib/
--rw-rw-rw-   0        0        0        0 2023-06-01 08:53:08.000000 colablib-0.1.5.dev4/colablib/__init__.py
--rw-rw-rw-   0        0        0     1127 2023-06-01 09:15:56.000000 colablib-0.1.5.dev4/colablib/cprint.py
--rw-rw-rw-   0        0        0     1169 2023-06-01 11:43:55.000000 colablib-0.1.5.dev4/colablib/deb_utils.py
--rw-rw-rw-   0        0        0     2408 2023-06-01 09:46:58.000000 colablib-0.1.5.dev4/colablib/git_utils.py
--rw-rw-rw-   0        0        0     9467 2023-06-01 12:35:18.000000 colablib-0.1.5.dev4/colablib/model_validators.py
--rw-rw-rw-   0        0        0     3330 2023-06-01 12:22:37.000000 colablib-0.1.5.dev4/colablib/py_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-01 14:06:00.617355 colablib-0.1.5.dev4/colablib.egg-info/
--rw-rw-rw-   0        0        0      218 2023-06-01 14:06:00.000000 colablib-0.1.5.dev4/colablib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-06-01 14:06:00.000000 colablib-0.1.5.dev4/colablib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 14:06:00.000000 colablib-0.1.5.dev4/colablib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-01 14:06:00.000000 colablib-0.1.5.dev4/colablib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 14:06:00.619721 colablib-0.1.5.dev4/setup.cfg
--rw-rw-rw-   0        0        0      316 2023-06-01 14:05:44.000000 colablib-0.1.5.dev4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 14:18:06.973576 colablib-0.1.5.dev5/
+-rw-rw-rw-   0        0        0      218 2023-06-01 14:18:06.973576 colablib-0.1.5.dev5/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2023-06-01 08:34:56.000000 colablib-0.1.5.dev5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 14:18:06.956185 colablib-0.1.5.dev5/colablib/
+-rw-rw-rw-   0        0        0        0 2023-06-01 08:53:08.000000 colablib-0.1.5.dev5/colablib/__init__.py
+-rw-rw-rw-   0        0        0     1127 2023-06-01 09:15:56.000000 colablib-0.1.5.dev5/colablib/cprint.py
+-rw-rw-rw-   0        0        0     1169 2023-06-01 11:43:55.000000 colablib-0.1.5.dev5/colablib/deb_utils.py
+-rw-rw-rw-   0        0        0     2408 2023-06-01 09:46:58.000000 colablib-0.1.5.dev5/colablib/git_utils.py
+-rw-rw-rw-   0        0        0     8696 2023-06-01 14:17:34.000000 colablib-0.1.5.dev5/colablib/model_validators.py
+-rw-rw-rw-   0        0        0     3330 2023-06-01 12:22:37.000000 colablib-0.1.5.dev5/colablib/py_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-01 14:18:06.971576 colablib-0.1.5.dev5/colablib.egg-info/
+-rw-rw-rw-   0        0        0      218 2023-06-01 14:18:06.000000 colablib-0.1.5.dev5/colablib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-06-01 14:18:06.000000 colablib-0.1.5.dev5/colablib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 14:18:06.000000 colablib-0.1.5.dev5/colablib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-01 14:18:06.000000 colablib-0.1.5.dev5/colablib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 14:18:06.974575 colablib-0.1.5.dev5/setup.cfg
+-rw-rw-rw-   0        0        0      316 2023-06-01 14:16:52.000000 colablib-0.1.5.dev5/setup.py
```

### Comparing `colablib-0.1.5.dev4/colablib/cprint.py` & `colablib-0.1.5.dev5/colablib/cprint.py`

 * *Files identical despite different names*

### Comparing `colablib-0.1.5.dev4/colablib/deb_utils.py` & `colablib-0.1.5.dev5/colablib/deb_utils.py`

 * *Files identical despite different names*

### Comparing `colablib-0.1.5.dev4/colablib/git_utils.py` & `colablib-0.1.5.dev5/colablib/git_utils.py`

 * *Files identical despite different names*

### Comparing `colablib-0.1.5.dev4/colablib/model_validators.py` & `colablib-0.1.5.dev5/colablib/model_validators.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,178 +3,179 @@
 import torch
 import json
 import hashlib
 from torch import load
 from safetensors.torch import load_file, safe_open
 from .cprint import cprint
 
-def is_safetensors(path):
-    return os.path.splitext(path)[1].lower() == '.safetensors'
-
-def is_ckpt(path):
-    return os.path.splitext(path)[1].lower() == '.ckpt'
+class Validator:
+    """
+    Validator is a helper class for validating models, vae, and lora. 
+    It provides utility methods for checking and loading different types of files.
+    """
+
+    # Define lora parameters as class variables
+    lora_args = lora_dim = lora_alpha = lora_module = lora_d8ahazard = None
+    lora_conv_dim = lora_conv_alpha = lora_algo = lora_unit = lora_type = None
+
+    @staticmethod
+    def is_safetensors(path):
+        """
+        Checks if the given path corresponds to a safetensors file.
+        """
+        return os.path.splitext(path)[1].lower() == '.safetensors'
+
+    @staticmethod
+    def is_ckpt(path):
+        """
+        Checks if the given path corresponds to a checkpoint file.
+        """
+        return os.path.splitext(path)[1].lower() == '.ckpt'
+
+    @staticmethod
+    def validate_model(model_path, map_location="cpu"):
+        """
+        Validates the model by attempting to load it.
+        """
+        if Validator.is_safetensors(model_path):
+            return Validator._attempt_load(model_path, load_file, map_location, ".ckpt")
+        elif Validator.is_ckpt(model_path):
+            return Validator._attempt_load(model_path, load, map_location, ".safetensors")
+        else:
+            return None
 
-def validate_model(model_path, map_location="cpu"):
-    if is_safetensors(model_path):
-        try:
-            tmp = load_file(model_path, device=map_location)
-            del tmp
-            gc.collect()
-            torch.cuda.empty_cache()
-        except Exception as e:
-            new_model_path = os.path.splitext(model_path)[0] + ".ckpt"
-            os.rename(model_path, new_model_path)
-            cprint(f"Model Info: model renamed to {os.path.basename(new_model_path)}", color="green")
-            return new_model_path
-    elif is_ckpt(model_path):
+    @staticmethod
+    def _attempt_load(model_path, load_func, map_location, new_ext):
+        """
+        Attempts to load a model given a specific load function, map location, and new extension.
+        """
         try:
-            tmp = load(model_path, map_location=map_location)
+            tmp = load_func(model_path, device=map_location)
             del tmp
             gc.collect()
             torch.cuda.empty_cache()
-        except Exception as e:
-            new_model_path = os.path.splitext(model_path)[0] + ".safetensors"
+        except Exception:
+            new_model_path = os.path.splitext(model_path)[0] + new_ext
             os.rename(model_path, new_model_path)
             cprint(f"Model Info: model renamed to {os.path.basename(new_model_path)}", color="green")
             return new_model_path
+        return None
 
-    return None
+    @staticmethod
+    def validate_vae(vae_path):
+        """
+        Validates the vae by checking if its sha256 hash is in the expected hash list.
+        """
+        expected_hash = {
+            'Animevae'                                : 'f921fb3f29891d2a77a6571e56b8b5052420d2884129517a333c60b1b4816cdf',
+            'kl-f8-anime'                             : '2f11c4a99ddc28d0ad8bce0acc38bed310b45d38a3fe4bb367dc30f3ef1a4868',
+            'kl-f8-anime2'                            : 'df3c506e51b7ee1d7b5a6a2bb7142d47d488743c96aa778afb0f53a2cdc2d38d',
+            'autoencoder_fix_kl-f8-trinart_characters': '2453b80bc1716bc3f94496d4e56be891e267051dc43c5144f384b66a73ac8295',
+            'vae-ft-mse-840000-ema-pruned'            : 'c6a580b13a5bc05a5e16e4dbb80608ff2ec251a162311590c1f34c013d7f3dab',
+            'mse840000_klf8anime'                     : '53cfd845736459e78f208786f8d56109093f37dc427e366769416f6ca9ea6fc9',
+            'mse840000_klf8anime_klf8anime2'          : 'a9a44822203eaa05104d37a242ec5af405d0fcfb98a81fb89f0c2e8bb71ae962',
+            'ClearVAE'                                : '600345c503784cd77536d714f0e4c43f9e1fa4379007e730d54c454c66ee36db',
+            'ClearVAE-NansLessTest'                   : '4809659b70d67d314c45062ece33a7f9f8abc9aaf13805173a129cad2664e091',
+            'ClearVAE-Variant'                        : '9c2d6dc265bd4758042cc2385b090aede02d8160b556830e9385db8a74ddcaab', 
+            'ACertainThing-0064'                      : '319adc806290ec775f361bac6c68a878a96c9982e1dd77c9545240cc811c4e58',
+            'flat_paint_b_v2'                         : '2da3f767874561a7e0e52ef2c24c8a0ea2997fd267727cfd2981fd9594e8bbd4',
+            'flat_paint_b_v3'                         : '0b4ff3b7be8c164b2a80d3a3a7c5eebc41a11994420a8633abf8190cff9cfc9c',
+            'SD15NewVAEpruned'                        : '27a4ac756c5c4fb25bfb7bd32a700a89fe77a66926338b1d78b97e25e1e85f75'
+        }
+        with open(vae_path, 'rb') as file:
+            contents = file.read()
+        sha256_hash = hashlib.sha256(contents).hexdigest()
+        for vae_name, hash_value in expected_hash.items():
+            if hash_value == sha256_hash:
+                cprint(f"VAE Info: VAE shared the same sha256 with {vae_name}.", color="green")
+                return
+
+    @staticmethod
+    def validate_lora(lora_path):
+        """
+        Validates lora by checking its metadata.
+        """
+        try:
+            lora_args = lora_dim = lora_alpha = lora_module = lora_d8ahazard = None
+            lora_conv_dim = lora_conv_alpha = lora_algo = lora_unit = lora_type = None
 
-def validate_vae(vae_path):
-    expected_hash = {
-        'Animevae'                                : 'f921fb3f29891d2a77a6571e56b8b5052420d2884129517a333c60b1b4816cdf',
-        'kl-f8-anime'                             : '2f11c4a99ddc28d0ad8bce0acc38bed310b45d38a3fe4bb367dc30f3ef1a4868',
-        'kl-f8-anime2'                            : 'df3c506e51b7ee1d7b5a6a2bb7142d47d488743c96aa778afb0f53a2cdc2d38d',
-        'autoencoder_fix_kl-f8-trinart_characters': '2453b80bc1716bc3f94496d4e56be891e267051dc43c5144f384b66a73ac8295',
-        'vae-ft-mse-840000-ema-pruned'            : 'c6a580b13a5bc05a5e16e4dbb80608ff2ec251a162311590c1f34c013d7f3dab',
-        'mse840000_klf8anime'                     : '53cfd845736459e78f208786f8d56109093f37dc427e366769416f6ca9ea6fc9',
-        'mse840000_klf8anime_klf8anime2'          : 'a9a44822203eaa05104d37a242ec5af405d0fcfb98a81fb89f0c2e8bb71ae962',
-        'ClearVAE'                                : '600345c503784cd77536d714f0e4c43f9e1fa4379007e730d54c454c66ee36db',
-        'ClearVAE-NansLessTest'                   : '4809659b70d67d314c45062ece33a7f9f8abc9aaf13805173a129cad2664e091',
-        'ClearVAE-Variant'                        : '9c2d6dc265bd4758042cc2385b090aede02d8160b556830e9385db8a74ddcaab', 
-        'ACertainThing-0064'                      : '319adc806290ec775f361bac6c68a878a96c9982e1dd77c9545240cc811c4e58',
-        'flat_paint_b_v2'                         : '2da3f767874561a7e0e52ef2c24c8a0ea2997fd267727cfd2981fd9594e8bbd4',
-        'flat_paint_b_v3'                         : '0b4ff3b7be8c164b2a80d3a3a7c5eebc41a11994420a8633abf8190cff9cfc9c',
-        'SD15NewVAEpruned'                        : '27a4ac756c5c4fb25bfb7bd32a700a89fe77a66926338b1d78b97e25e1e85f75'
-    }
-    with open(vae_path, 'rb') as file:
-        contents = file.read()
-
-    sha256_hash = hashlib.sha256(contents).hexdigest()
-
-    for vae_name, hash_value in expected_hash.items():
-        if hash_value == sha256_hash:
-            cprint(f"VAE Info: VAE shared the same sha256 with {vae_name}.", color="green")
-            return
-        
-def validate_vae(vae_path):
-    expected_hash = {
-        'Animevae'                                : 'f921fb3f29891d2a77a6571e56b8b5052420d2884129517a333c60b1b4816cdf',
-        'kl-f8-anime'                             : '2f11c4a99ddc28d0ad8bce0acc38bed310b45d38a3fe4bb367dc30f3ef1a4868',
-        'kl-f8-anime2'                            : 'df3c506e51b7ee1d7b5a6a2bb7142d47d488743c96aa778afb0f53a2cdc2d38d',
-        'autoencoder_fix_kl-f8-trinart_characters': '2453b80bc1716bc3f94496d4e56be891e267051dc43c5144f384b66a73ac8295',
-        'vae-ft-mse-840000-ema-pruned'            : 'c6a580b13a5bc05a5e16e4dbb80608ff2ec251a162311590c1f34c013d7f3dab',
-        'mse840000_klf8anime'                     : '53cfd845736459e78f208786f8d56109093f37dc427e366769416f6ca9ea6fc9',
-        'mse840000_klf8anime_klf8anime2'          : 'a9a44822203eaa05104d37a242ec5af405d0fcfb98a81fb89f0c2e8bb71ae962',
-        'ClearVAE'                                : '600345c503784cd77536d714f0e4c43f9e1fa4379007e730d54c454c66ee36db',
-        'ClearVAE-NansLessTest'                   : '4809659b70d67d314c45062ece33a7f9f8abc9aaf13805173a129cad2664e091',
-        'ClearVAE-Variant'                        : '9c2d6dc265bd4758042cc2385b090aede02d8160b556830e9385db8a74ddcaab', 
-        'ACertainThing-0064'                      : '319adc806290ec775f361bac6c68a878a96c9982e1dd77c9545240cc811c4e58',
-        'flat_paint_b_v2'                         : '2da3f767874561a7e0e52ef2c24c8a0ea2997fd267727cfd2981fd9594e8bbd4',
-        'flat_paint_b_v3'                         : '0b4ff3b7be8c164b2a80d3a3a7c5eebc41a11994420a8633abf8190cff9cfc9c',
-        'SD15NewVAEpruned'                        : '27a4ac756c5c4fb25bfb7bd32a700a89fe77a66926338b1d78b97e25e1e85f75'
-    }
-    with open(vae_path, 'rb') as file:
-        contents = file.read()
-
-    sha256_hash = hashlib.sha256(contents).hexdigest()
-
-    for vae_name, hash_value in expected_hash.items():
-        if hash_value == sha256_hash:
-            cprint(f"VAE Info: VAE shared the same sha256 with {vae_name}.", color="green")
-            return
-        
-def validate_lora(lora_path):
-    global lora_args, lora_dim, lora_alpha, lora_module, lora_d8ahazard
-    global lora_conv_dim, lora_conv_alpha, lora_algo, lora_unit, lora_type
-    
-    try:
-        lora_args = lora_dim = lora_alpha = lora_module = lora_d8ahazard = None
-        lora_conv_dim = lora_conv_alpha = lora_algo = lora_unit = lora_type = None
-
-        if is_safetensors(lora_path):
-            with safe_open(lora_path, framework="pt") as f:
-                metadata = f.metadata()
-
-            if metadata:
-                lora_args, lora_dim, lora_alpha, lora_module, lora_d8ahazard = (
-                    metadata.get(key) for key in ("ss_network_args", "ss_network_dim", "ss_network_alpha", "ss_network_module", "lora_key_encoding")
-                )
-                
-                if lora_module is not None:
-                    if lora_args is not None:
-                        lora_args_dict = json.loads(lora_args)
-                        lora_conv_dim, lora_conv_alpha, lora_algo, lora_unit = (
-                            lora_args_dict.get(key) for key in ("conv_dim", "conv_alpha", "algo", "unit")
-                        )
-                        lora_type = validate_kohya_lora(lora_module, lora_algo, lora_conv_dim, lora_conv_alpha)
-                    else:
-                        if 'networks.lora' in lora_module:
-                            lora_type = "LoRA_LierLa"
+            if Validator.is_safetensors(lora_path):
+                with safe_open(lora_path, framework="pt") as f:
+                    metadata = f.metadata()
+
+                if metadata:
+                    lora_args, lora_dim, lora_alpha, lora_module, lora_d8ahazard = (
+                        metadata.get(key) for key in ("ss_network_args", "ss_network_dim", "ss_network_alpha", "ss_network_module", "lora_key_encoding")
+                    )
+                    
+                    if lora_module is not None:
+                        if lora_args is not None:
+                            lora_args_dict = json.loads(lora_args)
+                            lora_conv_dim, lora_conv_alpha, lora_algo, lora_unit = (
+                                lora_args_dict.get(key) for key in ("conv_dim", "conv_alpha", "algo", "unit")
+                            )
+                            lora_type = Validator.validate_kohya_lora(lora_module, lora_algo, lora_conv_dim, lora_conv_alpha)
                         else:
-                            del metadata
-                            return (False, "LoRA Info: LoRA is not trained using 'kohya-ss/sd-scripts'")
+                            if 'networks.lora' in lora_module:
+                                lora_type = "LoRA_LierLa"
+                            else:
+                                del metadata
+                                return (False, "LoRA Info: LoRA is not trained using 'kohya-ss/sd-scripts'")
+
+                        data_dict = {
+                            "type"      : lora_type,
+                            "dim"       : lora_dim,
+                            "alpha"     : lora_alpha,
+                            "conv_dim"  : lora_conv_dim,
+                            "conv_alpha": lora_conv_alpha,
+                            "algo"      : lora_algo,
+                            "unit"      : lora_unit,
+                        }
+
+                        output_list = [f"{key}: {value}" for key, value in data_dict.items() if value is not None]
+                        
+                        del metadata
+                        return (True, f"LoRA Info: {output_list}")
+                    elif lora_d8ahazard is not None:
+                        del metadata
+                        return (False, "LoRA Info: LoRA is not trained using 'kohya-ss/sd-scripts' but using 'd8ahazard/sd_dreambooth_extension'")
+                else:
+                    del metadata
+                    return (True, "LoRA Info: No metadata saved")
+            else:
+                return (True, "LoRA Info: No metadata saved, your model is not in safetensors format")
+        except Exception as e:
+            cprint(f"An error occurred: {str(e)}", color="green")
 
-                    data_dict = {
-                        "type"      : lora_type,
-                        "dim"       : lora_dim,
-                        "alpha"     : lora_alpha,
-                        "conv_dim"  : lora_conv_dim,
-                        "conv_alpha": lora_conv_alpha,
-                        "algo"      : lora_algo,
-                        "unit"      : lora_unit,
-                    }
+    @staticmethod
+    def validate_kohya_lora(lora_module, lora_algo, lora_conv_dim, lora_conv_alpha):
+        """
+        Validates kohya lora by checking its parameters.
+        """
+        lora_type = None
 
-                    output_list = [f"{key}: {value}" for key, value in data_dict.items() if value is not None]
-                    
-                    del metadata
-                    return (True, f"LoRA Info: {output_list}")
-                elif lora_d8ahazard is not None:
-                    del metadata
-                    return (False, "LoRA Info: LoRA is not trained using 'kohya-ss/sd-scripts' but using 'd8ahazard/sd_dreambooth_extension'")
+        if 'lycoris.kohya' in lora_module:
+            if lora_algo:
+                if "locon" in lora_algo or "lora" in lora_algo:
+                    lora_type = "LoCon"
+                elif "loha" in lora_algo:
+                    lora_type = "LoHA"
+                elif "lokr" in lora_algo:
+                    lora_type = "LoKR"
+                elif "ia3" in lora_algo:
+                    lora_type = "IA3"
+                elif "dylora" in lora_algo:
+                    lora_type = "DyLoRA_LyCORIS"
+        elif 'networks.lora' in lora_module:
+            if lora_conv_dim is not None or lora_conv_alpha is not None:
+                lora_type = "LoRA_C3Lier"
             else:
-                del metadata
-                return (True, "LoRA Info: No metadata saved")
-        else:
-            return (True, "LoRA Info: No metadata saved, your model is not in safetensors format")
-    except Exception as e:
-        cprint(f"An error occurred: {str(e)}", color="green")
-
-def validate_kohya_lora(lora_module, lora_algo, lora_conv_dim, lora_conv_alpha):
-    lora_type = None
-
-    if 'lycoris.kohya' in lora_module:
-        if lora_algo:
-            if "locon" in lora_algo or "lora" in lora_algo:
-                lora_type = "LoCon"
-            elif "loha" in lora_algo:
-                lora_type = "LoHA"
-            elif "lokr" in lora_algo:
-                lora_type = "LoKR"
-            elif "ia3" in lora_algo:
-                lora_type = "IA3"
-            elif "dylora" in lora_algo:
-                lora_type = "DyLoRA_LyCORIS"
-    elif 'networks.lora' in lora_module:
-        if lora_conv_dim is not None or lora_conv_alpha is not None:
-            lora_type = "LoRA_C3Lier"
-        else:
-            lora_type = "LoRA_LierLa"
-    elif 'networks.dylora' in lora_module:
-        if lora_conv_dim is not None or lora_conv_alpha is not None:
-            lora_type = "DyLoRA_C3Lier"
+                lora_type = "LoRA_LierLa"
+        elif 'networks.dylora' in lora_module:
+            if lora_conv_dim is not None or lora_conv_alpha is not None:
+                lora_type = "DyLoRA_C3Lier"
+            else:
+                lora_type = "DyLoRA_LierLa"
         else:
-            lora_type = "DyLoRA_LierLa"
-    else:
-        lora_type = None
+            lora_type = None
 
-    return lora_type
+        return lora_type
```

### Comparing `colablib-0.1.5.dev4/colablib/py_utils.py` & `colablib-0.1.5.dev5/colablib/py_utils.py`

 * *Files identical despite different names*

