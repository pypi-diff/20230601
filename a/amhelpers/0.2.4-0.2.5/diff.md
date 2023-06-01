# Comparing `tmp/amhelpers-0.2.4.tar.gz` & `tmp/amhelpers-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amhelpers-0.2.4.tar", max compression
+gzip compressed data, was "amhelpers-0.2.5.tar", max compression
```

## Comparing `amhelpers-0.2.4.tar` & `amhelpers-0.2.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0     1072 2022-05-30 13:43:08.846346 amhelpers-0.2.4/LICENSE
--rw-r--r--   0        0        0      405 2022-05-30 13:43:55.780186 amhelpers-0.2.4/README.md
--rw-r--r--   0        0        0      588 2022-07-07 16:07:10.845028 amhelpers-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      111 2022-05-30 13:43:08.893968 amhelpers-0.2.4/src/amhelpers/__init__.py
--rw-r--r--   0        0        0     1936 2022-05-30 14:19:11.627209 amhelpers-0.2.4/src/amhelpers/amhelpers.py
--rw-r--r--   0        0        0     3605 2022-07-07 15:52:41.512674 amhelpers-0.2.4/src/amhelpers/config_parsing.py
--rw-r--r--   0        0        0      990 2022-07-07 16:13:36.092598 amhelpers-0.2.4/setup.py
--rw-r--r--   0        0        0      850 2022-07-07 16:13:36.092834 amhelpers-0.2.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2022-05-30 13:43:08.846346 amhelpers-0.2.5/LICENSE
+-rw-r--r--   0        0        0      405 2022-05-30 13:43:55.780186 amhelpers-0.2.5/README.md
+-rw-r--r--   0        0        0      588 2023-06-01 08:34:26.725673 amhelpers-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      111 2022-05-30 13:43:08.893968 amhelpers-0.2.5/src/amhelpers/__init__.py
+-rw-r--r--   0        0        0     1936 2022-05-30 14:19:11.627209 amhelpers-0.2.5/src/amhelpers/amhelpers.py
+-rw-r--r--   0        0        0     4236 2023-06-01 08:25:43.146994 amhelpers-0.2.5/src/amhelpers/config_parsing.py
+-rw-r--r--   0        0        0      990 2023-06-01 08:36:37.080238 amhelpers-0.2.5/setup.py
+-rw-r--r--   0        0        0      850 2023-06-01 08:36:37.080545 amhelpers-0.2.5/PKG-INFO
```

### Comparing `amhelpers-0.2.4/LICENSE` & `amhelpers-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `amhelpers-0.2.4/pyproject.toml` & `amhelpers-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "amhelpers"
-version = "0.2.4"
+version = "0.2.5"
 description = "A collection of handy utilities."
 authors = ["Anton Matsson"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
```

### Comparing `amhelpers-0.2.4/src/amhelpers/amhelpers.py` & `amhelpers-0.2.5/src/amhelpers/amhelpers.py`

 * *Files identical despite different names*

### Comparing `amhelpers-0.2.4/src/amhelpers/config_parsing.py` & `amhelpers-0.2.5/src/amhelpers/config_parsing.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,15 +29,23 @@
         return value
     elif isinstance(value, list):
         return [_check_value(v) for v in value]
     elif isinstance(value, dict):
         if 'type' in value:
             is_called = value.pop('is_called')
             if is_called:
-                return create_object_from_dict(value)
+                has_nested_dict = any(
+                    [isinstance(v, dict) and 'type' in v for v in value.values()]
+                )
+                if has_nested_dict:
+                    return create_object_from_dict(
+                        {k: _check_value(v) for k, v in value.items()}
+                    )
+                else:
+                    return create_object_from_dict(value)
             else:
                 type_str = value['type']
                 return get_class_from_str(type_str)
         else:
             return {k: _check_value(v) for k, v in value.items()}
     elif value is None:
         return value
@@ -47,25 +55,32 @@
 def _get_object_and_parameters(name, default_params, specified_params):
     default_params.pop('is_called', None)
     specified_params.pop('is_called', None)
 
     prefix = name + '__'
 
     if 'type' in specified_params:
-        # Take everything from "specified"
+        # Take everything from specified_params
         out = {name: get_class_from_str(specified_params.pop('type'))}
         out.update(
             {prefix+k: _check_value(v) for k, v in specified_params.items()}
         )
     elif 'type' in default_params:
-        # Replace default values if they exist in "specified"
+        # Replace default values if they exist in specified_params
         out = {name: get_class_from_str(default_params.pop('type'))}
-        out.update(
-            {prefix+k: _check_value(specified_params[k]) if k in specified_params else _check_value(default_params[k]) for k in default_params.keys()}
-        )
+        new = {}
+        for k in default_params.keys():
+            if k in specified_params:
+                v = specified_params.pop(k)
+                new[prefix+k] = _check_value(v)
+            else:
+                new[prefix+k] = _check_value(default_params[k])
+        out.update(new)
+        # Add values that exist in specified_params but not in default_params
+        out.update({prefix+k: _check_value(v) for k, v in specified_params.items()})
     else:
         out = {}
         for k in set(list(default_params.keys()) + list(specified_params.keys())):
             out[prefix+k] = _check_value(specified_params[k]) if k in specified_params else _check_value(default_params[k])
 
     return out
```

### Comparing `amhelpers-0.2.4/setup.py` & `amhelpers-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ['amhelpers']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'amhelpers',
-    'version': '0.2.4',
+    'version': '0.2.5',
     'description': 'A collection of handy utilities.',
     'long_description': '# amhelpers\n\nA collection of handy utilities.\n\n## Installation\n\n```bash\n$ pip install amhelpers\n```\n\n## License\n\n`amhelpers` was created by Anton Matsson. It is licensed under the terms of the MIT license.\n\n## Credits\n\n`amhelpers` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Anton Matsson',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `amhelpers-0.2.4/PKG-INFO` & `amhelpers-0.2.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amhelpers
-Version: 0.2.4
+Version: 0.2.5
 Summary: A collection of handy utilities.
 License: MIT
 Author: Anton Matsson
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

