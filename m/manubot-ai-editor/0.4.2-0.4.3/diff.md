# Comparing `tmp/manubot-ai-editor-0.4.2.tar.gz` & `tmp/manubot-ai-editor-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manubot-ai-editor-0.4.2.tar", last modified: Fri Apr  7 14:54:32 2023, max compression
+gzip compressed data, was "manubot-ai-editor-0.4.3.tar", last modified: Thu Jun  1 19:40:02 2023, max compression
```

## Comparing `manubot-ai-editor-0.4.2.tar` & `manubot-ai-editor-0.4.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-04-07 14:54:32.087034 manubot-ai-editor-0.4.2/
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2556 2023-04-07 14:54:32.087034 manubot-ai-editor-0.4.2/PKG-INFO
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2074 2023-03-17 13:06:41.000000 manubot-ai-editor-0.4.2/README.md
-drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-04-07 14:54:32.083034 manubot-ai-editor-0.4.2/libs/
-drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-04-07 14:54:32.087034 manubot-ai-editor-0.4.2/libs/manubot_ai_editor/
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)        0 2023-01-25 04:03:27.000000 manubot-ai-editor-0.4.2/libs/manubot_ai_editor/__init__.py
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    16525 2023-03-09 16:05:14.000000 manubot-ai-editor-0.4.2/libs/manubot_ai_editor/editor.py
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2848 2023-04-07 14:50:29.000000 manubot-ai-editor-0.4.2/libs/manubot_ai_editor/env_vars.py
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    20101 2023-04-07 14:50:29.000000 manubot-ai-editor-0.4.2/libs/manubot_ai_editor/models.py
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)      632 2023-01-25 04:03:27.000000 manubot-ai-editor-0.4.2/libs/manubot_ai_editor/utils.py
-drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-04-07 14:54:32.087034 manubot-ai-editor-0.4.2/libs/manubot_ai_editor.egg-info/
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2556 2023-04-07 14:54:32.000000 manubot-ai-editor-0.4.2/libs/manubot_ai_editor.egg-info/PKG-INFO
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)      467 2023-04-07 14:54:32.000000 manubot-ai-editor-0.4.2/libs/manubot_ai_editor.egg-info/SOURCES.txt
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)        1 2023-04-07 14:54:32.000000 manubot-ai-editor-0.4.2/libs/manubot_ai_editor.egg-info/dependency_links.txt
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)       20 2023-04-07 14:54:32.000000 manubot-ai-editor-0.4.2/libs/manubot_ai_editor.egg-info/requires.txt
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)       19 2023-04-07 14:54:32.000000 manubot-ai-editor-0.4.2/libs/manubot_ai_editor.egg-info/top_level.txt
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)       38 2023-04-07 14:54:32.087034 manubot-ai-editor-0.4.2/setup.cfg
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)      938 2023-04-07 14:52:24.000000 manubot-ai-editor-0.4.2/setup.py
-drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-04-07 14:54:32.087034 manubot-ai-editor-0.4.2/tests/
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    62136 2023-04-07 14:50:29.000000 manubot-ai-editor-0.4.2/tests/test_completion_model.py
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    38761 2023-01-25 04:03:27.000000 manubot-ai-editor-0.4.2/tests/test_editor.py
+drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-01 19:40:02.974068 manubot-ai-editor-0.4.3/
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2544 2023-06-01 19:40:02.974068 manubot-ai-editor-0.4.3/PKG-INFO
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2062 2023-06-01 16:26:59.000000 manubot-ai-editor-0.4.3/README.md
+drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-01 19:40:02.974068 manubot-ai-editor-0.4.3/libs/
+drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-01 19:40:02.974068 manubot-ai-editor-0.4.3/libs/manubot_ai_editor/
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)        0 2023-01-26 21:56:19.000000 manubot-ai-editor-0.4.3/libs/manubot_ai_editor/__init__.py
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    16783 2023-06-01 19:27:16.000000 manubot-ai-editor-0.4.3/libs/manubot_ai_editor/editor.py
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2965 2023-06-01 19:38:16.000000 manubot-ai-editor-0.4.3/libs/manubot_ai_editor/env_vars.py
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    20582 2023-06-01 16:43:05.000000 manubot-ai-editor-0.4.3/libs/manubot_ai_editor/models.py
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)      632 2023-01-26 21:56:19.000000 manubot-ai-editor-0.4.3/libs/manubot_ai_editor/utils.py
+drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-01 19:40:02.974068 manubot-ai-editor-0.4.3/libs/manubot_ai_editor.egg-info/
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2544 2023-06-01 19:40:02.000000 manubot-ai-editor-0.4.3/libs/manubot_ai_editor.egg-info/PKG-INFO
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)      498 2023-06-01 19:40:02.000000 manubot-ai-editor-0.4.3/libs/manubot_ai_editor.egg-info/SOURCES.txt
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)        1 2023-06-01 19:40:02.000000 manubot-ai-editor-0.4.3/libs/manubot_ai_editor.egg-info/dependency_links.txt
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)       20 2023-06-01 19:40:02.000000 manubot-ai-editor-0.4.3/libs/manubot_ai_editor.egg-info/requires.txt
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)       19 2023-06-01 19:40:02.000000 manubot-ai-editor-0.4.3/libs/manubot_ai_editor.egg-info/top_level.txt
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)       38 2023-06-01 19:40:02.974068 manubot-ai-editor-0.4.3/setup.cfg
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)      938 2023-06-01 19:08:33.000000 manubot-ai-editor-0.4.3/setup.py
+drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-01 19:40:02.974068 manubot-ai-editor-0.4.3/tests/
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    61034 2023-06-01 15:22:56.000000 manubot-ai-editor-0.4.3/tests/test_completion_model.py
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    40588 2023-06-01 16:32:37.000000 manubot-ai-editor-0.4.3/tests/test_editor.py
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     7738 2023-06-01 16:46:08.000000 manubot-ai-editor-0.4.3/tests/test_model_get_prompt.py
```

### Comparing `manubot-ai-editor-0.4.2/PKG-INFO` & `manubot-ai-editor-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manubot-ai-editor
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Manubot plugin to revise a manuscript using GPT-3
 Home-page: https://github.com/greenelab/manubot-ai-editor
 Author: Milton Pividori
 Author-email: miltondp@gmail.com
 License: BSD-2-Clause Plus Patent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -55,15 +55,15 @@
 
 # first I create a temporary directory to store the revised manuscript
 output_folder = (Path("tmp") / "manubot-ai-editor-output").resolve()
 shutil.rmtree(output_folder, ignore_errors=True)
 output_folder.mkdir(parents=True, exist_ok=True)
 
 # then I revise the manuscript
