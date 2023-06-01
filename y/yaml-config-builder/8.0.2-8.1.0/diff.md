# Comparing `tmp/yaml_config_builder-8.0.2.tar.gz` & `tmp/yaml_config_builder-8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaml_config_builder-8.0.2.tar", max compression
+gzip compressed data, was "yaml_config_builder-8.1.0.tar", max compression
```

## Comparing `yaml_config_builder-8.0.2.tar` & `yaml_config_builder-8.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11412 2023-05-25 13:19:06.793465 yaml_config_builder-8.0.2/LICENSE
--rw-r--r--   0        0        0      950 2023-05-25 13:19:06.793465 yaml_config_builder-8.0.2/README.md
--rw-r--r--   0        0        0     2739 2023-05-25 13:19:06.797466 yaml_config_builder-8.0.2/pyproject.toml
--rw-r--r--   0        0        0      452 2023-05-25 14:08:10.333408 yaml_config_builder-8.0.2/src/config_builder/__init__.py
--rw-r--r--   0        0        0    17679 2023-05-25 13:19:06.797466 yaml_config_builder-8.0.2/src/config_builder/base_config_class.py
--rw-r--r--   0        0        0    13656 2023-05-25 14:08:10.333408 yaml_config_builder-8.0.2/src/config_builder/config_builder.py
--rw-r--r--   0        0        0        0 2023-05-25 13:19:06.797466 yaml_config_builder-8.0.2/src/config_builder/py.typed
--rw-r--r--   0        0        0     3913 2023-05-25 13:19:06.797466 yaml_config_builder-8.0.2/src/config_builder/replacement_map.py
--rw-r--r--   0        0        0     2684 2023-05-25 13:19:06.797466 yaml_config_builder-8.0.2/src/config_builder/utils.py
--rw-r--r--   0        0        0    10568 2023-05-25 13:19:06.797466 yaml_config_builder-8.0.2/src/config_builder/yaml_constructors.py
--rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 yaml_config_builder-8.0.2/setup.py
--rw-r--r--   0        0        0     2305 1970-01-01 00:00:00.000000 yaml_config_builder-8.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11412 2023-05-31 14:39:43.205875 yaml_config_builder-8.1.0/LICENSE
+-rw-r--r--   0        0        0      950 2023-05-31 14:39:43.205875 yaml_config_builder-8.1.0/README.md
+-rw-r--r--   0        0        0     2739 2023-06-01 09:28:31.630154 yaml_config_builder-8.1.0/pyproject.toml
+-rw-r--r--   0        0        0      452 2023-06-01 09:28:10.625382 yaml_config_builder-8.1.0/src/config_builder/__init__.py
+-rw-r--r--   0        0        0    18716 2023-05-31 14:39:43.209875 yaml_config_builder-8.1.0/src/config_builder/base_config_class.py
+-rw-r--r--   0        0        0    13656 2023-05-31 14:39:43.209875 yaml_config_builder-8.1.0/src/config_builder/config_builder.py
+-rw-r--r--   0        0        0        0 2023-05-31 14:39:43.209875 yaml_config_builder-8.1.0/src/config_builder/py.typed
+-rw-r--r--   0        0        0     3913 2023-05-31 14:39:43.209875 yaml_config_builder-8.1.0/src/config_builder/replacement_map.py
+-rw-r--r--   0        0        0     2684 2023-05-31 14:39:43.209875 yaml_config_builder-8.1.0/src/config_builder/utils.py
+-rw-r--r--   0        0        0    10568 2023-05-31 14:39:43.209875 yaml_config_builder-8.1.0/src/config_builder/yaml_constructors.py
+-rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 yaml_config_builder-8.1.0/setup.py
+-rw-r--r--   0        0        0     2305 1970-01-01 00:00:00.000000 yaml_config_builder-8.1.0/PKG-INFO
```

### Comparing `yaml_config_builder-8.0.2/LICENSE` & `yaml_config_builder-8.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yaml_config_builder-8.0.2/README.md` & `yaml_config_builder-8.1.0/README.md`

 * *Files identical despite different names*

### Comparing `yaml_config_builder-8.0.2/pyproject.toml` & `yaml_config_builder-8.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "yaml-config-builder"
 description = "Yaml-Config-Builder: SDK for building configuration classes on the basis of given content from YAML configuration files"
