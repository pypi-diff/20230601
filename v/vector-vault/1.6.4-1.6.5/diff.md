# Comparing `tmp/vector_vault-1.6.4.tar.gz` & `tmp/vector_vault-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.6.4.tar", last modified: Thu Jun  1 01:06:08 2023, max compression
+gzip compressed data, was "vector_vault-1.6.5.tar", last modified: Thu Jun  1 21:44:38 2023, max compression
```

## Comparing `vector_vault-1.6.4.tar` & `vector_vault-1.6.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-01 01:06:08.099679 vector_vault-1.6.4/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.6.4/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-01 01:06:08.099512 vector_vault-1.6.4/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.6.4/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-01 01:06:08.099717 vector_vault-1.6.4/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-01 01:04:34.000000 vector_vault-1.6.4/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-01 01:06:08.096159 vector_vault-1.6.4/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-01 01:06:08.000000 vector_vault-1.6.4/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-01 01:06:08.000000 vector_vault-1.6.4/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-01 01:06:08.000000 vector_vault-1.6.4/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-01 01:06:08.000000 vector_vault-1.6.4/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-01 01:06:08.000000 vector_vault-1.6.4/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-01 01:06:08.099104 vector_vault-1.6.4/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.6.4/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     6238 2023-05-28 06:54:07.000000 vector_vault-1.6.4/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3249 2023-06-01 00:49:04.000000 vector_vault-1.6.4/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1843 2023-05-30 20:06:58.000000 vector_vault-1.6.4/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.6.4/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1582 2023-06-01 00:49:00.000000 vector_vault-1.6.4/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.6.4/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    18190 2023-06-01 00:49:07.000000 vector_vault-1.6.4/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.6.4/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.6.4/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-01 21:44:38.622686 vector_vault-1.6.5/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.6.5/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-01 21:44:38.622516 vector_vault-1.6.5/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.6.5/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-01 21:44:38.622721 vector_vault-1.6.5/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-01 21:44:19.000000 vector_vault-1.6.5/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-01 21:44:38.619806 vector_vault-1.6.5/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-01 21:44:38.000000 vector_vault-1.6.5/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-01 21:44:38.000000 vector_vault-1.6.5/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-01 21:44:38.000000 vector_vault-1.6.5/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-01 21:44:38.000000 vector_vault-1.6.5/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-01 21:44:38.000000 vector_vault-1.6.5/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-01 21:44:38.622189 vector_vault-1.6.5/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.6.5/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     7621 2023-06-01 06:30:30.000000 vector_vault-1.6.5/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3249 2023-06-01 21:39:08.000000 vector_vault-1.6.5/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1843 2023-05-30 20:06:58.000000 vector_vault-1.6.5/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.6.5/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1582 2023-06-01 21:39:11.000000 vector_vault-1.6.5/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.6.5/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    19247 2023-06-01 21:39:02.000000 vector_vault-1.6.5/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.6.5/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.6.5/vectorvault/wrap.py
```

### Comparing `vector_vault-1.6.4/LICENSE` & `vector_vault-1.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.4/PKG-INFO` & `vector_vault-1.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 1.6.4
+Version: 1.6.5
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.6.4/README.md` & `vector_vault-1.6.5/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.4/setup.py` & `vector_vault-1.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.6.4",
+    version="1.6.5",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.6.4/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.6.5/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 1.6.4
+Version: 1.6.5
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.6.4/vectorvault/__init__.py` & `vector_vault-1.6.5/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.4/vectorvault/ai.py` & `vector_vault-1.6.5/vectorvault/ai.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import tiktoken
 
 class AI:
     def __init__(self) -> None:
         pass
 
     # This function returns a ChatGPT completion based on a provided input.
-    def llm(self, user_input, history=None, model='gpt-3.5-turbo'):
+    def llm(self, user_input, history=None, model='gpt-3.5-turbo', stream=False):
         inchar = len(user_input)
         histchar = len(history) if history else 0
         if inchar + histchar > 16000:
             char_left = 16000 - inchar
             if history:
                 history = history[-char_left:]
         if history:
@@ -35,23 +35,38 @@
                     {"role": "system", "content": f"{history}"},
                     {"role": "user", "content": f"{user_input}"}]
             )
         else:
             # 'model' is the name of the model to use
             # 'messages' is a list of message objects that mimics a conversation.
             # Each object has a 'role' that can be 'system', 'user', or 'assistant', and a 'content' which is the actual content of the message.
-            response = openai.ChatCompletion.create(
-                model="gpt-3.5-turbo",
-                messages=[{"role": "user", "content": f"{user_input}"}]
-            )
+            if stream == False:
+                response = openai.ChatCompletion.create(
+                    model=model,
+                    messages=[{"role": "user", "content": f"{user_input}"}]
+                )
+                return response['choices'][0]['message']['content']
+            elif stream == True:
+                response = openai.ChatCompletion.create(
+                    model=model,
+                    messages=[{"role": "user", "content": f"{user_input}"}],
+                    stream=True
+                )
             # The API responds with a 'choices' array containing the 'message' object.
-        return response['choices'][0]['message']['content']
-    
+                for message in response:
+                    choices = message.get('choices', [])
+                    if choices:
+                        delta = choices[0].get('delta', {})
+                        if 'content' in delta:
+                            content = delta['content']
+                            yield content
+                        
+                    
     # This function returns a ChatGPT completion based contextual input