-me.revise_manuscript(output_folder, model, debug=True)
+me.revise_manuscript(output_folder, model)
 
 # here I move the revised manuscript back to the content folder
 # CAUTION: this will overwrite the original manuscript
 for f in output_folder.glob("*"):
     f.rename(me.content_dir / f.name)
 
 # remove output folder
```

### Comparing `manubot-ai-editor-0.4.2/README.md` & `manubot-ai-editor-0.4.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 # first I create a temporary directory to store the revised manuscript
 output_folder = (Path("tmp") / "manubot-ai-editor-output").resolve()
 shutil.rmtree(output_folder, ignore_errors=True)
 output_folder.mkdir(parents=True, exist_ok=True)
 
 # then I revise the manuscript
-me.revise_manuscript(output_folder, model, debug=True)
+me.revise_manuscript(output_folder, model)
 
 # here I move the revised manuscript back to the content folder
 # CAUTION: this will overwrite the original manuscript
 for f in output_folder.glob("*"):
     f.rename(me.content_dir / f.name)
 
 # remove output folder
```

### Comparing `manubot-ai-editor-0.4.2/libs/manubot_ai_editor/editor.py` & `manubot-ai-editor-0.4.3/libs/manubot_ai_editor/editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,16 +75,16 @@
                 paragraph_text += " ".join(simple_sentences) + suffix
 
         return paragraph_text
 
     @staticmethod
     def revise_and_write_paragraph(
         paragraph: list[str],
-        section_name: str,
         revision_model: ManuscriptRevisionModel,
+        section_name: str = None,
         outfile=None,
     ) -> None | tuple[str, str]:
         """
         Revises and writes a paragraph to the output file.
 
         Arguments:
             paragraph: list of lines of the paragraph.
@@ -330,15 +330,15 @@
                         prev_line = ""
                         while len(paragraph) > 0 and paragraph[-1] == "":
                             paragraph.pop()
                             prev_line += "\n"
 
                     # revise and write paragraph to output file
                     self.revise_and_write_paragraph(
-                        paragraph, section_name, revision_model, outfile
+                        paragraph, revision_model, section_name, outfile
                     )
 
                     # clear the paragraph list
                     if line.strip() == "":
                         outfile.write(line)
                         paragraph = []
                     else:
@@ -371,15 +371,15 @@
 
                 prev_line = line
 
             # If there's any remaining paragraph, process and write it to the
             # output file
             if paragraph:
                 self.revise_and_write_paragraph(
-                    paragraph, section_name, revision_model, outfile
+                    paragraph, revision_model, section_name, outfile
                 )
 
     def revise_manuscript(
         self,
         output_dir: Path | str,
         revision_model: ManuscriptRevisionModel,
         debug: bool = False,
@@ -399,16 +399,22 @@
                     f.strip() for f in filenames_to_revise.split(",")
                 }
                 print(f"File names to revise: {filenames_to_revise}", flush=True)
             else:
                 filenames_to_revise = None
 
         for filename in sorted(self.content_dir.glob("*.md")):
+            # ignore front-matter file
+            if "front-matter" in filename.name:
+                continue
+
             filename_section = self.get_section_from_filename(filename.name)
-            if filename_section is None:
+
+            # we do not process the file if it has no section and there is no custom prompt
+            if filename_section is None and env_vars.CUSTOM_PROMPT not in os.environ:
                 continue
 
             if (
                 filenames_to_revise is not None
                 and filename.name not in filenames_to_revise
             ):
                 continue
```

### Comparing `manubot-ai-editor-0.4.2/libs/manubot_ai_editor/env_vars.py` & `manubot-ai-editor-0.4.3/libs/manubot_ai_editor/env_vars.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 OpenAI model, such as LAGUANGE_MODEL or MAX_TOKENS_PER_REQUEST. For this, see
 more details in https://beta.openai.com/docs/api-reference/completions/create
 """
 
 # OpenAI API key to use
 OPENAI_API_KEY = "OPENAI_API_KEY"
 
