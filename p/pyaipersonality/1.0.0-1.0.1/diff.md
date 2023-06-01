# Comparing `tmp/pyaipersonality-1.0.0.tar.gz` & `tmp/pyaipersonality-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaipersonality-1.0.0.tar", last modified: Wed May 31 23:51:22 2023, max compression
+gzip compressed data, was "pyaipersonality-1.0.1.tar", last modified: Thu Jun  1 21:46:24 2023, max compression
```

## Comparing `pyaipersonality-1.0.0.tar` & `pyaipersonality-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 23:51:22.746039 pyaipersonality-1.0.0/
--rw-rw-rw-   0        0        0    11558 2023-04-29 07:11:51.000000 pyaipersonality-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    14413 2023-05-31 23:51:22.746039 pyaipersonality-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    13920 2023-05-07 01:23:25.000000 pyaipersonality-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 23:51:22.731094 pyaipersonality-1.0.0/pyaipersonality/
--rw-rw-rw-   0        0        0    31620 2023-05-31 22:07:47.000000 pyaipersonality-1.0.0/pyaipersonality/__init__.py
--rw-rw-rw-   0        0        0     6626 2023-05-31 23:13:08.000000 pyaipersonality-1.0.0/pyaipersonality/binding.py
--rw-rw-rw-   0        0        0     9357 2023-05-31 23:39:19.000000 pyaipersonality-1.0.0/pyaipersonality/langchain_integration.py
--rw-rw-rw-   0        0        0     3852 2023-05-31 23:37:08.000000 pyaipersonality-1.0.0/pyaipersonality/server.py
-drwxrwxrwx   0        0        0        0 2023-05-31 23:51:22.745043 pyaipersonality-1.0.0/pyaipersonality.egg-info/
--rw-rw-rw-   0        0        0    14413 2023-05-31 23:51:22.000000 pyaipersonality-1.0.0/pyaipersonality.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-05-31 23:51:22.000000 pyaipersonality-1.0.0/pyaipersonality.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 23:51:22.000000 pyaipersonality-1.0.0/pyaipersonality.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-05-31 23:51:22.000000 pyaipersonality-1.0.0/pyaipersonality.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-31 23:51:22.000000 pyaipersonality-1.0.0/pyaipersonality.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 23:51:22.746039 pyaipersonality-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1075 2023-05-31 23:48:18.000000 pyaipersonality-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:46:24.154505 pyaipersonality-1.0.1/
+-rw-rw-rw-   0        0        0    11558 2023-04-29 07:11:51.000000 pyaipersonality-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0    14413 2023-06-01 21:46:24.154505 pyaipersonality-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    13920 2023-05-07 01:23:25.000000 pyaipersonality-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 21:46:24.135763 pyaipersonality-1.0.1/pyaipersonality/
+-rw-rw-rw-   0        0        0    32027 2023-06-01 21:38:22.000000 pyaipersonality-1.0.1/pyaipersonality/__init__.py
+-rw-rw-rw-   0        0        0     6608 2023-06-01 17:42:39.000000 pyaipersonality-1.0.1/pyaipersonality/binding.py
+-rw-rw-rw-   0        0        0     9357 2023-05-31 23:39:19.000000 pyaipersonality-1.0.1/pyaipersonality/langchain_integration.py
+-rw-rw-rw-   0        0        0     7535 2023-06-01 21:41:53.000000 pyaipersonality-1.0.1/pyaipersonality/lllm_server.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:46:24.153504 pyaipersonality-1.0.1/pyaipersonality.egg-info/
+-rw-rw-rw-   0        0        0    14413 2023-06-01 21:46:24.000000 pyaipersonality-1.0.1/pyaipersonality.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      389 2023-06-01 21:46:24.000000 pyaipersonality-1.0.1/pyaipersonality.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 21:46:24.000000 pyaipersonality-1.0.1/pyaipersonality.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-06-01 21:46:24.000000 pyaipersonality-1.0.1/pyaipersonality.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      143 2023-06-01 21:46:24.000000 pyaipersonality-1.0.1/pyaipersonality.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-01 21:46:24.000000 pyaipersonality-1.0.1/pyaipersonality.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 21:46:24.155506 pyaipersonality-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2023-06-01 17:52:13.000000 pyaipersonality-1.0.1/setup.py
```

### Comparing `pyaipersonality-1.0.0/LICENSE` & `pyaipersonality-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaipersonality-1.0.0/PKG-INFO` & `pyaipersonality-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaipersonality
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/PyAIPersonality
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyaipersonality-1.0.0/README.md` & `pyaipersonality-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyaipersonality-1.0.0/pyaipersonality/__init__.py` & `pyaipersonality-1.0.1/pyaipersonality/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     # Run the workflow
     my_processor.run_workflow(generate_fn, prompt)
     ```
     """
     def __init__(self) -> None:
         pass
 
-    def run_workflow(self, generate_fn, prompt, previous_discussion_text="", callback=None):
+    def run_workflow(self, prompt, previous_discussion_text="", callback=None):
         """
         Runs the workflow for processing the model input and output.
 
         This method should be called to execute the processing workflow.
 
         Args:
             generate_fn (function): A function that generates model output based on the input prompt.
@@ -181,39 +181,48 @@
         # Version
         self._version = pkg_resources.get_distribution('pyaipersonality').version
 
         self.run_scripts = run_scripts
 
         #General information
         self._author: str = "ParisNeo"
-        self._name: str = "gpt4all"
+        self._name: str = "LLLM"
         self._user_name: str = "user"
         self._language: str = "en_XX"
         self._category: str = "General"
 
         # Conditionning
         self._personality_description: str = "This personality is a helpful and Kind AI ready to help you solve your problems"
-        self._personality_conditioning: str = "GPT4All is a smart and helpful Assistant built by Nomic-AI. It can discuss with humans and assist them.\nDate: {{date}}"
-        self._welcome_message: str = "Welcome! I am GPT4All A free and open assistant. What can I do for you today?"
+        self._personality_conditioning: str = """## Instructions:
+LLLM (Lord of LLMs) is a smart and helpful Assistant built by the computer geek ParisNeo.
+It is compatible with many bindings to LLM models such as llama, gpt4all, gptj, autogptq etc.
+It can discuss with humans and assist them on many subjects.
+It runs locally on your machine. No need to connect to the internet.
+It answers the questions with precise details
+Its performance depends on the underlying model size and training.
+Try to answer with as much details as you can
+Date: {{date}}
+"""
+        self._welcome_message: str = "Welcome! I am LLLM (Lord of LLMs) A free and open assistant built by ParisNeo. What can I do for you today?"
         self._include_welcome_message_in_disucssion: bool = True
-        self._user_message_prefix: str = "### Human:"
+        self._user_message_prefix: str = "## Human: "
         self._link_text: str = "\n"
-        self._ai_message_prefix: str = "### Assistant:"
-        self._anti_prompts:list = ["###Human","###Assistant","### Human","### Assistant"]
+        self._ai_message_prefix: str = "## LLLM:"
+        self._anti_prompts:list = ["## Human","## LLLM","##Human","##Assistant","##LLLM"]
 
         # Extra
         self._dependencies: List[str] = []
 
         # Disclaimer
         self._disclaimer: str = ""
 
         
         # Default model parameters
         self._model_temperature: float = 0.8 # higher: more creative, lower more deterministic
-        self._model_n_predicts: int = 1024 # higher: generates many words, lower generates
+        self._model_n_predicts: int = 2048 # higher: generates many words, lower generates
         self._model_top_k: int = 50
         self._model_top_p: float = 0.95
         self._model_repeat_penalty: float = 1.3
         self._model_repeat_last_n: int = 40
         
         self._processor_cfg: dict = {}
```