-version = "8.0.2"
+version = "8.1.0"
 license = "Open Logistics Foundation License 1.3"
 readme = "README.md"
 homepage = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/config-builder"
 repository = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/config-builder"
 documentation = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/config-builder/-/blob/main/documentation/index.adoc"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `yaml_config_builder-8.0.2/src/config_builder/base_config_class.py` & `yaml_config_builder-8.1.0/src/config_builder/base_config_class.py`

 * *Files 3% similar despite different names*

```diff
@@ -271,14 +271,24 @@
         setattr(self, class_name, new_list)
 
     def _replace_strings_in_attribute_dict(
         self,
         class_name: str,
         class_attribute: Dict[str, Any],
     ) -> None:
+        new_dict = self.__replace_strings_in_attribute_dict_step(
+            class_name, class_attribute
+        )
+        setattr(self, class_name, new_dict)
+
+    @staticmethod
+    def __replace_strings_in_attribute_dict_step(
+        class_name: str,
+        class_attribute: Dict[str, Any],
+    ) -> Dict[str, Any]:
         """
         Same as the method '_replace_string_in_attribute', but runs the replacement
         check on a list of string-attributes
 
         Args:
             class_name: Name of this dictionary attribute
             class_attribute: Value of this dictionary attribute
@@ -309,45 +319,57 @@
                         )
                         new_dict[class_attribute_key] = replace_directory_in_path(
                             file_path=new_dict[class_attribute_key],
                             replacement_key=key,
                             replacement_value=value,
                         )
 
-            elif isinstance(new_dict[class_attribute_key], list) and check_list_type(
-                obj=cast(List[str], new_dict[class_attribute_key]), obj_type=str
-            ):
+            elif isinstance(new_dict[class_attribute_key], list):
                 for list_index, list_element in enumerate(
                     new_dict[class_attribute_key]
                 ):
-                    new_list_element = list_element
+                    if isinstance(list_element, str):
+                        new_list_element = list_element
 
-                    for key, value in get_current_replacement_map().items():
-                        # Don't run replacements with empty string
-                        if value == "":
-                            continue
-
-                        # Replace the occurrence of the value in the class attribute, if it is
-                        # a directory
-                        if key in list_element:
-                            logger.debug(
-                                f"Replace '{key}' "
-                                f"in dict list entry {list_element} "
-                                f"of {class_name} "
-                                f"with '{value}'"
-                            )
-                            new_list_element = replace_directory_in_path(
-                                file_path=list_element,
-                                replacement_key=key,
-                                replacement_value=value,
-                            )
-
-                    new_dict[class_attribute_key][list_index] = new_list_element
+                        for key, value in get_current_replacement_map().items():
+                            # Don't run replacements with empty string
+                            if value == "":
+                                continue
+
+                            # Replace the occurrence of the value in the class attribute, if it is
+                            # a directory
+                            if key in list_element:
+                                logger.debug(
+                                    f"Replace '{key}' "
+                                    f"in dict list entry {list_element} "
+                                    f"of {class_name} "
+                                    f"with '{value}'"
+                                )
+                                new_list_element = replace_directory_in_path(
+                                    file_path=list_element,
+                                    replacement_key=key,
+                                    replacement_value=value,
+                                )
+                        new_dict[class_attribute_key][list_index] = new_list_element
+                    elif isinstance(list_element, dict):
+                        new_dict[class_attribute_key][
+                            list_index
+                        ] = BaseConfigClass.__replace_strings_in_attribute_dict_step(
+                            class_name=class_attribute_key,
+                            class_attribute=list_element,
+                        )
+            elif isinstance(new_dict[class_attribute_key], dict):
+                new_dict[
+                    class_attribute_key
+                ] = BaseConfigClass.__replace_strings_in_attribute_dict_step(
+                    class_name=class_attribute_key,
+                    class_attribute=class_attribute_value,
+                )
 
-        setattr(self, class_name, new_dict)
+        return new_dict
 
     def check_values(self) -> bool:
         """
         Placeholder method that is intended to be used to check any attribute
         for correct values.
 
         Returns:
```

### Comparing `yaml_config_builder-8.0.2/src/config_builder/config_builder.py` & `yaml_config_builder-8.1.0/src/config_builder/config_builder.py`

 * *Files identical despite different names*