-# Language model to use. For example, "text-davinci-003"
+# Language model to use. For example, "text-davinci-003", "gpt-3.5-turbo", "gpt-3.5-turbo-0301", etc
 LANGUAGE_MODEL = "AI_EDITOR_LANGUAGE_MODEL"
 
 # Model parameter: max_tokens
 MAX_TOKENS_PER_REQUEST = "AI_EDITOR_MAX_TOKENS_PER_REQUEST"
 
 # Model parameter: temperature
 TEMPERATURE = "AI_EDITOR_TEMPERATURE"
@@ -49,13 +49,15 @@
 RETRY_COUNT = "AI_EDITOR_RETRY_COUNT"
 
 # If specified, only these file names will be revised. Multiple files can be
 # specified, separated by commas. For example: "01.intro.md,02.review.md"
 FILENAMES_TO_REVISE = "AI_EDITOR_FILENAMES_TO_REVISE"
 
 # It allows to specify a single, custom prompt for all sections. For example:
-# "proofread and revise the following paragraph", where the tool will automatically
-# append the characters ':\n\n' followed by the paragraph at the end of the prompt.
-# Another example is "proofread and revise the following paragraph from the section {section_name} of scientific mauscript:\n\n{paragraph_text}".
+# "proofread and revise the following paragraph"; in this case, the tool will automatically
+# append the characters ':\n\n' followed by the paragraph.
+# It is also possible to include placeholders in the prompt, which will be replaced
+# by the corresponding values. For example, "proofread and revise the following
+# paragraph from the section {section_name} of a scientific manuscript with title '{title}'".
 # The complete list of placeholders is: {paragraph_text}, {section_name},
-# {manuscript_title}, {manuscript_keywords}.
+# {title}, {keywords}.
 CUSTOM_PROMPT = "AI_EDITOR_CUSTOM_PROMPT"
