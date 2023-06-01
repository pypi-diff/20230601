# Comparing `tmp/cloud_radar-0.7.0.tar.gz` & `tmp/cloud_radar-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud_radar-0.7.0.tar", max compression
+gzip compressed data, was "cloud_radar-0.7.1.tar", max compression
```

## Comparing `cloud_radar-0.7.0.tar` & `cloud_radar-0.7.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2023-05-08 13:56:13.907853 cloud_radar-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0    12786 2023-05-08 13:56:13.907853 cloud_radar-0.7.0/README.md
--rw-r--r--   0        0        0     1431 2023-05-08 13:56:28.571994 cloud_radar-0.7.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-08 13:56:13.911853 cloud_radar-0.7.0/src/cloud_radar/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 13:56:13.911853 cloud_radar-0.7.0/src/cloud_radar/cf/__init__.py
--rw-r--r--   0        0        0       48 2023-05-08 13:56:13.911853 cloud_radar-0.7.0/src/cloud_radar/cf/e2e/__init__.py
--rw-r--r--   0        0        0     1677 2023-05-08 13:56:13.911853 cloud_radar-0.7.0/src/cloud_radar/cf/e2e/_stack.py
--rw-r--r--   0        0        0       57 2023-05-08 13:56:13.911853 cloud_radar-0.7.0/src/cloud_radar/cf/unit/__init__.py
--rw-r--r--   0        0        0      711 2023-05-08 13:56:13.911853 cloud_radar-0.7.0/src/cloud_radar/cf/unit/_condition.py
--rw-r--r--   0        0        0     1822 2023-05-08 13:56:13.911853 cloud_radar-0.7.0/src/cloud_radar/cf/unit/_output.py
--rw-r--r--   0        0        0     3199 2023-05-08 13:56:13.911853 cloud_radar-0.7.0/src/cloud_radar/cf/unit/_parameter.py
--rw-r--r--   0        0        0     3872 2023-05-08 13:56:13.911853 cloud_radar-0.7.0/src/cloud_radar/cf/unit/_resource.py
--rw-r--r--   0        0        0     5230 2023-05-08 13:56:13.911853 cloud_radar-0.7.0/src/cloud_radar/cf/unit/_stack.py
--rw-r--r--   0        0        0     9167 2023-05-08 13:56:13.911853 cloud_radar-0.7.0/src/cloud_radar/cf/unit/_template.py
--rw-r--r--   0        0        0    24791 2023-05-08 13:56:13.911853 cloud_radar-0.7.0/src/cloud_radar/cf/unit/functions.py
--rw-r--r--   0        0        0    13986 1970-01-01 00:00:00.000000 cloud_radar-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-01 13:36:09.488122 cloud_radar-0.7.1/LICENSE.txt
+-rw-r--r--   0        0        0    12370 2023-06-01 13:36:09.488122 cloud_radar-0.7.1/README.md
+-rw-r--r--   0        0        0     1433 2023-06-01 13:36:24.944476 cloud_radar-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-01 13:36:09.488122 cloud_radar-0.7.1/src/cloud_radar/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 13:36:09.488122 cloud_radar-0.7.1/src/cloud_radar/cf/__init__.py
+-rw-r--r--   0        0        0       48 2023-06-01 13:36:09.488122 cloud_radar-0.7.1/src/cloud_radar/cf/e2e/__init__.py
+-rw-r--r--   0        0        0     1677 2023-06-01 13:36:09.488122 cloud_radar-0.7.1/src/cloud_radar/cf/e2e/_stack.py
+-rw-r--r--   0        0        0       57 2023-06-01 13:36:09.488122 cloud_radar-0.7.1/src/cloud_radar/cf/unit/__init__.py
+-rw-r--r--   0        0        0      711 2023-06-01 13:36:09.488122 cloud_radar-0.7.1/src/cloud_radar/cf/unit/_condition.py
+-rw-r--r--   0        0        0     1822 2023-06-01 13:36:09.488122 cloud_radar-0.7.1/src/cloud_radar/cf/unit/_output.py
+-rw-r--r--   0        0        0     3199 2023-06-01 13:36:09.488122 cloud_radar-0.7.1/src/cloud_radar/cf/unit/_parameter.py
+-rw-r--r--   0        0        0     3872 2023-06-01 13:36:09.488122 cloud_radar-0.7.1/src/cloud_radar/cf/unit/_resource.py
+-rw-r--r--   0        0        0     5230 2023-06-01 13:36:09.488122 cloud_radar-0.7.1/src/cloud_radar/cf/unit/_stack.py
+-rw-r--r--   0        0        0    11587 2023-06-01 13:36:09.488122 cloud_radar-0.7.1/src/cloud_radar/cf/unit/_template.py
+-rw-r--r--   0        0        0    24791 2023-06-01 13:36:09.488122 cloud_radar-0.7.1/src/cloud_radar/cf/unit/functions.py
+-rw-r--r--   0        0        0    13524 1970-01-01 00:00:00.000000 cloud_radar-0.7.1/PKG-INFO
```

### Comparing `cloud_radar-0.7.0/LICENSE.txt` & `cloud_radar-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.7.0/README.md` & `cloud_radar-0.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -258,29 +258,23 @@
 A real functional testing example using Pytest can be seen [here](./tests/test_cf/test_examples/test_functional.py)
 
 </details>
 
 ## Roadmap
 
 ### Project