### Comparing `pyaipersonality-1.0.0/pyaipersonality/binding.py` & `pyaipersonality-1.0.1/pyaipersonality/binding.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,24 +144,24 @@
         self.config = config
         self.inline = inline
 
 
     def generate(self, 
                  prompt:str,                  
                  n_predict: int = 128,
-                 new_text_callback: Callable[[str], None] = None,
+                 callback: Callable[[str], None] = None,
                  verbose: bool = False,
                  **gpt_params ):
         """Generates text out of a prompt
         This should ber implemented by child class
 
         Args:
             prompt (str): The prompt to use for generation
             n_predict (int, optional): Number of tokens to prodict. Defaults to 128.
-            new_text_callback (Callable[[str], None], optional): A callback function that is called everytime a new text element is generated. Defaults to None.
+            callback (Callable[[str], None], optional): A callback function that is called everytime a new text element is generated. Defaults to None.
             verbose (bool, optional): If true, the code will spit many informations about the generation process. Defaults to False.
         """
         pass
     def tokenize(self, prompt):
         """
         Tokenizes the given prompt using the model's tokenizer.
```

### Comparing `pyaipersonality-1.0.0/pyaipersonality/langchain_integration.py` & `pyaipersonality-1.0.1/pyaipersonality/langchain_integration.py`

 * *Files identical despite different names*

### Comparing `pyaipersonality-1.0.0/pyaipersonality.egg-info/PKG-INFO` & `pyaipersonality-1.0.1/pyaipersonality.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaipersonality
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/PyAIPersonality
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyaipersonality-1.0.0/setup.py` & `pyaipersonality-1.0.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,23 +13,28 @@
 
 
 requirements = read_requirements("requirements.txt")
 requirements_dev = read_requirements("requirements_dev.txt")
 
 setuptools.setup(
     name="pyaipersonality",
-    version="1.0.0",
+    version="1.0.1",
     author="Saifeddine ALOUI",
     author_email="aloui.saifeddine@gmail.com",
     description="A python library for AI personality definition",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/PyAIPersonality",
     packages=setuptools.find_packages(),
     install_requires=requirements,
+    entry_points={
+        'console_scripts': [
+            'pyaipersonality-server = pyaipersonality.lllm_server:main',
+        ],
+    },
     extras_require={"dev": requirements_dev},
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
 )
```