```

### Comparing `manubot-ai-editor-0.4.2/libs/manubot_ai_editor/models.py` & `manubot-ai-editor-0.4.3/libs/manubot_ai_editor/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,15 +249,15 @@
             for key, value in self.model_parameters.items()
             if value is not None
         }
 
         self.several_spaces_pattern = re.compile(r"\s+")
 
     def get_prompt(
-        self, paragraph_text: str, section_name: str
+        self, paragraph_text: str, section_name: str = None
     ) -> str | tuple[str, str]:
         """
         Returns the prompt to be used for the revision of a paragraph that
         belongs to a given section. There are three types of prompts according
         to the section: Abstract, Introduction, Methods, and the rest (i.e.
         Results, Discussion, etc.).
 
@@ -276,15 +276,26 @@
         """
 
         if env_vars.CUSTOM_PROMPT in os.environ:
             prompt = os.environ[env_vars.CUSTOM_PROMPT]
             print(
                 f"Using custom prompt from environment variable '{env_vars.CUSTOM_PROMPT}'"
             )
-            return f"{prompt}:\n\n{paragraph_text}"
+
+            placeholders = {
+                "paragraph_text": paragraph_text,
+                "section_name": section_name,
+                "title": self.title,
+                "keywords": ", ".join(self.keywords),
+            }
+
+            if "{paragraph_text}" not in prompt:
+                prompt += ":\n\n{paragraph_text}"
+
+            return prompt.format(**placeholders)
 
         if section_name in ("abstract",):
             prompt = f"""
                 Revise the following paragraph from the {section_name} of an academic paper (with the title '{self.title}' and keywords '{", ".join(self.keywords)}')
                 so the research problem/question is clear,
                    the solution proposed is clear,
                    the text grammar is correct, spelling errors are fixed,
@@ -326,20 +337,25 @@
                    most references to equations (such as "Equation (@id)") are kept,
                    all equations definitions (such as '{equation_definition}') are included with newlines before and after,
                    the most important symbols in equations are defined,
                    spelling errors are fixed, the text grammar is correct,
                    and the text has a clear sentence structure
             """.strip()
         else:
-            prompt = f"""
-                Revise the following paragraph from the {section_name.capitalize()} section of an academic paper (with the title '{self.title}' and keywords '{", ".join(self.keywords)}')
+            prompt = "Revise the following paragraph"
+
+            if section_name is not None and section_name != "":
+                prompt += f" from the {section_name.capitalize()} section"
+
+            prompt += f" of an academic paper (with title '{self.title}' and keywords '{', '.join(self.keywords)}')"
+            prompt += """
                 so
-                   the text minimizes the use of jargon,
-                   the text grammar is correct, spelling errors are fixed,
-                   and the text has a clear sentence structure
+                    the text minimizes the use of jargon,
+                    the text grammar is correct, spelling errors are fixed,
+                    and the text has a clear sentence structure
             """
 
         prompt = self.several_spaces_pattern.sub(" ", prompt).strip()
 
         if not self.edit_endpoint:
             return f"{prompt}.\n\n{paragraph_text.strip()}"
         else:
@@ -413,15 +429,15 @@
         return {
             "max_context_length": max_context_length,
             "requested_tokens": requested_tokens,
             "tokens_in_prompt": tokens_in_prompt,
             "tokens_in_completion": tokens_in_completion,
         }
 
-    def revise_paragraph(self, paragraph_text, section_name):
+    def revise_paragraph(self, paragraph_text: str, section_name: str = None):
         """
         It revises a paragraph using GPT-3 completion model.
 
         Arguments:
             paragraph_text (str): Paragraph text to revise.
             section_name (str): Section name of the paragraph.
             throw_error (bool): If True, it throws an error if the API call fails.
```

### Comparing `manubot-ai-editor-0.4.2/libs/manubot_ai_editor/utils.py` & `manubot-ai-editor-0.4.3/libs/manubot_ai_editor/utils.py`

 * *Files identical despite different names*

### Comparing `manubot-ai-editor-0.4.2/libs/manubot_ai_editor.egg-info/PKG-INFO` & `manubot-ai-editor-0.4.3/libs/manubot_ai_editor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manubot-ai-editor
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Manubot plugin to revise a manuscript using GPT-3
 Home-page: https://github.com/greenelab/manubot-ai-editor
 Author: Milton Pividori
 Author-email: miltondp@gmail.com
 License: BSD-2-Clause Plus Patent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -55,15 +55,15 @@
 
 # first I create a temporary directory to store the revised manuscript
 output_folder = (Path("tmp") / "manubot-ai-editor-output").resolve()
 shutil.rmtree(output_folder, ignore_errors=True)
 output_folder.mkdir(parents=True, exist_ok=True)
 
 # then I revise the manuscript