-- Python 3.7 support
-- Add Logging
 - Add Logo
-- Make it easier to interact with stack resources.
-  * Getting a resource for testing should be as easy as `stack.Resources('MyResource)` or `template.Resources('MyResource')`
 - Easier to pick regions for testing
 
 ### Unit
 - Add full functionality to pseudo variables.
   * Variables like `Partition`, `URLSuffix` should change if the region changes.
   * Variables like `StackName` and `StackId` should have a better default than ""
 - Handle References to resources that shouldn't exist.
   * It's currently possible that a `!Ref` to a Resource stays in the final template even if that resource is later removed because of a conditional.
-- Handle function order
-  * Some functions are only allowed in [certain parts](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/intrinsic-function-reference-conditions.html) of the template.
 
 ### Functional
 - Add the ability to update a stack instance to Taskcat.
 
 See the [open issues](https://github.com/DontShaveTheYak/cloud-radar/issues) for a list of proposed features (and known issues).
 
 ## Contributing
```

### Comparing `cloud_radar-0.7.0/pyproject.toml` & `cloud_radar-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cloud-radar"
-version = "0.7.0"
+version = "0.7.1"
 description = "Run functional tests on cloudformation stacks."
 readme = "README.md"
 authors = ["Levi Blaney <shadycuz@gmail.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/DontShaveTheYak/cloud-radar"
 keywords = ["aws", "cloudformation", "cloud-radar", "testing", "taskcat", "cloud", "radar"]
 classifiers = [
@@ -15,25 +15,25 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Topic :: Software Development :: Libraries",
   "Topic :: Software Development :: Testing"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.8.1"
 taskcat = "^0.9.20"
 cfn-flip = "^1.2.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0.0"
 coverage = {extras = ["toml"], version = "^7.0.0"}
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.6.1"
 black = "^23.0.0"
-flake8 = "^5.0.0"
+flake8 = "^6.0.0"
 flake8-black = "^0.3.0"
 flake8-import-order = "^0.18.1"
 flake8-bugbear = "^23.0.0"
 mypy = "^1.0.0"
 types-requests = "^2.28.11"
 types-PyYAML = "^6.0.12"
```

### Comparing `cloud_radar-0.7.0/src/cloud_radar/cf/e2e/_stack.py` & `cloud_radar-0.7.1/src/cloud_radar/cf/e2e/_stack.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.7.0/src/cloud_radar/cf/unit/_condition.py` & `cloud_radar-0.7.1/src/cloud_radar/cf/unit/_condition.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.7.0/src/cloud_radar/cf/unit/_output.py` & `cloud_radar-0.7.1/src/cloud_radar/cf/unit/_output.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.7.0/src/cloud_radar/cf/unit/_parameter.py` & `cloud_radar-0.7.1/src/cloud_radar/cf/unit/_parameter.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.7.0/src/cloud_radar/cf/unit/_resource.py` & `cloud_radar-0.7.1/src/cloud_radar/cf/unit/_resource.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.7.0/src/cloud_radar/cf/unit/_stack.py` & `cloud_radar-0.7.1/src/cloud_radar/cf/unit/_stack.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.7.0/src/cloud_radar/cf/unit/_template.py` & `cloud_radar-0.7.1/src/cloud_radar/cf/unit/_template.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 from pathlib import Path
-from typing import Any, Callable, Dict, Optional, Union
+from typing import Any, Callable, Dict, Generator, Optional, Tuple, Union
 
-from cfn_tools import dump_yaml, load_yaml  # type: ignore
-
-import yaml
+import yaml  # noqa: I100
+from cfn_tools import dump_yaml, load_yaml  # type: ignore  # noqa: I100, I201
 
 from . import functions
 from ._stack import Stack
 
 IntrinsicFunc = Callable[["Template", Any], Any]
 
 
@@ -104,31 +103,75 @@
             self.Region = region
 
         self.template = yaml.load(self.raw, Loader=yaml.FullLoader)
         self.set_parameters(params)
 
         add_metadata(self.template, self.Region)
 
-        self.resolve_values(
-            self.template,
-            functions.ALL_FUNCTIONS,
-        )
-
-        resources = self.template["Resources"]
-        for r_name, r_value in list(resources.items()):
-            if "Condition" not in r_value:
+        self.template = self.render_all_sections(self.template)
+
+        self.template = self.remove_condtional_resources(self.template)
+
+        return self.template
+
+    def render_all_sections(self, template: Dict[str, Any]) -> Dict[str, Any]:
+        """Solves all conditionals, references and pseudo variables for all sections"""
+        if "Conditions" in template:
+            template["Conditions"] = self.resolve_values(
+                template["Conditions"],
+                functions.ALL_FUNCTIONS,
+            )
+
+        template_sections = ["Resources", "Outputs"]
+
+        for section in template_sections:
+            if section not in template:
                 continue
 
-            keep_resource = r_value["Condition"]
+            for r_name, r_value in get_section_items(template, section):
+                if is_conditional(r_value):
+                    condition_value = get_condition_value(
+                        r_value["Condition"], template["Conditions"]
+                    )
+
+                    if not condition_value:
+                        continue
+
+                template[section][r_name] = self.resolve_values(
+                    r_value,
+                    functions.ALL_FUNCTIONS,
+                )
+
+        return template
 
-            if not keep_resource:
-                del self.template["Resources"][r_name]
+    def remove_condtional_resources(self, template: Dict[str, Any]) -> Dict[str, Any]:
+        """Removes all resources that have a condition that evaluates to False."""
+
+        # These are sections that can have conditional resources
+        conditional_sections = ["Resources", "Outputs"]
+
+        for section in conditional_sections:
+            if section not in template:
                 continue
 
-        return self.template
+            resources = template[section]
+
+            for r_name, r_value in list(resources.items()):
+                if not is_conditional(r_value):
+                    continue
+
+                condition_value = get_condition_value(
+                    r_value["Condition"], template["Conditions"]
+                )
+
+                if not condition_value:
+                    del template[section][r_name]
+                    continue
+
+        return template
 
     def create_stack(
         self, params: Optional[Dict[str, str]] = None, region: Optional[str] = None
     ):
         if region:
             self.Region = region
 
@@ -167,15 +210,15 @@
                     )
                     continue
 
                 # Takes care of the tricky 'Condition' key
                 if key == "Condition":
                     # This takes care of conditional resources
                     if "Properties" in data:
-                        data[key] = functions.condition(self, value)
+                        # data[key] = functions.condition(self, value)
                         continue
 
                     # If it's an intrinsic func
                     if is_condition_func(value):
                         return functions.condition(self, value)
 
                     # Normal key like in an IAM role
@@ -278,7 +321,36 @@
     Returns:
         bool: True if we think this `Condition` key is an instrinsic function.
     """
     if isinstance(value, str):
         return True
 
     return False
+
+
+# Loop through a dictionary yielding the key and value
+def iter_dict(data: dict) -> Generator[Tuple[str, Any], None, None]:
+    for key, value in data.items():
+        yield key, value
+
+
+# return iter_dict for a given key in a dictionary
+def get_section_items(
+    data: dict, section: str
+) -> Generator[Tuple[str, Any], None, None]:
+    if section not in data:
+        return iter_dict({})
+
+    return iter_dict(data[section])
+
+
+# Check if a dictionary has a key "Condition"
+def is_conditional(data: dict) -> bool:
+    if "Condition" in data:
+        return True
+
+    return False
+
+
+# Return the conditional value of a resouce
+def get_condition_value(condition_name: str, conditions: Dict[str, bool]) -> bool:
+    return conditions[condition_name]
```

### Comparing `cloud_radar-0.7.0/src/cloud_radar/cf/unit/functions.py` & `cloud_radar-0.7.1/src/cloud_radar/cf/unit/functions.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.7.0/PKG-INFO` & `cloud_radar-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: cloud-radar
-Version: 0.7.0
+Version: 0.7.1
 Summary: Run functional tests on cloudformation stacks.
 Home-page: https://github.com/DontShaveTheYak/cloud-radar
 License: Apache-2.0
 Keywords: aws,cloudformation,cloud-radar,testing,taskcat,cloud,radar
 Author: Levi Blaney
 Author-email: shadycuz@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
@@ -286,29 +285,23 @@
 A real functional testing example using Pytest can be seen [here](./tests/test_cf/test_examples/test_functional.py)
 
 </details>
 
 ## Roadmap
 
 ### Project
-- Python 3.7 support
-- Add Logging
 - Add Logo
-- Make it easier to interact with stack resources.
-  * Getting a resource for testing should be as easy as `stack.Resources('MyResource)` or `template.Resources('MyResource')`
 - Easier to pick regions for testing
 
 ### Unit
 - Add full functionality to pseudo variables.
   * Variables like `Partition`, `URLSuffix` should change if the region changes.
   * Variables like `StackName` and `StackId` should have a better default than ""
 - Handle References to resources that shouldn't exist.
   * It's currently possible that a `!Ref` to a Resource stays in the final template even if that resource is later removed because of a conditional.
-- Handle function order
-  * Some functions are only allowed in [certain parts](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/intrinsic-function-reference-conditions.html) of the template.
 
 ### Functional
 - Add the ability to update a stack instance to Taskcat.
 
 See the [open issues](https://github.com/DontShaveTheYak/cloud-radar/issues) for a list of proposed features (and known issues).
 
 ## Contributing
```

#### html2text {}

```diff
@@ -1,26 +1,25 @@
-Metadata-Version: 2.1 Name: cloud-radar Version: 0.7.0 Summary: Run functional
+Metadata-Version: 2.1 Name: cloud-radar Version: 0.7.1 Summary: Run functional
 tests on cloudformation stacks. Home-page: https://github.com/DontShaveTheYak/
 cloud-radar License: Apache-2.0 Keywords: aws,cloudformation,cloud-
 radar,testing,taskcat,cloud,radar Author: Levi Blaney Author-email:
-shadycuz@gmail.com Requires-Python: >=3.8,<4.0 Classifier: Development Status
-:: 2 - Pre-Alpha Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic ::
-Software Development :: Libraries Classifier: Topic :: Software Development ::
-Testing Requires-Dist: cfn-flip (>=1.2.3,<2.0.0) Requires-Dist: taskcat
-(>=0.9.20,<0.10.0) Project-URL: Repository, https://github.com/DontShaveTheYak/
-cloud-radar Description-Content-Type: text/markdown   [![Python][python-
-shield]][pypi-url] [![Latest][version-shield]][pypi-url] [![Tests][test-
-shield]][test-url] [![Coverage][codecov-shield]][codecov-url] [![License]
-[license-shield]][license-url]
+shadycuz@gmail.com Requires-Python: >=3.8.1,<4.0.0 Classifier: Development
+Status :: 2 - Pre-Alpha Classifier: License :: OSI Approved :: Apache Software
+License Classifier: Operating System :: OS Independent Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Topic :: Software Development ::
+Libraries Classifier: Topic :: Software Development :: Testing Requires-Dist:
+cfn-flip (>=1.2.3,<2.0.0) Requires-Dist: taskcat (>=0.9.20,<0.10.0) Project-
+URL: Repository, https://github.com/DontShaveTheYak/cloud-radar Description-
+Content-Type: text/markdown   [![Python][python-shield]][pypi-url] [![Latest]
+[version-shield]][pypi-url] [![Tests][test-shield]][test-url] [![Coverage]
+[codecov-shield]][codecov-url] [![License][license-shield]][license-url]
                              **** Cloud-Radar ****
            Write unit and functional tests for AWS Cloudformation.
                      Report_Bug Â· Request_Feature Â· Guide
   Table of Contents
    1. About_The_Project
           o Built_With
    2. Getting_Started
@@ -104,37 +103,32 @@
 template_path = Path("tests/templates/log_bucket/log_bucket.yaml") cls.test =
 Stack(template_path) cls.test.create() @classmethod def tearDownClass(cls):
 cls.test.delete() def test_bucket(self): stacks = self.__class__.test.stacks
 for stack in stacks: # Test ``` All the properties and methods of a [stack
 instance](https://github.com/aws-quickstart/taskcat/blob/main/taskcat/_cfn/
 stack.py#L188). A real functional testing example using Pytest can be seen
 [here](./tests/test_cf/test_examples/test_functional.py)  ## Roadmap ###
-Project - Python 3.7 support - Add Logging - Add Logo - Make it easier to
-interact with stack resources. * Getting a resource for testing should be as
-easy as `stack.Resources('MyResource)` or `template.Resources('MyResource')` -
-Easier to pick regions for testing ### Unit - Add full functionality to pseudo
-variables. * Variables like `Partition`, `URLSuffix` should change if the
-region changes. * Variables like `StackName` and `StackId` should have a better
-default than "" - Handle References to resources that shouldn't exist. * It's
-currently possible that a `!Ref` to a Resource stays in the final template even
-if that resource is later removed because of a conditional. - Handle function
-order * Some functions are only allowed in [certain parts](https://
-docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/intrinsic-function-
-reference-conditions.html) of the template. ### Functional - Add the ability to
-update a stack instance to Taskcat. See the [open issues](https://github.com/
-DontShaveTheYak/cloud-radar/issues) for a list of proposed features (and known
-issues). ## Contributing Contributions are what make the open-source community
-such an amazing place to learn, inspire, and create. Any contributions you make
-are **greatly appreciated**. This project uses poetry to manage dependencies
-and pre-commit to run formatting, linting and tests. You will need to have both
-installed to your system as well as python 3.9. 1. Fork the Project 2. Setup
-environment (`poetry install`) 3. Setup commit hooks (`pre-commit install`) 2.
-Create your Feature Branch (`git checkout -b feature/AmazingFeature`) 3. Commit
-your Changes (`git commit -m 'Add some AmazingFeature'`) 4. Push to the Branch
-(`git push origin feature/AmazingFeature`) 5. Open a Pull Request ## License
+Project - Add Logo - Easier to pick regions for testing ### Unit - Add full
+functionality to pseudo variables. * Variables like `Partition`, `URLSuffix`
+should change if the region changes. * Variables like `StackName` and `StackId`
+should have a better default than "" - Handle References to resources that
+shouldn't exist. * It's currently possible that a `!Ref` to a Resource stays in
+the final template even if that resource is later removed because of a
+conditional. ### Functional - Add the ability to update a stack instance to
+Taskcat. See the [open issues](https://github.com/DontShaveTheYak/cloud-radar/
+issues) for a list of proposed features (and known issues). ## Contributing
+Contributions are what make the open-source community such an amazing place to
+learn, inspire, and create. Any contributions you make are **greatly
+appreciated**. This project uses poetry to manage dependencies and pre-commit
+to run formatting, linting and tests. You will need to have both installed to
+your system as well as python 3.9. 1. Fork the Project 2. Setup environment
+(`poetry install`) 3. Setup commit hooks (`pre-commit install`) 2. Create your
+Feature Branch (`git checkout -b feature/AmazingFeature`) 3. Commit your
+Changes (`git commit -m 'Add some AmazingFeature'`) 4. Push to the Branch (`git
+push origin feature/AmazingFeature`) 5. Open a Pull Request ## License
 Distributed under the Apache-2.0 License. See [LICENSE.txt](./LICENSE.txt) for
 more information. ## Contact Levi - [@shady_cuz](https://twitter.com/shady_cuz)
 ## Acknowledgements * [Taskcat](https://aws-quickstart.github.io/taskcat/) *
 [Hypermodern Python](https://cjolowicz.github.io/posts/hypermodern-python-01-
 setup/) * [Best-README-Template](https://github.com/othneildrew/Best-README-
 Template)   [python-shield]: https://img.shields.io/pypi/pyversions/cloud-
 radar?style=for-the-badge [version-shield]: https://img.shields.io/pypi/v/
```

