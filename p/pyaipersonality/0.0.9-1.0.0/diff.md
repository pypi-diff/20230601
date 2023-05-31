# Comparing `tmp/pyaipersonality-0.0.9.tar.gz` & `tmp/pyaipersonality-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaipersonality-0.0.9.tar", last modified: Sat May  6 19:24:28 2023, max compression
+gzip compressed data, was "pyaipersonality-1.0.0.tar", last modified: Wed May 31 23:51:22 2023, max compression
```

## Comparing `pyaipersonality-0.0.9.tar` & `pyaipersonality-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 19:24:28.451794 pyaipersonality-0.0.9/
--rw-rw-rw-   0        0        0    11558 2023-04-29 07:11:51.000000 pyaipersonality-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     9394 2023-05-06 19:24:28.451794 pyaipersonality-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     8901 2023-05-06 19:24:03.000000 pyaipersonality-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 19:24:28.437278 pyaipersonality-0.0.9/pyaipersonality/
--rw-rw-rw-   0        0        0     8636 2023-05-06 19:04:20.000000 pyaipersonality-0.0.9/pyaipersonality/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 19:24:28.450794 pyaipersonality-0.0.9/pyaipersonality.egg-info/
--rw-rw-rw-   0        0        0     9394 2023-05-06 19:24:28.000000 pyaipersonality-0.0.9/pyaipersonality.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-05-06 19:24:28.000000 pyaipersonality-0.0.9/pyaipersonality.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 19:24:28.000000 pyaipersonality-0.0.9/pyaipersonality.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-05-06 19:24:28.000000 pyaipersonality-0.0.9/pyaipersonality.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-06 19:24:28.000000 pyaipersonality-0.0.9/pyaipersonality.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 19:24:28.452796 pyaipersonality-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1075 2023-05-06 19:23:53.000000 pyaipersonality-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 23:51:22.746039 pyaipersonality-1.0.0/
+-rw-rw-rw-   0        0        0    11558 2023-04-29 07:11:51.000000 pyaipersonality-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0    14413 2023-05-31 23:51:22.746039 pyaipersonality-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    13920 2023-05-07 01:23:25.000000 pyaipersonality-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 23:51:22.731094 pyaipersonality-1.0.0/pyaipersonality/
+-rw-rw-rw-   0        0        0    31620 2023-05-31 22:07:47.000000 pyaipersonality-1.0.0/pyaipersonality/__init__.py
+-rw-rw-rw-   0        0        0     6626 2023-05-31 23:13:08.000000 pyaipersonality-1.0.0/pyaipersonality/binding.py
+-rw-rw-rw-   0        0        0     9357 2023-05-31 23:39:19.000000 pyaipersonality-1.0.0/pyaipersonality/langchain_integration.py
+-rw-rw-rw-   0        0        0     3852 2023-05-31 23:37:08.000000 pyaipersonality-1.0.0/pyaipersonality/server.py
+drwxrwxrwx   0        0        0        0 2023-05-31 23:51:22.745043 pyaipersonality-1.0.0/pyaipersonality.egg-info/
+-rw-rw-rw-   0        0        0    14413 2023-05-31 23:51:22.000000 pyaipersonality-1.0.0/pyaipersonality.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-05-31 23:51:22.000000 pyaipersonality-1.0.0/pyaipersonality.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 23:51:22.000000 pyaipersonality-1.0.0/pyaipersonality.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-05-31 23:51:22.000000 pyaipersonality-1.0.0/pyaipersonality.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-31 23:51:22.000000 pyaipersonality-1.0.0/pyaipersonality.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 23:51:22.746039 pyaipersonality-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1075 2023-05-31 23:48:18.000000 pyaipersonality-1.0.0/setup.py
```

### Comparing `pyaipersonality-0.0.9/LICENSE` & `pyaipersonality-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaipersonality-0.0.9/PKG-INFO` & `pyaipersonality-1.0.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaipersonality
-Version: 0.0.9
+Version: 1.0.0
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/PyAIPersonality
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -20,15 +20,15 @@
 ![GitHub forks](https://img.shields.io/github/forks/ParisNeo/PyAIPersonality)
 [![Discord](https://img.shields.io/discord/1092918764925882418?color=7289da&label=Discord&logo=discord&logoColor=ffffff)](https://discord.gg/4rR282WJb6)
 [![Follow me on Twitter](https://img.shields.io/twitter/follow/SpaceNerduino?style=social)](https://twitter.com/SpaceNerduino)
 [![Follow Me on YouTube](https://img.shields.io/badge/Follow%20Me%20on-YouTube-red?style=flat&logo=youtube)](https://www.youtube.com/user/Parisneo)
 
 [![PyPI](https://img.shields.io/pypi/v/pyaipersonality.svg)](https://pypi.org/project/pyaipersonality/)
 
-## Current version : 0.0.9 (GLaDOS)
+## Current version : 0.0.10 (GLaDOS)
 ## Main developer [ParisNeo](https://github.com/ParisNeo)
 
 PyAIPersonality is a Python library for defining AI personalities for AI-based models. With PyAIPersonality, you can define a file format, assets, and personalized scripts to create unique AI personalities.
 
 ## Installation
 
 You can install PyAIPersonality using pip:
@@ -115,39 +115,34 @@
             urllib.request.urlretrieve(url, folder_path / url.split("/")[-1], reporthook=report_progress)
             print("File downloaded successfully!")
         except Exception as e:
             print("Error downloading file:", e)
             sys.exit(1)
 
     personality = AIPersonality("personalities_zoo/english/generic/gpt4all")
-    full_context = personality.personality_conditioning+personality.link_text+personality.ai_message_prefix+personality.welcome_message if personality.welcome_message!="" else personality.personality_conditioning
-    model = Model(model_path=f'models/{url.split("/")[-1]}',
-                  prompt_context=full_context,
-                  prompt_prefix=personality.link_text + personality.user_message_prefix + personality.link_text,
-                  prompt_suffix=personality.link_text + personality.ai_message_prefix + personality.link_text
-                  )
+    model = Model(model_path=f'models/{url.split("/")[-1]}', n_ctx=2048)
     # If there is a disclaimer, show it
     if personality.disclaimer!="":
         print()
         print("Disclaimer")
         print(personality.disclaimer)
         print()
-
-    # Show conditionning
-    print(full_context)
     
+
+    full_discussion = personality.personality_conditioning+personality.ai_message_prefix+personality.welcome_message+personality.link_text
     while True:
         try:
             prompt = input("You: ")
+            full_discussion+=personality.ai_message_prefix+prompt
             if prompt == '':
                 continue
             print(f"{personality.name}:", end='')
             output=""
             for tok in model.generate(
-                            prompt, 
+                            full_discussion, 
                             n_predict=personality.model_n_predicts, 
                             temp=personality.model_temperature,
                             top_k=personality.model_top_k,
                             top_p=personality.model_top_p,
                             repeat_last_n=personality.model_repeat_last_n,
                             repeat_penalty=personality.model_repeat_penalty
                         ):
@@ -160,14 +155,15 @@
                     print(f"{tok}", end='', flush=True)
             print()
         except KeyboardInterrupt:
             print("Keyboard interrupt detected.\nBye")
             break
     print("Done")
     print(f"{personality}")
+
 ```
 
 # Naming Rationale
 For our new multi-personality AI agent library, we wanted to come up with a naming scheme that reflected our love for science fiction and artificial intelligence. Each release of the application will feature a different AI agent with a distinct personality and set of capabilities, so we felt it was important to give each version a unique and memorable name.
 
 # Current version name: GLaDOS
 GLaDOS is a fictional AI character from the popular video game series "Portal" developed by Valve Corporation. She serves as the primary antagonist throughout the series, with her primary function being the management of the Aperture Science Enrichment Center.
@@ -185,9 +181,150 @@
 2. Create a new branch (`git checkout -b my-new-branch`)
 3. Make your changes
 4. Commit your changes (`git commit -am 'Add some feature'`)
 5. Push to the branch (`git push origin my-new-branch`)
 6. Create a new pull request
 
 
+To build a new personality, you only need to have a config.yaml file with the following fields:
+
+- author
+    - YAML field: `author`
+    - Description: The author of the personality.
+
+- version
+    - YAML field: `version`
+    - Description: The version number of the personality.
+
+- personality_description
+    - YAML field: `personality_description`
+    - Description: A description of the personality, providing information about its characteristics and behavior.
+
+- disclaimer
+    - YAML field: `disclaimer`
+    - Description: A disclaimer or legal statement regarding the use of the personality and any associated liabilities.
+
+- language
+    - YAML field: `language`
+    - Description: The language code or identifier used by the personality (e.g., "en_US" for American English).
+
+- category
+    - YAML field: `category`
+    - Description: The category or type of the personality (e.g., "General", "Technical Support", "Entertainment").
+
+- name
+    - YAML field: `name`
+    - Description: The name or title of the personality.
+
+- user_name
+    - YAML field: `user_name`
+    - Description: The username or identifier associated with the user interacting with the personality.
+
+- personality_conditioning
+    - YAML field: `personality_conditioning`
+    - Description: Information or context about the personality, including its purpose, capabilities, and origin.
+
+- ai_message_prefix
+    - YAML field: `ai_message_prefix`
+    - Description: The prefix or tag used to identify messages generated by the AI assistant.
+
+- welcome_message
+    - YAML field: `welcome_message`
+    - Description: A welcoming message displayed when interacting with the personality.
+
+- link_text
+    - YAML field: `link_text`
+    - Description: Additional text or formatting used for line breaks or spacing in messages.
+
+- user_message_prefix
+    - YAML field: `user_message_prefix`
+    - Description: The prefix or tag used to identify messages generated by the user.
+
+- anti_prompts
+    - YAML field: `anti_prompts`
+    - Description: A list of strings or patterns that can be used to identify and exclude certain message types from prompts or inputs.
+
+- dependencies
+    - YAML field: `dependencies`
+    - Description: A list of dependencies or external resources required by the personality.
+
+- model_temperature
+    - YAML field: `model_temperature`
+    - Description: The temperature value controlling the randomness of the AI model's responses. Higher values result in more creative outputs.
+
+- model_n_predicts
+    - YAML field: `model_n_predicts`
+    - Description: The number of words or tokens to generate in each response from the AI model.
+
+- model_top_k
+    - YAML field: `model_top_k`
+    - Description: The value of K used in the top-K sampling algorithm, controlling the diversity of the generated responses.
+
+- model_top_p
+    - YAML field: `model_top_p`
+    - Description: The value of p used in the nucleus sampling algorithm, controlling the diversity of the generated responses.
+
+- model_repeat_penalty
+    - YAML field: `model_repeat_penalty`
+    - Description: The penalty factor applied to repeated words or phrases in the generated responses to encourage more varied outputs.
+
+- model_repeat_last_n
+    - YAML field: `model_repeat_last_n`
+    - Description: The number of previous tokens to consider when calculating the repetition penalty.
+
+# Information
+From v 0.0.11, we have added processors which allow your personality to have a spersonalized script that is applied on the use text or the ai output text.
+You must put the code inside a file called `processor.py` inside a subfolder called scripts.
+
+inside `processor.py` create a class that inherits from `from pyaipersonality import PAPScript`.
+
+Here is the current form of this class. it will have more elements in the future:
+Look at gpt4internetv0 and gpt4intervet examples for more information
+```python
+class PAPScript:
+    """
+    Template class for implementing personality processor classes in the PAPScript framework.
+
+    This class provides a basic structure and placeholder methods for processing model inputs and outputs.
+    Personality-specific processor classes should inherit from this class and override the necessary methods.
+
+    Methods:
+        process_model_input(text): Process the model input.
+        process_model_output(text): Process the model output.
+    """
+    def __init__(self) -> None:
+        pass
+
+    def process_model_input(self, text):
+        """
+        Process the model input.
+
+        This method should be overridden in the personality-specific processor class to define
+        the desired behavior for processing the model input.
+
+        Args:
+            text (str): The model input text.
+
+        Returns:
+            Any: The processed model input.
+        """
+        return None
+
+    def process_model_output(self, text):
+        """
+        Process the model output.
+
+        This method should be overridden in the personality-specific processor class to define
+        the desired behavior for processing the model output.
+
+        Args:
+            text (str): The model output text.
+
+        Returns:
+            Any: The processed model output.
+        """
+        return None
+
+```
+
 # License
 PyAIPersonality is licensed under the Apache 2.0 license. See the `LICENSE` file for more information.
```

### Comparing `pyaipersonality-0.0.9/pyaipersonality.egg-info/PKG-INFO` & `pyaipersonality-1.0.0/pyaipersonality.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaipersonality
-Version: 0.0.9
+Version: 1.0.0
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/PyAIPersonality
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -20,15 +20,15 @@
 ![GitHub forks](https://img.shields.io/github/forks/ParisNeo/PyAIPersonality)
 [![Discord](https://img.shields.io/discord/1092918764925882418?color=7289da&label=Discord&logo=discord&logoColor=ffffff)](https://discord.gg/4rR282WJb6)
 [![Follow me on Twitter](https://img.shields.io/twitter/follow/SpaceNerduino?style=social)](https://twitter.com/SpaceNerduino)
 [![Follow Me on YouTube](https://img.shields.io/badge/Follow%20Me%20on-YouTube-red?style=flat&logo=youtube)](https://www.youtube.com/user/Parisneo)
 
 [![PyPI](https://img.shields.io/pypi/v/pyaipersonality.svg)](https://pypi.org/project/pyaipersonality/)
 
-## Current version : 0.0.9 (GLaDOS)
+## Current version : 0.0.10 (GLaDOS)
 ## Main developer [ParisNeo](https://github.com/ParisNeo)
 
 PyAIPersonality is a Python library for defining AI personalities for AI-based models. With PyAIPersonality, you can define a file format, assets, and personalized scripts to create unique AI personalities.
 
 ## Installation
 
 You can install PyAIPersonality using pip:
@@ -115,39 +115,34 @@
             urllib.request.urlretrieve(url, folder_path / url.split("/")[-1], reporthook=report_progress)
             print("File downloaded successfully!")
         except Exception as e:
             print("Error downloading file:", e)
             sys.exit(1)
 
     personality = AIPersonality("personalities_zoo/english/generic/gpt4all")
-    full_context = personality.personality_conditioning+personality.link_text+personality.ai_message_prefix+personality.welcome_message if personality.welcome_message!="" else personality.personality_conditioning
-    model = Model(model_path=f'models/{url.split("/")[-1]}',
-                  prompt_context=full_context,
-                  prompt_prefix=personality.link_text + personality.user_message_prefix + personality.link_text,
-                  prompt_suffix=personality.link_text + personality.ai_message_prefix + personality.link_text
-                  )
+    model = Model(model_path=f'models/{url.split("/")[-1]}', n_ctx=2048)
     # If there is a disclaimer, show it
     if personality.disclaimer!="":
         print()
         print("Disclaimer")
         print(personality.disclaimer)
         print()
-
-    # Show conditionning
-    print(full_context)
     
+
+    full_discussion = personality.personality_conditioning+personality.ai_message_prefix+personality.welcome_message+personality.link_text
     while True:
         try:
             prompt = input("You: ")
+            full_discussion+=personality.ai_message_prefix+prompt
             if prompt == '':
                 continue
             print(f"{personality.name}:", end='')
             output=""
             for tok in model.generate(
-                            prompt, 
+                            full_discussion, 
                             n_predict=personality.model_n_predicts, 
                             temp=personality.model_temperature,
                             top_k=personality.model_top_k,
                             top_p=personality.model_top_p,
                             repeat_last_n=personality.model_repeat_last_n,
                             repeat_penalty=personality.model_repeat_penalty
                         ):
@@ -160,14 +155,15 @@
                     print(f"{tok}", end='', flush=True)
             print()
         except KeyboardInterrupt:
             print("Keyboard interrupt detected.\nBye")
             break
     print("Done")
     print(f"{personality}")
+
 ```
 
 # Naming Rationale
 For our new multi-personality AI agent library, we wanted to come up with a naming scheme that reflected our love for science fiction and artificial intelligence. Each release of the application will feature a different AI agent with a distinct personality and set of capabilities, so we felt it was important to give each version a unique and memorable name.
 
 # Current version name: GLaDOS
 GLaDOS is a fictional AI character from the popular video game series "Portal" developed by Valve Corporation. She serves as the primary antagonist throughout the series, with her primary function being the management of the Aperture Science Enrichment Center.
@@ -185,9 +181,150 @@
 2. Create a new branch (`git checkout -b my-new-branch`)
 3. Make your changes
 4. Commit your changes (`git commit -am 'Add some feature'`)
 5. Push to the branch (`git push origin my-new-branch`)
 6. Create a new pull request
 
 
+To build a new personality, you only need to have a config.yaml file with the following fields:
+
+- author
+    - YAML field: `author`
+    - Description: The author of the personality.
+
+- version
+    - YAML field: `version`
+    - Description: The version number of the personality.
+
+- personality_description
+    - YAML field: `personality_description`
+    - Description: A description of the personality, providing information about its characteristics and behavior.
+
+- disclaimer
+    - YAML field: `disclaimer`
+    - Description: A disclaimer or legal statement regarding the use of the personality and any associated liabilities.
+
+- language
+    - YAML field: `language`
+    - Description: The language code or identifier used by the personality (e.g., "en_US" for American English).
+
+- category
+    - YAML field: `category`
+    - Description: The category or type of the personality (e.g., "General", "Technical Support", "Entertainment").
+
+- name
+    - YAML field: `name`
+    - Description: The name or title of the personality.
+
+- user_name
+    - YAML field: `user_name`
+    - Description: The username or identifier associated with the user interacting with the personality.
+
+- personality_conditioning
+    - YAML field: `personality_conditioning`
+    - Description: Information or context about the personality, including its purpose, capabilities, and origin.
+
+- ai_message_prefix
+    - YAML field: `ai_message_prefix`
+    - Description: The prefix or tag used to identify messages generated by the AI assistant.
+
+- welcome_message
+    - YAML field: `welcome_message`
+    - Description: A welcoming message displayed when interacting with the personality.
+
+- link_text
+    - YAML field: `link_text`
+    - Description: Additional text or formatting used for line breaks or spacing in messages.
+
+- user_message_prefix
+    - YAML field: `user_message_prefix`
+    - Description: The prefix or tag used to identify messages generated by the user.
+
+- anti_prompts
+    - YAML field: `anti_prompts`
+    - Description: A list of strings or patterns that can be used to identify and exclude certain message types from prompts or inputs.
+
+- dependencies
+    - YAML field: `dependencies`
+    - Description: A list of dependencies or external resources required by the personality.
+
+- model_temperature
+    - YAML field: `model_temperature`
+    - Description: The temperature value controlling the randomness of the AI model's responses. Higher values result in more creative outputs.
+
+- model_n_predicts
+    - YAML field: `model_n_predicts`
+    - Description: The number of words or tokens to generate in each response from the AI model.
+
+- model_top_k
+    - YAML field: `model_top_k`
+    - Description: The value of K used in the top-K sampling algorithm, controlling the diversity of the generated responses.
+
+- model_top_p
+    - YAML field: `model_top_p`
+    - Description: The value of p used in the nucleus sampling algorithm, controlling the diversity of the generated responses.
+
+- model_repeat_penalty
+    - YAML field: `model_repeat_penalty`
+    - Description: The penalty factor applied to repeated words or phrases in the generated responses to encourage more varied outputs.
+
+- model_repeat_last_n
+    - YAML field: `model_repeat_last_n`
+    - Description: The number of previous tokens to consider when calculating the repetition penalty.
+
+# Information
+From v 0.0.11, we have added processors which allow your personality to have a spersonalized script that is applied on the use text or the ai output text.
+You must put the code inside a file called `processor.py` inside a subfolder called scripts.
+
+inside `processor.py` create a class that inherits from `from pyaipersonality import PAPScript`.
+
+Here is the current form of this class. it will have more elements in the future:
+Look at gpt4internetv0 and gpt4intervet examples for more information
+```python
+class PAPScript:
+    """
+    Template class for implementing personality processor classes in the PAPScript framework.
+
+    This class provides a basic structure and placeholder methods for processing model inputs and outputs.
+    Personality-specific processor classes should inherit from this class and override the necessary methods.
+
+    Methods:
+        process_model_input(text): Process the model input.
+        process_model_output(text): Process the model output.
+    """
+    def __init__(self) -> None:
+        pass
+
+    def process_model_input(self, text):
+        """
+        Process the model input.
+
+        This method should be overridden in the personality-specific processor class to define
+        the desired behavior for processing the model input.
+
+        Args:
+            text (str): The model input text.
+
+        Returns:
+            Any: The processed model input.
+        """
+        return None
+
+    def process_model_output(self, text):
+        """
+        Process the model output.
+
+        This method should be overridden in the personality-specific processor class to define
+        the desired behavior for processing the model output.
+
+        Args:
+            text (str): The model output text.
+
+        Returns:
+            Any: The processed model output.
+        """
+        return None
+
+```
+
 # License
 PyAIPersonality is licensed under the Apache 2.0 license. See the `LICENSE` file for more information.
```

### Comparing `pyaipersonality-0.0.9/setup.py` & `pyaipersonality-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 requirements = read_requirements("requirements.txt")
 requirements_dev = read_requirements("requirements_dev.txt")
 
 setuptools.setup(
     name="pyaipersonality",
-    version="0.0.9",
+    version="1.0.0",
     author="Saifeddine ALOUI",
     author_email="aloui.saifeddine@gmail.com",
     description="A python library for AI personality definition",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/PyAIPersonality",
     packages=setuptools.find_packages(),
```