-me.revise_manuscript(output_folder, model, debug=True)
+me.revise_manuscript(output_folder, model)
 
 # here I move the revised manuscript back to the content folder
 # CAUTION: this will overwrite the original manuscript
 for f in output_folder.glob("*"):
     f.rename(me.content_dir / f.name)
 
 # remove output folder
```

### Comparing `manubot-ai-editor-0.4.2/setup.py` & `manubot-ai-editor-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # twine upload dist/*
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="manubot-ai-editor",
-    version="0.4.2",
+    version="0.4.3",
     author="Milton Pividori",
     author_email="miltondp@gmail.com",
     description="A Manubot plugin to revise a manuscript using GPT-3",
     license="BSD-2-Clause Plus Patent",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/greenelab/manubot-ai-editor",
```

### Comparing `manubot-ai-editor-0.4.2/tests/test_completion_model.py` & `manubot-ai-editor-0.4.3/tests/test_completion_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,55 +23,14 @@
                 title="Test title",
                 keywords=["test", "keywords"],
             )
     finally:
         os.environ = _environ
 
 
-def test_get_prompt_no_custom_prompt():
-    model = GPT3CompletionModel(
-        title="Test title",
-        keywords=["test", "keywords"],
-    )
-
-    paragraph_text = """
-This is the first sentence.
-And this is the second sentence.
-Finally, the third sentence.
-    """.strip()
-
-    prompt = model.get_prompt(paragraph_text, "introduction")
-    assert prompt.startswith("Revise the following paragraph from the ")
-    assert prompt.endswith(paragraph_text[-20:])
-
-
-@mock.patch.dict(
-    "os.environ",
-    {env_vars.CUSTOM_PROMPT: "proofread and revise the following paragraph"},
-)
-def test_get_prompt_custom_prompt_no_placeholders():
-    model = GPT3CompletionModel(
-        title="Test title",
-        keywords=["test", "keywords"],
-    )
-
-    paragraph_text = """
-This is the first sentence.
-And this is the second sentence.
-Finally, the third sentence.
-    """.strip()
-
-    prompt = model.get_prompt(paragraph_text, "introduction")
-    assert (
-        prompt == f"proofread and revise the following paragraph:\n\n{paragraph_text}"
-    )
-
-    # TODO: add other sections, should return same output
-
-
 @mock.patch.dict("os.environ", {env_vars.OPENAI_API_KEY: "env_var_test_value"})
 def test_model_object_init_with_openai_api_key_as_environment_variable():
     GPT3CompletionModel(
         title="Test title",
         keywords=["test", "keywords"],
     )
 
@@ -354,15 +313,15 @@
     model.keywords = [
         "correlation coefficient",
         "nonlinear relationships",
         "gene expression",
     ]
 
     paragraph_text, paragraph_revised = ManuscriptEditor.revise_and_write_paragraph(
-        paragraph, "abstract", model
+        paragraph, model, "abstract"
     )
     assert paragraph_text is not None
     assert paragraph_revised is not None
     assert isinstance(paragraph_revised, str)
     assert paragraph_revised != paragraph_text
     assert len(paragraph_revised) > 100
     assert "<!--\nERROR:" not in paragraph_revised
@@ -417,15 +376,15 @@
         "gene co-expression",
         "therapeutic targets",
         "drug repurposing",
         "clustering of complex traits",
     ]
 
     paragraph_text, paragraph_revised = ManuscriptEditor.revise_and_write_paragraph(
-        paragraph, "abstract", model
+        paragraph, model, "abstract"
     )
     assert paragraph_text is not None
     assert paragraph_revised is not None
     assert isinstance(paragraph_revised, str)
     assert paragraph_revised != paragraph_text
     assert len(paragraph_revised) > 100
     assert "<!--\nERROR:" not in paragraph_revised
@@ -475,15 +434,15 @@
         "manubot",
         "artificial intelligence",
         "scholarly publishing",
         "software",
     ]
 
     paragraph_text, paragraph_revised = ManuscriptEditor.revise_and_write_paragraph(
-        paragraph, "abstract", model
+        paragraph, model, "abstract"
     )
     assert paragraph_text is not None
     assert paragraph_revised is not None
     assert isinstance(paragraph_revised, str)
     assert paragraph_revised != paragraph_text
     assert len(paragraph_revised) > 100
     assert "<!--\nERROR:" not in paragraph_revised
