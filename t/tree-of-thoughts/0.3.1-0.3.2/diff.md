# Comparing `tmp/tree-of-thoughts-0.3.1.tar.gz` & `tmp/tree-of-thoughts-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree-of-thoughts-0.3.1.tar", last modified: Tue May 30 15:09:00 2023, max compression
+gzip compressed data, was "tree-of-thoughts-0.3.2.tar", last modified: Thu Jun  1 02:10:00 2023, max compression
```

## Comparing `tree-of-thoughts-0.3.1.tar` & `tree-of-thoughts-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:09:00.354980 tree-of-thoughts-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 15:08:47.000000 tree-of-thoughts-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-30 15:09:00.354980 tree-of-thoughts-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13951 2023-05-30 15:08:47.000000 tree-of-thoughts-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 15:09:00.354980 tree-of-thoughts-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-30 15:08:47.000000 tree-of-thoughts-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:09:00.350980 tree-of-thoughts-0.3.1/tree_of_thoughts/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-30 15:08:47.000000 tree-of-thoughts-0.3.1/tree_of_thoughts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-30 15:08:47.000000 tree-of-thoughts-0.3.1/tree_of_thoughts/abstractLanguageModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-05-30 15:08:47.000000 tree-of-thoughts-0.3.1/tree_of_thoughts/guidanceModels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-05-30 15:08:47.000000 tree-of-thoughts-0.3.1/tree_of_thoughts/huggingModels.py
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-05-30 15:08:47.000000 tree-of-thoughts-0.3.1/tree_of_thoughts/openaiModels.py
--rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-05-30 15:08:47.000000 tree-of-thoughts-0.3.1/tree_of_thoughts/treeofthoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:09:00.354980 tree-of-thoughts-0.3.1/tree_of_thoughts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-30 15:09:00.000000 tree-of-thoughts-0.3.1/tree_of_thoughts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-30 15:09:00.000000 tree-of-thoughts-0.3.1/tree_of_thoughts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 15:09:00.000000 tree-of-thoughts-0.3.1/tree_of_thoughts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-30 15:09:00.000000 tree-of-thoughts-0.3.1/tree_of_thoughts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-30 15:09:00.000000 tree-of-thoughts-0.3.1/tree_of_thoughts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:10:00.663338 tree-of-thoughts-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-01 02:09:47.000000 tree-of-thoughts-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-01 02:10:00.663338 tree-of-thoughts-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-01 02:09:47.000000 tree-of-thoughts-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 02:10:00.663338 tree-of-thoughts-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-01 02:09:47.000000 tree-of-thoughts-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:10:00.663338 tree-of-thoughts-0.3.2/tree_of_thoughts/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-01 02:09:47.000000 tree-of-thoughts-0.3.2/tree_of_thoughts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-01 02:09:47.000000 tree-of-thoughts-0.3.2/tree_of_thoughts/abstractLanguageModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-06-01 02:09:47.000000 tree-of-thoughts-0.3.2/tree_of_thoughts/guidanceModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-01 02:09:47.000000 tree-of-thoughts-0.3.2/tree_of_thoughts/huggingModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10885 2023-06-01 02:09:47.000000 tree-of-thoughts-0.3.2/tree_of_thoughts/openaiModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-06-01 02:09:47.000000 tree-of-thoughts-0.3.2/tree_of_thoughts/treeofthoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:10:00.663338 tree-of-thoughts-0.3.2/tree_of_thoughts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-01 02:10:00.000000 tree-of-thoughts-0.3.2/tree_of_thoughts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-01 02:10:00.000000 tree-of-thoughts-0.3.2/tree_of_thoughts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 02:10:00.000000 tree-of-thoughts-0.3.2/tree_of_thoughts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-01 02:10:00.000000 tree-of-thoughts-0.3.2/tree_of_thoughts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-01 02:10:00.000000 tree-of-thoughts-0.3.2/tree_of_thoughts.egg-info/top_level.txt
```

### Comparing `tree-of-thoughts-0.3.1/LICENSE` & `tree-of-thoughts-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.3.1/PKG-INFO` & `tree-of-thoughts-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.3.1
+Version: 0.3.2
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tree-of-thoughts-0.3.1/README.md` & `tree-of-thoughts-0.3.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Tree of Thoughts 🌳🌲🌴🌿🍃
 