-    def llm_w_context(self, user_input, context, history=None, model='gpt-3.5-turbo'):
+    def llm_w_context(self, user_input, context, history=None, model='gpt-3.5-turbo', stream=False):
         prompt_template = """
         Use the following pieces of context to answer the question at the end. 
         Answer as if you were the modern voice of the context. Make sure to not just repeat what is referenced. Don't preface, and don't give any warnings at the end.
 
         {context}
 
         Question: {question}
@@ -87,20 +102,36 @@
                     char_to_take_away = remainder * 5
                     context = context[char_to_take_away:]
 
         # Format the prompt
         user_input = history + user_input
         prompt = prompt_template.format(context=context, question=user_input)
 
-        response = openai.ChatCompletion.create(
-            model=model,
-            messages=[
-                {"role": "user", "content": f"{prompt}"}]
-        )
-        return response['choices'][0]['message']['content']
+        if stream == False:
+            response = openai.ChatCompletion.create(
+                model=model,
+                messages=[
+                    {"role": "user", "content": f"{prompt}"}]
+            )
+            return response['choices'][0]['message']['content']
+        elif stream == True:
+            response = openai.ChatCompletion.create(
+                model=model,
+                messages=[
+                    {"role": "user", "content": f"{prompt}"}],
+                stream=True
+            )
+        # The API responds with a 'choices' array containing the 'message' object.
+            for message in response:
+                choices = message.get('choices', [])
+                if choices:
+                    delta = choices[0].get('delta', {})
+                    if 'content' in delta:
+                        content = delta['content']
+                        yield content
 
 
     def summarize(self, user_input, model='gpt-3.5-turbo'):    
         response = openai.ChatCompletion.create(
             model=model,
             messages=[{"role": "user", "content": f"Summarize the following: {user_input}"}]
         )
```

### Comparing `vector_vault-1.6.4/vectorvault/cloudmanager.py` & `vector_vault-1.6.5/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.4/vectorvault/creds.py` & `vector_vault-1.6.5/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.4/vectorvault/download.py` & `vector_vault-1.6.5/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.4/vectorvault/itemize.py` & `vector_vault-1.6.5/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.4/vectorvault/signup.py` & `vector_vault-1.6.5/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.4/vectorvault/vault.py` & `vector_vault-1.6.5/vectorvault/vault.py`

 * *Files 4% similar despite different names*

```diff
@@ -295,15 +295,15 @@
         self.first_run = False
         if self.verbose == True:
             print("get vectors time --- %s seconds ---" % (time.time() - start_time))
 
     def get_chat_cloud(self, text: str, history: str = None, summary: bool = False, get_context = False, n_context = 4, return_context = False, expansion = False, history_search = False, model='gpt-3.5-turbo', include_context_meta=False):
         return call_get_chat(self.user, self.vault, self.api, text, history, summary, get_context, n_context, return_context, expansion, history_search, model, include_context_meta)
     
-    def get_chat(self, text: str, history: str = None, summary: bool = False, get_context = False, n_context = 4, return_context = False, expansion = False, history_search = False, model='gpt-3.5-turbo', include_context_meta=False):
+    def get_chat(self, text: str, history: str = None, summary: bool = False, get_context = False, n_context = 4, return_context = False, expansion = False, history_search = False, model='gpt-3.5-turbo', include_context_meta=False, stream=False):
         '''
             Chat get response from OpenAI's ChatGPT. 
             Rate limiting, auto retries, and chat histroy slicing built-in so you can chat with ease. 
             Enter your text, add optional chat history, and optionally choose a summary response (default: summmary = False)
 
             Example Signle Usage: 
             `response = vault.get_chat(text)`
@@ -401,25 +401,53 @@
                             context = self.get_similar(user_input, n=n_context)
                             input = str(context)
                         else:
                             context = self.get_similar(user_input, n=n_context)
                             input = ''
                             for text in context:
                                 input += text['data']
-                        response = self.ai.llm_w_context(segment, input, history, model=model)
+                        if stream == False:
+                            response = self.ai.llm_w_context(segment, input, history, model=model)
+                        elif stream == True:
+                            for word in self.ai.llm_w_context(segment, input, history, model=model, stream=True):
+                                yield word
                     else:
-                        response = self.ai.llm(segment, history, model=model)
+                        if stream == False:
+                            response = self.ai.llm(segment, history, model=model)
+                        elif stream == True:
+                            for word in self.ai.llm(segment, history, model=model, stream=True):
+                                yield word
                     break
                 except Exception as e:
                     print(f"API Error: {e}. Sleeping 5 seconds")
                     time.sleep(5)
                     
             self.last_chat_time = start_time
 
         if self.verbose == True:
             print("get chat time --- %s seconds ---" % (time.time() - start_time))
 
         if return_context == False:
             return response
         else:
             return {'response': response, 'context': context}
+        
+
+    def print_stream(self, function):
+        full_text= ''
+        newlinetime=1
+        for word in function:
+            full_text += word
+            self.print_stream(word) 
+            if len(full_text) / 80 > newlinetime:
+                newlinetime += 1
+                print('\n', end='', flush=True)
     
+            
+    def cloud_stream(self, function):
+        for word in function:
+            try:
+                word = word.replace('\n', '<br/>')
+                yield f"data: {word} \n\n"
+            except:
+                yield word
+
```

### Comparing `vector_vault-1.6.4/vectorvault/vecreq.py` & `vector_vault-1.6.5/vectorvault/vecreq.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.4/vectorvault/wrap.py` & `vector_vault-1.6.5/vectorvault/wrap.py`

 * *Files identical despite different names*