@@ -536,15 +495,15 @@
     model.keywords = [
         "correlation coefficient",
         "nonlinear relationships",
         "gene expression",
     ]
 
     paragraph_text, paragraph_revised = ManuscriptEditor.revise_and_write_paragraph(
-        paragraph, "introduction", model
+        paragraph, model, "introduction"
     )
     assert paragraph_text is not None
     assert paragraph_revised is not None
     assert isinstance(paragraph_revised, str)
     assert paragraph_revised != paragraph_text
     assert len(paragraph_revised) > 100
     assert "<!--\nERROR:" not in paragraph_revised
@@ -594,15 +553,15 @@
         "gene co-expression",
         "therapeutic targets",
         "drug repurposing",
         "clustering of complex traits",
     ]
 
     paragraph_text, paragraph_revised = ManuscriptEditor.revise_and_write_paragraph(
-        paragraph, "introduction", model
+        paragraph, model, "introduction"
     )
     assert paragraph_text is not None
     assert paragraph_revised is not None
     assert isinstance(paragraph_revised, str)
     assert paragraph_revised != paragraph_text
     assert len(paragraph_revised) > 100
     assert "<!--\nERROR:" not in paragraph_revised
@@ -651,15 +610,15 @@
         "manubot",
         "artificial intelligence",
         "scholarly publishing",
         "software",
     ]
 
     paragraph_text, paragraph_revised = ManuscriptEditor.revise_and_write_paragraph(
-        paragraph, "introduction", model
+        paragraph, model, "introduction"
     )
     assert paragraph_text is not None
     assert paragraph_revised is not None
     assert isinstance(paragraph_revised, str)
     assert paragraph_revised != paragraph_text
     assert len(paragraph_revised) > 25
     assert "<!--\nERROR:" not in paragraph_revised
@@ -708,15 +667,15 @@
     model.keywords = [
         "correlation coefficient",
         "nonlinear relationships",
         "gene expression",
     ]
 
     paragraph_text, paragraph_revised = ManuscriptEditor.revise_and_write_paragraph(
-        paragraph, "results", model
+        paragraph, model, "results"
     )
     assert paragraph_text is not None
     assert paragraph_revised is not None
     assert isinstance(paragraph_revised, str)
     assert paragraph_revised != paragraph_text
     assert len(paragraph_revised) > 100
     assert "<!--\nERROR:" not in paragraph_revised
@@ -763,15 +722,15 @@
         "gene co-expression",
         "therapeutic targets",
         "drug repurposing",
         "clustering of complex traits",
     ]
 
     paragraph_text, paragraph_revised = ManuscriptEditor.revise_and_write_paragraph(
-        paragraph, "results", model
+        paragraph, model, "results"
     )
     assert paragraph_text is not None
     assert paragraph_revised is not None
     assert isinstance(paragraph_revised, str)
     assert paragraph_revised != paragraph_text
     assert len(paragraph_revised) > 100
     assert "<!--\nERROR:" not in paragraph_revised
@@ -820,15 +779,15 @@
     model.keywords = [
         "correlation coefficient",
         "nonlinear relationships",
         "gene expression",
     ]
 
     paragraph_text, paragraph_revised = ManuscriptEditor.revise_and_write_paragraph(
-        paragraph, "results", model
+        paragraph, model, "results"
     )
     assert paragraph_text is not None
     assert paragraph_revised is not None
     assert isinstance(paragraph_revised, str)
     assert paragraph_revised != paragraph_text
 
     # if there is an error, it should return the original paragraph with a header specifying the error
@@ -878,15 +837,15 @@
     model.keywords = [
         "correlation coefficient",
         "nonlinear relationships",
         "gene expression",
     ]
 
     paragraph_text, paragraph_revised = ManuscriptEditor.revise_and_write_paragraph(
-        paragraph, "discussion", model
+        paragraph, model, "discussion"
     )
     assert paragraph_text is not None
     assert paragraph_revised is not None
     assert isinstance(paragraph_revised, str)
     assert paragraph_revised != paragraph_text
     assert len(paragraph_revised) > 100
     assert "<!--\nERROR:" not in paragraph_revised