-![tree of thoughts banner](tree-of-thoughts.jpeg)
+![tree of thoughts banner](tree-of-thoughts.png)
 
 [Paper link](https://arxiv.org/pdf/2305.10601.pdf)
 
 Tree of Thoughts (ToT) is an all-new powerful and flexible algorithm that advances model reasoning by a whopping 70%. This is an plug in and play verision, connect your own models and enjoy superintelligence!
 
 
 Share this repository by clicking on the following buttons 😊 
@@ -21,15 +21,19 @@
 
 # Basic Prompts:
 No complex implementations, just pass in one of these prompts to your model: head over to `prompts.txt`
 
 'Three experts with exceptional logical thinking skills are collaboratively answering a question using a tree of thoughts method. Each expert will share their thought process in detail, taking into account the previous thoughts of others and admitting any errors. They will iteratively refine and expand upon each other's ideas, giving credit where it's due. The process continues until a conclusive answer is found. Organize the entire response in a markdown table format. The question is...'
 
 ## Getting started
-Set Openai key in your environment file `.env.` as `OPENAI_API_KEY='SK'`
+Set Openai key in an environment file,
+
+first create an file called: `.env` 
+
+Then get your openai key and input it inside the '' as `OPENAI_API_KEY='SK-YOUR KEY'`
 
 
 ## Method1
 Clone this repository with 
 
 ```git clone https://github.com/kyegomez/tree-of-thoughts```
 
@@ -37,28 +41,30 @@
 cd tree-of-thoughts
 python3 -m pip install -r requirements.txt
 cd tree_of_thoughts
 python3 treeofthoughts.py --problem "design an new transportation system for an all-new city" --search_algorithm="BFS"
 ```
 Add ` OPENAI_API_KEY='API KEY'` in the .env!
 
+!!!! For much improved performance provide custom few prompt shots in the generate thoughts and generate states! !!!!!
+
 And in the `examples` folder we have other examples for huggingface transformers + hugginggface pipelines
 
 ## Method2
 or:
 
 ```pip install tree-of-thoughts ```
 
 
 Create a Python script (e.g., example.py) and import the necessary classes:
 
 ``` python
 import os
-from tree_of_thoughts.openaiModels import OptimizedOpenAILanguageModel
-from tree_of_thoughts.treeofthoughts import TreeofThoughts
+from tree_of_thoughts import OptimizedOpenAILanguageModel
+from tree_of_thoughts import TreeofThoughts
 
 
 api_key = os.getenv("OPENAI_API_KEY")
 model = OptimizedOpenAILanguageModel(api_key=api_key) # api_model="gpt4" # for higher performance base model is not smart
 
 
 #choose search algorithm('BFS' or 'DFS')
@@ -187,15 +193,15 @@
 ``` 
 git clone https://github.com/kyegomez/tree-of-thoughts
 cd tree-of-thoughts
 python3 huggingfaceExample.py
 ```
 
 ```python
-from tree_of_thoughts.tree_of_thoughts import HuggingLanguageModel
+from tree_of_thoughts import HuggingLanguageModel
 
 model_name="gpt2"
 model_tokenizer="your tokenizer"
 
 huggingface_model = HuggingLanguageModel(model_name, model_tokenizer)
 ```
 
@@ -213,19 +219,19 @@
 
         inputs = self.tokenizer(prompt, return_tensors="pt")
         outputs = self.model.generate(**inputs, num_return_sequences=k)
         thoughts = [self.tokenizer.decode(output, skip_special_tokens=True) for output in outputs]
 
         return thoughts
 
-    def evaluate_states(self, states, inital_prompt):
+    def evaluate_states(self, states, initial_prompt):
         state_values = {}
         for state in states:
             state_text = ' '.join(state)
-            prompt = f"Given the current state of reasoning: '{state_text}', pessimitically evaluate its value as a float between 0 and 1 based on it's potential to achieve {inital_prompt}"
+            prompt = f"Given the current state of reasoning: '{state_text}', pessimitically evaluate its value as a float between 0 and 1 based on it's potential to achieve {initial_prompt}"
 
             inputs = self.tokenizer(prompt, return_tensors="pt")
             outputs = self.model.generate(**inputs, num_return_sequences=1)
             value_text = self.tokenizer.decode(outputs[0], skip_special_tokens=True)
 
             try:
                 value = float(value_text)
@@ -252,62 +258,33 @@
 
 For Instagram, while it doesn't directly support sharing of web links, you can share the screenshot of our project and the link in your caption or bio. You can download the project screenshot by clicking the image below:
 
 [![Tree of Thoughts](https://github.com/kyegomez/tree-of-thoughts/raw/main/tree-of-thoughts.jpeg)](https://github.com/kyegomez/tree-of-thoughts/raw/main/tree-of-thoughts.jpeg)
 
 We greatly appreciate any help in spreading the word about our project. Thank you for your support!
 
+# Roadmap:
 
-## Roadmap
-
-now:
-Generate suite of evaluations used in the paper testing AI agents with other reasoning methods like COT and self consistency and run them in parallel to conduct evaluation experiments.
-
-Implement a more sophisticated prompt engineering strategy to guide the model's reasoning process more effectively.
-
-Script that generates an dataset based on a topic input, -> set of questions are asked, then multiple trees of thoughts are run concurrently to generate the decision making rich dataset
-
-
-Introduce a reinforcement learning, distillment, and finetuning scripts to finely tune the model based on feedback from the Tree of Thoughts algorithm.
-
-Integrate heuristics that autonomously determine the search algorithm based on indicators
-
-Integrate heuristics that autonomously determine the strategy cos or propose
-
-Integrate heuristics that autonomously set the input params:
-
-k = 
-T = 
-b = 
-vth = 
-
-
-# multi modal 
-multi-modality tree of thoughts
-
-multi-modality forest of thoughts
+* Resilient Prompting: Teach model how to think rather than what to think.
 
-multi-modality world of thoughts
+* Add pruning treshold management for precise bad state cutoff
 
+* Evaluating each thought as soon as thought generated then evaluating an chain of thoughts or the state of thoughts by averaging out the values of each thought evaluation.
 
+* Add Traversal method, which "will incapsulate the run of either dfs or bfs under the hood so that the issue of different args is solved from @ivanzhovannik
 
-### Multi-Modality Tree of Thoughts 🌐🌳
+* Add Delay between generate solutions and generate values
 
-The next big advancement for the Tree of Thoughts algorithm is to extend it to multi-modality, enabling it to handle not only text but also images, audio, and other data types. This will bring us closer to multi-modal superintelligence.
+* Dynamic and adaptive parameters, like max steps, num_thoughts, max_states and value threshold that shift depending on the complexity of the user objective.
 
-#### Actionable Steps
+* Add Rejected reasoning metadata (thought, state, reasoning_on_state) into  generate solutions
 
-1. Research and identify suitable multi-modal pre-trained models that can handle various data types (e.g., text, images, audio).
-2. Adapt the thought decomposition, thought generator, and state evaluator functions to handle multi-modal data.
-3. Develop a method for combining different modalities in the search tree, allowing the algorithm to reason across different data types.
-4. Implement and test the multi-modal Tree of Thoughts algorithm with various problems and datasets.
-5. Optimize the algorithm for performance and resource usage, ensuring it scales well with large multi-modal datasets.
-6. Publish the results and gather feedback from the community to further improve the multi-modal Tree of Thoughts algorithm.
+* any other ideas? Please pr request this algorithm is very infant and it's potential is limitless
 
-Join us on this exciting journey to advance the Tree of Thoughts algorithm to multi-modality superintelligence! 🚀
+* Chain of Thought Hub Evaluation tests!
 
 # Documentation:
 
 ## input_problem (str): 
 The initial problem statement or prompt for which the Tree of Thoughts algorithm will generate a solution.
 
 ## num_thoughts (int, default=5):
```

### Comparing `tree-of-thoughts-0.3.1/setup.py` & `tree-of-thoughts-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'tree-of-thoughts',
   packages = find_packages(exclude=[]),
-  version = '0.3.1',
+  version = '0.3.2',
   license='MIT',
   description = 'Tree of Thoughts - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/tree-of-thoughts',
   keywords = [
```

### Comparing `tree-of-thoughts-0.3.1/tree_of_thoughts/guidanceModels.py` & `tree-of-thoughts-0.3.2/tree_of_thoughts/guidanceModels.py`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.3.1/tree_of_thoughts/huggingModels.py` & `tree-of-thoughts-0.3.2/tree_of_thoughts/huggingModels.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
         return thoughts
 
     def evaluate_states(self, states, initial_prompt, max_length=10):
         state_values = {}
         for state in states:
             state_text = ' '.join(state)
-            prompt = f"Given the current state of reasoning: '{state_text}', pessimitically evaluate its value as a float between 0 and 1 based on it's potential to achieve {inital_prompt}"
+            prompt = f"Given the current state of reasoning: '{state_text}', pessimitically evaluate its value as a float between 0 and 1 based on it's potential to achieve {initial_prompt}"
 
             if self.verbose:
                 print(f"Evaluating state: {state_text}")
 
             try:
                 inputs = self.tokenizer(prompt, return_tensors="pt")
                 outputs = self.model.generate(**inputs, num_return_sequences=1, max_length=max_length)
```

### Comparing `tree-of-thoughts-0.3.1/tree_of_thoughts/treeofthoughts.py` & `tree-of-thoughts-0.3.2/tree_of_thoughts/treeofthoughts.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,38 @@
-
+#thought -> evaluated value (0.4, This solution is invalid because x) -> thought prompt + this solution is invalid because + better eval
 
 import os
 import time
 import json
 from tree_of_thoughts.openaiModels import OptimizedOpenAILanguageModel
 DATA_PATH = './data'
 import logging 
 import argparse
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 logger = logging.getLogger(__name__)
 from typing import Any, Dict, List, Optional, Set, Tuple, Union
-
+import re
 
 
 class TreeofThoughts:
     def __init__(self, model, search_algorithm):
         self.model = model
         self.search_algorithm = search_algorithm
-        self.tree: Dict[str, Dict[str, float]] = {
-            "nodes": {}
+        self.tree: Dict[str, Dict[str, Union[float, Dict[str, Any]]]] = {
+            "nodes": {},
+            # "rejected_paths": {}
         }
 
     def solve(self, initial_prompt: str, 
               num_thoughts: Optional[int] = None, 
               max_steps: Optional[int] = None, 
               max_states: Optional[int] = None, 
               value_threshold: Optional[float] = None, 
               pruning_threshold: Optional[float] = 0.5,
-              timeout: Optional[float] = None, 
-              confidence_threshold: Optional[float] = None, 
-              max_iterations: Optional[int] = None, 
-              convergence_threshold: Optional[float] = None, 
-              convergence_count: Optional[int] = None) -> str:
+            ):
         start_time = time.time()
         self.file_name = f"logs/tree_of_thoughts_output_{self.search_algorithm}.json"
         try:
             best_thoughts = ""
             if self.search_algorithm == 'BFS':
                 result = self.tot_bfs(initial_prompt, num_thoughts, max_steps, max_states, pruning_threshold)
                 if result:
@@ -61,77 +58,112 @@
             self.save_tree_to_json(self.file_name)
 
     def logNewState(self, state, evaluation):
         if not (type(state) == str):
             state = " | ".join(state)
         self.tree["nodes"][state] = evaluation
         self.save_tree_to_json(self.file_name)    
+    
+    #reject condition conditioning
+    def reject_condition(self, current_path, rejected_path, reason, value_threshold):
+        if reason["value"] < value_threshold:
+            return True
+        return False
+    
+    def parse_evaluation(self, evaluation):
+        parsed_evaluation = re.findall(r'`(\d+\.\d+)`', evaluation)
+        return parsed_evaluation
+    
+
+
+
+    #takes rejected state value reason -> injects into the the generate solutions prompt.
+    def update_current_branch(self, current_path, rejected_path_info):
+        parsed_evaluation = self.parse_evaluation(rejected_path_info["evaluation"])
+        updated_solution= f"{current_path} {parsed_evaluation}"
+        return updated_solution
+
+    #rejected states passing into next thoughts
+    def integrate_rejected_paths(self, current_path):
+        for rejected_path, reason in self.tree['rejected_paths'].items():
+            if self.reject_condition(current_path, rejected_path, reason):
+                updated_solution = self.update_current_branch(current_path, reason)
+                current_path = updated_solution
+
         
     def tot_bfs(self, initial_prompt, num_thoughts, max_steps, max_states, pruning_threshold):
         current_states = [initial_prompt]
         state_values = {}
         try:
             for step in range(1, max_steps + 1):
                 selected_states = []
                 for state in current_states:
+                    # self.integrate_rejected_paths(state)
+                    #for thought in thoughts:
                     thoughts = self.model.generate_thoughts(state, num_thoughts, initial_prompt)
+                                                            # rejected_solutions=state)
                     evaluated_thoughts = self.model.evaluate_states({thought: 0 for thought in thoughts}, initial_prompt)
                     for thought, value in evaluated_thoughts.items():
                         if value >= pruning_threshold:
                             flattened_state = (state, thought) if isinstance(state, str) else (*state, thought)
                             selected_states.append(flattened_state)
                             state_values[flattened_state] = value
                             self.logNewState(flattened_state, value)
+                        #Rejected loop pruning loop
+                        # else:
+                        #     reason_for_rejection = {"value": value, "evaluation": evaluation}
+                        #     self.tree["rejected_paths"][flattened_state] = reason_for_rejection
+
                 if len(selected_states) > 1:
                     current_states = selected_states[:max_states]
 
             if len(current_states) == 1:
                 return initial_prompt
 
             if current_states:
                 best_state = max(current_states, key=lambda state: state_values[state])
                 return best_state
         except Exception as e:
             logger.error(f"Error in tot_bfs: {e}")
             return None
 
     def tot_dfs(self,
-                inital_prompt: str,
+                initial_prompt: str,
                 num_thoughts: str,
                 max_steps: int,
                 value_threshold,
                 pruning_threshold=0.5):
         output = []
         file_name = f"logs/tree_of_thoughts_output_{self.search_algorithm}.json"
 
         def dfs(state, step):
             nonlocal output
             if step > max_steps:
-                thought = self.model.generate_thoughts(state, 1, inital_prompt)
-                value = self.model.evaluate_states({state}, inital_prompt)[state]
+                thought = self.model.generate_thoughts(state, 1, initial_prompt)
+                value = self.model.evaluate_states({state}, initial_prompt)[state]
                 output.append((thought, value))
                 return 
             
-            for next_state in sorted(self.model.generated_thoughts(state, num_thoughts, inital_prompt)):
-                state_value = self.model.evaluate_states({next_state}, inital_prompt)[next_state]
+            for next_state in sorted(self.model.generated_thoughts(state, num_thoughts, initial_prompt)):
+                state_value = self.model.evaluate_states({next_state}, initial_prompt)[next_state]
                 logger.ingo(f"state: {next_state}, value: {state_value}")
 
 
                 if state_value > value_threshold and (pruning_threshold is None or state_value >= pruning_threshold):
                     if isinstance(state, str):
                         child = (state, next_state)
                     else:
                         child = (*state, next_state)
 
                     dfs(child, step + 1)
 
             self.save_tree_to_json(file_name)
         
         try:
-            dfs(inital_prompt, 1)
+            dfs(initial_prompt, 1)
             best_state = max(output, key=lambda x: x[1])
             return best_state[0]
         except Exception as e:
             logger.error(f"Error in tot_dfs: {e}")
             return None
```

### Comparing `tree-of-thoughts-0.3.1/tree_of_thoughts.egg-info/PKG-INFO` & `tree-of-thoughts-0.3.2/tree_of_thoughts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.3.1
+Version: 0.3.2
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

