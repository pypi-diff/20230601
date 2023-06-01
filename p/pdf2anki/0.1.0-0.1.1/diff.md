# Comparing `tmp/pdf2anki-0.1.0.tar.gz` & `tmp/pdf2anki-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf2anki-0.1.0.tar", last modified: Thu Jun  1 17:23:54 2023, max compression
+gzip compressed data, was "pdf2anki-0.1.1.tar", last modified: Thu Jun  1 18:33:49 2023, max compression
```

## Comparing `pdf2anki-0.1.0.tar` & `pdf2anki-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 fcarva844   (501) staff       (20)        0 2023-06-01 17:23:54.331585 pdf2anki-0.1.0/
--rw-r--r--   0 fcarva844   (501) staff       (20)      456 2023-06-01 17:23:54.330112 pdf2anki-0.1.0/PKG-INFO
--rw-r--r--   0 fcarva844   (501) staff       (20)        0 2023-06-01 16:19:45.000000 pdf2anki-0.1.0/README.md
-drwxr-xr-x   0 fcarva844   (501) staff       (20)        0 2023-06-01 17:23:54.322203 pdf2anki-0.1.0/pdf2anki/
--rw-r--r--   0 fcarva844   (501) staff       (20)        0 2023-06-01 16:20:10.000000 pdf2anki-0.1.0/pdf2anki/__init__.py
--rw-r--r--   0 fcarva844   (501) staff       (20)     5654 2023-06-01 17:12:04.000000 pdf2anki-0.1.0/pdf2anki/main.py
-drwxr-xr-x   0 fcarva844   (501) staff       (20)        0 2023-06-01 17:23:54.328699 pdf2anki-0.1.0/pdf2anki.egg-info/
--rw-r--r--   0 fcarva844   (501) staff       (20)      456 2023-06-01 17:23:54.000000 pdf2anki-0.1.0/pdf2anki.egg-info/PKG-INFO
--rw-r--r--   0 fcarva844   (501) staff       (20)      250 2023-06-01 17:23:54.000000 pdf2anki-0.1.0/pdf2anki.egg-info/SOURCES.txt
--rw-r--r--   0 fcarva844   (501) staff       (20)        1 2023-06-01 17:23:54.000000 pdf2anki-0.1.0/pdf2anki.egg-info/dependency_links.txt
--rw-r--r--   0 fcarva844   (501) staff       (20)       48 2023-06-01 17:23:54.000000 pdf2anki-0.1.0/pdf2anki.egg-info/entry_points.txt
--rw-r--r--   0 fcarva844   (501) staff       (20)       30 2023-06-01 17:23:54.000000 pdf2anki-0.1.0/pdf2anki.egg-info/requires.txt
--rw-r--r--   0 fcarva844   (501) staff       (20)        9 2023-06-01 17:23:54.000000 pdf2anki-0.1.0/pdf2anki.egg-info/top_level.txt
--rw-r--r--   0 fcarva844   (501) staff       (20)       38 2023-06-01 17:23:54.331745 pdf2anki-0.1.0/setup.cfg
--rw-r--r--   0 fcarva844   (501) staff       (20)      842 2023-06-01 16:56:46.000000 pdf2anki-0.1.0/setup.py
+drwxr-xr-x   0 fcarva844   (501) staff       (20)        0 2023-06-01 18:33:49.762233 pdf2anki-0.1.1/
+-rw-r--r--   0 fcarva844   (501) staff       (20)     1062 2023-06-01 18:28:39.000000 pdf2anki-0.1.1/LICENSE
+-rw-r--r--   0 fcarva844   (501) staff       (20)     2359 2023-06-01 18:33:49.759541 pdf2anki-0.1.1/PKG-INFO
+-rw-r--r--   0 fcarva844   (501) staff       (20)     1877 2023-06-01 18:28:52.000000 pdf2anki-0.1.1/README.md
+drwxr-xr-x   0 fcarva844   (501) staff       (20)        0 2023-06-01 18:33:49.722526 pdf2anki-0.1.1/pdf2anki/
+-rw-r--r--   0 fcarva844   (501) staff       (20)        0 2023-06-01 18:28:52.000000 pdf2anki-0.1.1/pdf2anki/__init__.py
+-rw-r--r--   0 fcarva844   (501) staff       (20)     6121 2023-06-01 18:28:52.000000 pdf2anki-0.1.1/pdf2anki/main.py
+drwxr-xr-x   0 fcarva844   (501) staff       (20)        0 2023-06-01 18:33:49.754373 pdf2anki-0.1.1/pdf2anki.egg-info/
+-rw-r--r--   0 fcarva844   (501) staff       (20)     2359 2023-06-01 18:33:49.000000 pdf2anki-0.1.1/pdf2anki.egg-info/PKG-INFO
+-rw-r--r--   0 fcarva844   (501) staff       (20)      258 2023-06-01 18:33:49.000000 pdf2anki-0.1.1/pdf2anki.egg-info/SOURCES.txt
+-rw-r--r--   0 fcarva844   (501) staff       (20)        1 2023-06-01 18:33:49.000000 pdf2anki-0.1.1/pdf2anki.egg-info/dependency_links.txt
+-rw-r--r--   0 fcarva844   (501) staff       (20)       48 2023-06-01 18:33:49.000000 pdf2anki-0.1.1/pdf2anki.egg-info/entry_points.txt
+-rw-r--r--   0 fcarva844   (501) staff       (20)       30 2023-06-01 18:33:49.000000 pdf2anki-0.1.1/pdf2anki.egg-info/requires.txt
+-rw-r--r--   0 fcarva844   (501) staff       (20)        9 2023-06-01 18:33:49.000000 pdf2anki-0.1.1/pdf2anki.egg-info/top_level.txt
+-rw-r--r--   0 fcarva844   (501) staff       (20)       38 2023-06-01 18:33:49.762486 pdf2anki-0.1.1/setup.cfg
+-rw-r--r--   0 fcarva844   (501) staff       (20)      844 2023-06-01 18:28:52.000000 pdf2anki-0.1.1/setup.py
```

### Comparing `pdf2anki-0.1.0/pdf2anki/main.py` & `pdf2anki-0.1.1/pdf2anki/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import argparse
 import PyPDF2
 import openai
 import logging
 from joblib import load
 from typing import List
 