@@ -935,15 +894,15 @@
         "gene co-expression",
         "therapeutic targets",
         "drug repurposing",
         "clustering of complex traits",
     ]
 
     paragraph_text, paragraph_revised = ManuscriptEditor.revise_and_write_paragraph(
-        paragraph, "discussion", model
+        paragraph, model, "discussion"
     )
     assert paragraph_text is not None
     assert paragraph_revised is not None
     assert isinstance(paragraph_revised, str)
     assert paragraph_revised != paragraph_text
     assert len(paragraph_revised) > 100
     assert "<!--\nERROR:" not in paragraph_revised
@@ -991,15 +950,15 @@
         "manubot",
         "artificial intelligence",
         "scholarly publishing",
         "software",
     ]
 
     paragraph_text, paragraph_revised = ManuscriptEditor.revise_and_write_paragraph(
-        paragraph, "conclusions", model
+        paragraph, model, "conclusions"
     )
     assert paragraph_text is not None
     assert paragraph_revised is not None
     assert isinstance(paragraph_revised, str)
     assert paragraph_revised != paragraph_text
     assert len(paragraph_revised) > 100
     assert "<!--\nERROR:" not in paragraph_revised
@@ -1046,15 +1005,15 @@
     model.keywords = [
         "correlation coefficient",
         "nonlinear relationships",
         "gene expression",
     ]
 
     paragraph_text, paragraph_revised = ManuscriptEditor.revise_and_write_paragraph(
-        paragraph, "methods", model
+        paragraph, model, "methods"
     )
     assert paragraph_text is not None
     assert paragraph_revised is not None
     assert isinstance(paragraph_revised, str)
     assert paragraph_revised != paragraph_text
     assert len(paragraph_revised) > 100
     assert "<!--\nERROR:" not in paragraph_revised
@@ -1101,15 +1060,15 @@
         "gene co-expression",
         "therapeutic targets",
         "drug repurposing",
         "clustering of complex traits",
     ]
 
     paragraph_text, paragraph_revised = ManuscriptEditor.revise_and_write_paragraph(
-        paragraph, "methods", model
+        paragraph, model, "methods"
     )
     assert paragraph_text is not None
     assert paragraph_revised is not None
     assert isinstance(paragraph_revised, str)
     assert paragraph_revised != paragraph_text
     assert len(paragraph_revised) > 100
     assert "<!--\nERROR:" not in paragraph_revised
@@ -1174,15 +1133,15 @@
         "gene co-expression",
         "therapeutic targets",
         "drug repurposing",
         "clustering of complex traits",
     ]
 
     paragraph_text, paragraph_revised = ManuscriptEditor.revise_and_write_paragraph(
-        paragraph, "methods", model
+        paragraph, model, "methods"
     )
     assert paragraph_text is not None
     assert paragraph_revised is not None
     assert isinstance(paragraph_revised, str)
     assert paragraph_revised != paragraph_text
     assert len(paragraph_revised) > 100
     assert "<!--\nERROR:" not in paragraph_revised
@@ -1224,15 +1183,15 @@
         "manubot",
         "artificial intelligence",
         "scholarly publishing",
         "software",
     ]
 
     paragraph_text, paragraph_revised = ManuscriptEditor.revise_and_write_paragraph(
-        paragraph, "methods", model
+        paragraph, model, "methods"
     )
     assert paragraph_text is not None
     assert paragraph_revised is not None
     assert isinstance(paragraph_revised, str)
     assert paragraph_revised != paragraph_text
     assert len(paragraph_revised) > 100
     assert "<!--\nERROR:" not in paragraph_revised
@@ -1327,15 +1286,15 @@
         "gene co-expression",
         "therapeutic targets",
         "drug repurposing",
         "clustering of complex traits",
     ]
 
     paragraph_text, paragraph_revised = ManuscriptEditor.revise_and_write_paragraph(
-        paragraph, "methods", model
+        paragraph, model, "methods"
     )
     assert paragraph_text is not None
     assert paragraph_revised is not None
     assert isinstance(paragraph_revised, str)
     assert paragraph_revised != paragraph_text
     assert len(paragraph_revised) > 100
     assert "<!--\nERROR:" not in paragraph_revised