### Comparing `yaml_config_builder-8.0.2/src/config_builder/replacement_map.py` & `yaml_config_builder-8.1.0/src/config_builder/replacement_map.py`

 * *Files identical despite different names*

### Comparing `yaml_config_builder-8.0.2/src/config_builder/utils.py` & `yaml_config_builder-8.1.0/src/config_builder/utils.py`

 * *Files identical despite different names*

### Comparing `yaml_config_builder-8.0.2/src/config_builder/yaml_constructors.py` & `yaml_config_builder-8.1.0/src/config_builder/yaml_constructors.py`

 * *Files identical despite different names*

### Comparing `yaml_config_builder-8.0.2/setup.py` & `yaml_config_builder-8.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'attrs>=20',
  'future>0.18',
  'python-dateutil>2.8',
  'related-mltoolbox>=1.0.1,<2']
 
 setup_kwargs = {
     'name': 'yaml-config-builder',
-    'version': '8.0.2',
+    'version': '8.1.0',
     'description': 'Yaml-Config-Builder: SDK for building configuration classes on the basis of given content from YAML configuration files',
     'long_description': '# Config Builder\n\nThe ConfigBuilder provides an SDK for building configuration classes on the basis of \ngiven content from YAML configuration files. Details about the ConfigBuilder can be\nfound in the [documentation](documentation/index.adoc).\n\n## Install\n\nThe installation and setup of the ConfigBuilder is described in [chapter 11](documentation/12_tutorial.adoc) \nof the documentation.\n\n# Technology stack\n\n- Python \n\n## License\nSee the license file in the top directory.\n\n## Contact information\n\n\nMaintainer: \n- Maximilian Otten <a href="mailto:maximilian.otten@iml.fraunhofer.de?">maximilian.otten@iml.fraunhofer.de</a>\n\nDevelopment Team: \n- Christian Hoppe <a href="mailto:christian.hoppe@iml.fraunhofer.de?">christian.hoppe@iml.fraunhofer.de</a>\n- Oliver Bredtmann <a href="mailto:oliver.bredtmann@dbschenker.com?">oliver.bredtmann@dbschenker.com</a>\n- Thilo Bauer <a href="mailto:thilo.bauer@dbschenker.com?">thilo.bauer@dbschenker.com</a>\n\n\n',
     'author': 'Maximilian Otten',
     'author_email': 'maximilian.otten@iml.fraunhofer.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/config-builder',
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['config_builder'] package_data = \ {'': ['*']}
 install_requires = \ ['PyYAML>5.4', 'attrs>=20', 'future>0.18', 'python-
 dateutil>2.8', 'related-mltoolbox>=1.0.1,<2'] setup_kwargs = { 'name': 'yaml-
-config-builder', 'version': '8.0.2', 'description': 'Yaml-Config-Builder: SDK
+config-builder', 'version': '8.1.0', 'description': 'Yaml-Config-Builder: SDK
 for building configuration classes on the basis of given content from YAML
 configuration files', 'long_description': '# Config Builder\n\nThe
 ConfigBuilder provides an SDK for building configuration classes on the basis
 of \ngiven content from YAML configuration files. Details about the
 ConfigBuilder can be\nfound in the [documentation](documentation/
 index.adoc).\n\n## Install\n\nThe installation and setup of the ConfigBuilder
 is described in [chapter 11](documentation/12_tutorial.adoc) \nof the
```

### Comparing `yaml_config_builder-8.0.2/PKG-INFO` & `yaml_config_builder-8.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-config-builder
-Version: 8.0.2
+Version: 8.1.0
 Summary: Yaml-Config-Builder: SDK for building configuration classes on the basis of given content from YAML configuration files
 Home-page: https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/config-builder
 License: Open Logistics Foundation License 1.3
 Author: Maximilian Otten
 Author-email: maximilian.otten@iml.fraunhofer.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yaml-config-builder Version: 8.0.2 Summary: Yaml-
+Metadata-Version: 2.1 Name: yaml-config-builder Version: 8.1.0 Summary: Yaml-
 Config-Builder: SDK for building configuration classes on the basis of given
 content from YAML configuration files Home-page: https://
 git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/config-builder
 License: Open Logistics Foundation License 1.3 Author: Maximilian Otten Author-
 email: maximilian.otten@iml.fraunhofer.de Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: Other/Proprietary License
```