-# Initialize OpenAI API with your key
+# Initialize OpenAI API
 openai.api_key = os.getenv('OPENAI_API_KEY')
 
 ROOT_DIRECTORY = os.path.dirname(os.path.realpath(__file__))
 
 # Load the classifier and vectorizer
 classifier = load('classifier.joblib')
 vectorizer = load('vectorizer.joblib')
@@ -63,25 +63,29 @@
         section_size (int): The desired section size.
 
     Returns:
         List[str]: The divided text sections.
     """
     return [text[i:i+section_size] for i in range(0, len(text), section_size)]
 
-def create_anki_cards(pdf_text: str, output_file: str, model: str, temperature: float, max_tokens: int, section_size: int = 1000):
+def create_anki_cards(pdf_text: str, output_file: str, model: str, temperature: float, max_tokens: int, api_key: str, section_size: int = 1000):
     """Generate Anki cards from a PDF text and save to a file.
 
     Args:
         pdf_text (str): The extracted PDF text.
         output_file (str): Path to save the generated flashcards.
         model (str): The OpenAI model to use for generation.
         temperature (float): The OpenAI temperature setting.
         max_tokens (int): The maximum number of tokens for the OpenAI model.
+        api_key (str): The OpenAI API key.
         section_size (int, optional): The size of text sections. Defaults to 1000.
     """
+    # Set the API key
+    openai.api_key = api_key
+    
     try:
         divided_sections = divide_text(pdf_text, section_size)
         generated_flashcards = ''
         for i, text in enumerate(divided_sections):
             # Classify the text
             predicted_label = classify_text(text)
             messages = [
@@ -99,15 +103,15 @@
             if i==0:
                 break
         with open(output_file, "w") as f:
             f.write(generated_flashcards)
     except Exception as e:
         logging.error(f"Failed to create Anki cards. Error: {str(e)}")
 
-def main_func(source_dir: str, output_dir: str, model: str, temperature: float, max_tokens: int):
+def main_func(source_dir: str, output_dir: str, model: str, temperature: float, max_tokens: int, api_key: str):
     """Main execution function.
 
     Args:
         source_dir (str): Directory containing source PDFs.
         output_dir (str): Directory for output files.
         model (str): The OpenAI model to use for generation.
         temperature (float): The OpenAI temperature setting.
@@ -120,22 +124,30 @@
         logging.info(f"The output directory {output_dir} does not exist. Creating it.")
         os.makedirs(output_dir)
     
     for file_name in os.listdir(source_dir):
         if file_name.endswith(".pdf"):
             pdf_text = read_pdf(os.path.join(source_dir, file_name))
             output_file = os.path.join(output_dir, file_name.rsplit(".", 1)[0] + ".txt")
-            create_anki_cards(pdf_text, output_file, model, temperature, max_tokens)
+            create_anki_cards(pdf_text, output_file, model, temperature, max_tokens, api_key)
 
 def main():
     parser = argparse.ArgumentParser(description='Generate Anki flashcards from PDFs')
     parser.add_argument('--source-dir', type=str, required=True, help='Directory containing source PDFs')
     parser.add_argument('--output-dir', type=str, required=True, help='Directory for output files')
     parser.add_argument('--model', type=str, required=False, default='gpt-3.5-turbo', help='The OpenAI model to use for generation')
     parser.add_argument('--temperature', type=float, required=False, default='0.3', help='The OpenAI temperature setting')
     parser.add_argument('--max-tokens', type=int, required=False, default='2048', help='The maximum number of tokens for the OpenAI model')
+    parser.add_argument('--api-key', type=str, required=False, help='The OpenAI API key')
     parser.add_argument('--section-size', type=int, default=1000, help='Section size for dividing text')
     args = parser.parse_args()
-    main_func(args.source_dir, args.output_dir, args.model, args.temperature, args.max_tokens)
+    
+    api_key = args.api_key if args.api_key else os.getenv('OPENAI_API_KEY')
+    
+    if not api_key:
+        print('No OpenAI API key found. Please set OPENAI_API_KEY in your environment or pass the --api-key argument.')
+        return
+    
+    main_func(args.source_dir, args.output_dir, args.model, args.temperature, args.max_tokens, api_key)
 
 if __name__ == "__main__":
     main()
```

### Comparing `pdf2anki-0.1.0/setup.py` & `pdf2anki-0.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pdf2anki',
-    version='0.1.0',
+    version='0.1.1',
     description='A Python package to create Anki cards from PDFs using OpenAI.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Fabio Carvalho',
-    author_email='email@fabioac.com',
+    author_email='hipnologo@gmail.com',
     url='https://github.com/hipnologo/pdf2anki',
     packages=find_packages(exclude=['pdftoanki']),
     install_requires=[
         'openai>=0.27.0',
         'PyPDF2>=1.26.0',
     ],
     classifiers=[
```