@@ -1358,15 +1317,15 @@
     )
     paragraph = [sentence.strip() for sentence in paragraph]
     assert len(paragraph) == 1
 
     model = RandomManuscriptRevisionModel()
 
     paragraph_text, paragraph_revised = ManuscriptEditor.revise_and_write_paragraph(
-        paragraph, "methods", model
+        paragraph, model, "methods"
     )
     assert paragraph_text is not None
     assert isinstance(paragraph_text, str)
 
     assert paragraph_revised is not None
     assert isinstance(paragraph_revised, str)
     assert paragraph_revised == paragraph_text
@@ -1385,15 +1344,15 @@
     )
     paragraph = [sentence.strip() for sentence in paragraph]
     assert len(paragraph) == 3
 
     model = RandomManuscriptRevisionModel()
 
     paragraph_text, paragraph_revised = ManuscriptEditor.revise_and_write_paragraph(
-        paragraph, "methods", model
+        paragraph, model, "methods"
     )
     assert paragraph_text is not None
     assert isinstance(paragraph_text, str)
 
     assert paragraph_revised is not None
     assert isinstance(paragraph_revised, str)
     assert paragraph_revised == paragraph_text
```

### Comparing `manubot-ai-editor-0.4.2/tests/test_editor.py` & `manubot-ai-editor-0.4.3/tests/test_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -883,15 +883,15 @@
         "gene co-expression",
         "therapeutic targets",
         "drug repurposing",
         "clustering of complex traits",
     ]
 
     paragraph_text, paragraph_revised = ManuscriptEditor.revise_and_write_paragraph(
-        paragraph, "methods", model
+        paragraph, model, "methods",
     )
     assert paragraph_text is not None
     assert paragraph_revised is not None
     assert isinstance(paragraph_revised, str)
 
     # the paragraph does not contain the "Revised:" or "We revised" initial
     assert orig_paragraph_text.strip() == paragraph_revised.strip()
@@ -986,7 +986,75 @@
     output_folder = tmp_path
     assert output_folder.exists()
 
     me.revise_manuscript(output_folder, model)
 
     output_md_files = list(output_folder.glob("*.md"))
     assert len(output_md_files) == 12
+
+
+@mock.patch.dict(
+    "os.environ",
+    {
+        env_vars.FILENAMES_TO_REVISE: "",
+    },
+)
+@pytest.mark.parametrize(
+    "model",
+    [
+        RandomManuscriptRevisionModel(),
+        # GPT3CompletionModel(None, None),
+    ],
+)
+def test_revise_entire_manuscript_non_standard_filenames_without_custom_prompt(tmp_path, model):
+    # in this case, the list of selected files is empty and files have non standard names,
+    # so none of them are revised
+    print(f"\n{str(tmp_path)}\n")
+
+    me = ManuscriptEditor(
+        content_dir=MANUSCRIPTS_DIR / "ccc_non_standard_filenames",
+    )
+
+    model.title = me.title
+    model.keywords = me.keywords
+
+    output_folder = tmp_path
+    assert output_folder.exists()
+
+    me.revise_manuscript(output_folder, model)
+
+    output_md_files = list(output_folder.glob("*.md"))
+    assert len(output_md_files) == 0
+
+
+@mock.patch.dict(
+    "os.environ",
+    {
+        env_vars.FILENAMES_TO_REVISE: "",
+        env_vars.CUSTOM_PROMPT: "proofread and revise the following paragraph with manuscript title '{title}': {paragraph_text}"
+    },
+)
+@pytest.mark.parametrize(
+    "model",
+    [
+        RandomManuscriptRevisionModel(),
+        # GPT3CompletionModel(None, None),
+    ],
+)
+def test_revise_entire_manuscript_non_standard_filenames_with_custom_prompt(tmp_path, model):
+    # in this case, the list of selected files is empty but there is a custom prompt, so all files are revised
+    print(f"\n{str(tmp_path)}\n")
+
+    me = ManuscriptEditor(
+        content_dir=MANUSCRIPTS_DIR / "ccc_non_standard_filenames",
+    )
+
+    model.title = me.title
+    model.keywords = me.keywords
+
+    output_folder = tmp_path
+    assert output_folder.exists()
+
+    me.revise_manuscript(output_folder, model)
+
+    output_md_files = list(output_folder.glob("*.md"))
+    assert len(output_md_files) == 5
```

