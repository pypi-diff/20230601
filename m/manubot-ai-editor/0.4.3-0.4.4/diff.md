# Comparing `tmp/manubot-ai-editor-0.4.3.tar.gz` & `tmp/manubot-ai-editor-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manubot-ai-editor-0.4.3.tar", last modified: Thu Jun  1 19:40:02 2023, max compression
+gzip compressed data, was "manubot-ai-editor-0.4.4.tar", last modified: Thu Jun  1 19:58:35 2023, max compression
```

## Comparing `manubot-ai-editor-0.4.3.tar` & `manubot-ai-editor-0.4.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-01 19:40:02.974068 manubot-ai-editor-0.4.3/
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2544 2023-06-01 19:40:02.974068 manubot-ai-editor-0.4.3/PKG-INFO
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2062 2023-06-01 16:26:59.000000 manubot-ai-editor-0.4.3/README.md
-drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-01 19:40:02.974068 manubot-ai-editor-0.4.3/libs/
-drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-01 19:40:02.974068 manubot-ai-editor-0.4.3/libs/manubot_ai_editor/
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)        0 2023-01-26 21:56:19.000000 manubot-ai-editor-0.4.3/libs/manubot_ai_editor/__init__.py
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    16783 2023-06-01 19:27:16.000000 manubot-ai-editor-0.4.3/libs/manubot_ai_editor/editor.py
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2965 2023-06-01 19:38:16.000000 manubot-ai-editor-0.4.3/libs/manubot_ai_editor/env_vars.py
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    20582 2023-06-01 16:43:05.000000 manubot-ai-editor-0.4.3/libs/manubot_ai_editor/models.py
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)      632 2023-01-26 21:56:19.000000 manubot-ai-editor-0.4.3/libs/manubot_ai_editor/utils.py
-drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-01 19:40:02.974068 manubot-ai-editor-0.4.3/libs/manubot_ai_editor.egg-info/
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2544 2023-06-01 19:40:02.000000 manubot-ai-editor-0.4.3/libs/manubot_ai_editor.egg-info/PKG-INFO
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)      498 2023-06-01 19:40:02.000000 manubot-ai-editor-0.4.3/libs/manubot_ai_editor.egg-info/SOURCES.txt
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)        1 2023-06-01 19:40:02.000000 manubot-ai-editor-0.4.3/libs/manubot_ai_editor.egg-info/dependency_links.txt
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)       20 2023-06-01 19:40:02.000000 manubot-ai-editor-0.4.3/libs/manubot_ai_editor.egg-info/requires.txt
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)       19 2023-06-01 19:40:02.000000 manubot-ai-editor-0.4.3/libs/manubot_ai_editor.egg-info/top_level.txt
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)       38 2023-06-01 19:40:02.974068 manubot-ai-editor-0.4.3/setup.cfg
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)      938 2023-06-01 19:08:33.000000 manubot-ai-editor-0.4.3/setup.py
-drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-01 19:40:02.974068 manubot-ai-editor-0.4.3/tests/
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    61034 2023-06-01 15:22:56.000000 manubot-ai-editor-0.4.3/tests/test_completion_model.py
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    40588 2023-06-01 16:32:37.000000 manubot-ai-editor-0.4.3/tests/test_editor.py
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     7738 2023-06-01 16:46:08.000000 manubot-ai-editor-0.4.3/tests/test_model_get_prompt.py
+drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-01 19:58:35.896522 manubot-ai-editor-0.4.4/
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2544 2023-06-01 19:58:35.896522 manubot-ai-editor-0.4.4/PKG-INFO
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2062 2023-06-01 16:26:59.000000 manubot-ai-editor-0.4.4/README.md
+drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-01 19:58:35.896522 manubot-ai-editor-0.4.4/libs/
+drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-01 19:58:35.896522 manubot-ai-editor-0.4.4/libs/manubot_ai_editor/
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)        0 2023-01-26 21:56:19.000000 manubot-ai-editor-0.4.4/libs/manubot_ai_editor/__init__.py
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    16883 2023-06-01 19:57:14.000000 manubot-ai-editor-0.4.4/libs/manubot_ai_editor/editor.py
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2965 2023-06-01 19:38:16.000000 manubot-ai-editor-0.4.4/libs/manubot_ai_editor/env_vars.py
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    20582 2023-06-01 16:43:05.000000 manubot-ai-editor-0.4.4/libs/manubot_ai_editor/models.py
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)      632 2023-01-26 21:56:19.000000 manubot-ai-editor-0.4.4/libs/manubot_ai_editor/utils.py
+drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-01 19:58:35.896522 manubot-ai-editor-0.4.4/libs/manubot_ai_editor.egg-info/
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2544 2023-06-01 19:58:35.000000 manubot-ai-editor-0.4.4/libs/manubot_ai_editor.egg-info/PKG-INFO
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)      498 2023-06-01 19:58:35.000000 manubot-ai-editor-0.4.4/libs/manubot_ai_editor.egg-info/SOURCES.txt
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)        1 2023-06-01 19:58:35.000000 manubot-ai-editor-0.4.4/libs/manubot_ai_editor.egg-info/dependency_links.txt
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)       20 2023-06-01 19:58:35.000000 manubot-ai-editor-0.4.4/libs/manubot_ai_editor.egg-info/requires.txt
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)       19 2023-06-01 19:58:35.000000 manubot-ai-editor-0.4.4/libs/manubot_ai_editor.egg-info/top_level.txt
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)       38 2023-06-01 19:58:35.896522 manubot-ai-editor-0.4.4/setup.cfg
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)      938 2023-06-01 19:58:06.000000 manubot-ai-editor-0.4.4/setup.py
+drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-01 19:58:35.896522 manubot-ai-editor-0.4.4/tests/
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    61034 2023-06-01 15:22:56.000000 manubot-ai-editor-0.4.4/tests/test_completion_model.py
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    41575 2023-06-01 19:57:26.000000 manubot-ai-editor-0.4.4/tests/test_editor.py
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     7738 2023-06-01 16:46:08.000000 manubot-ai-editor-0.4.4/tests/test_model_get_prompt.py
```

### Comparing `manubot-ai-editor-0.4.3/PKG-INFO` & `manubot-ai-editor-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manubot-ai-editor
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Manubot plugin to revise a manuscript using GPT-3
 Home-page: https://github.com/greenelab/manubot-ai-editor
 Author: Milton Pividori
 Author-email: miltondp@gmail.com
 License: BSD-2-Clause Plus Patent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `manubot-ai-editor-0.4.3/README.md` & `manubot-ai-editor-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `manubot-ai-editor-0.4.3/libs/manubot_ai_editor/editor.py` & `manubot-ai-editor-0.4.4/libs/manubot_ai_editor/editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -406,15 +406,18 @@
             # ignore front-matter file
             if "front-matter" in filename.name:
                 continue
 
             filename_section = self.get_section_from_filename(filename.name)
 
             # we do not process the file if it has no section and there is no custom prompt
-            if filename_section is None and env_vars.CUSTOM_PROMPT not in os.environ:
+            if filename_section is None and (
+                env_vars.CUSTOM_PROMPT not in os.environ
+                or os.environ[env_vars.CUSTOM_PROMPT].strip() == ""
+            ):
                 continue
 
             if (
                 filenames_to_revise is not None
                 and filename.name not in filenames_to_revise
             ):
                 continue
```

### Comparing `manubot-ai-editor-0.4.3/libs/manubot_ai_editor/env_vars.py` & `manubot-ai-editor-0.4.4/libs/manubot_ai_editor/env_vars.py`

 * *Files identical despite different names*

### Comparing `manubot-ai-editor-0.4.3/libs/manubot_ai_editor/models.py` & `manubot-ai-editor-0.4.4/libs/manubot_ai_editor/models.py`

 * *Files identical despite different names*

### Comparing `manubot-ai-editor-0.4.3/libs/manubot_ai_editor/utils.py` & `manubot-ai-editor-0.4.4/libs/manubot_ai_editor/utils.py`

 * *Files identical despite different names*

### Comparing `manubot-ai-editor-0.4.3/libs/manubot_ai_editor.egg-info/PKG-INFO` & `manubot-ai-editor-0.4.4/libs/manubot_ai_editor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manubot-ai-editor
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Manubot plugin to revise a manuscript using GPT-3
 Home-page: https://github.com/greenelab/manubot-ai-editor
 Author: Milton Pividori
 Author-email: miltondp@gmail.com
 License: BSD-2-Clause Plus Patent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `manubot-ai-editor-0.4.3/setup.py` & `manubot-ai-editor-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # twine upload dist/*
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="manubot-ai-editor",
-    version="0.4.3",
+    version="0.4.4",
     author="Milton Pividori",
     author_email="miltondp@gmail.com",
     description="A Manubot plugin to revise a manuscript using GPT-3",
     license="BSD-2-Clause Plus Patent",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/greenelab/manubot-ai-editor",
```

### Comparing `manubot-ai-editor-0.4.3/tests/test_completion_model.py` & `manubot-ai-editor-0.4.4/tests/test_completion_model.py`

 * *Files identical despite different names*

### Comparing `manubot-ai-editor-0.4.3/tests/test_editor.py` & `manubot-ai-editor-0.4.4/tests/test_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -883,15 +883,17 @@
         "gene co-expression",
         "therapeutic targets",
         "drug repurposing",
         "clustering of complex traits",
     ]
 
     paragraph_text, paragraph_revised = ManuscriptEditor.revise_and_write_paragraph(
-        paragraph, model, "methods",
+        paragraph,
+        model,
+        "methods",
     )
     assert paragraph_text is not None
     assert paragraph_revised is not None
     assert isinstance(paragraph_revised, str)
 
     # the paragraph does not contain the "Revised:" or "We revised" initial
     assert orig_paragraph_text.strip() == paragraph_revised.strip()
@@ -1001,15 +1003,17 @@
 @pytest.mark.parametrize(
     "model",
     [
         RandomManuscriptRevisionModel(),
         # GPT3CompletionModel(None, None),
     ],
 )
-def test_revise_entire_manuscript_non_standard_filenames_without_custom_prompt(tmp_path, model):
+def test_revise_entire_manuscript_non_standard_filenames_without_custom_prompt(
+    tmp_path, model
+):
     # in this case, the list of selected files is empty and files have non standard names,
     # so none of them are revised
     print(f"\n{str(tmp_path)}\n")
 
     me = ManuscriptEditor(
         content_dir=MANUSCRIPTS_DIR / "ccc_non_standard_filenames",
     )
@@ -1026,25 +1030,27 @@
     assert len(output_md_files) == 0
 
 
 @mock.patch.dict(
     "os.environ",
     {
         env_vars.FILENAMES_TO_REVISE: "",
-        env_vars.CUSTOM_PROMPT: "proofread and revise the following paragraph with manuscript title '{title}': {paragraph_text}"
+        env_vars.CUSTOM_PROMPT: "proofread and revise the following paragraph with manuscript title '{title}': {paragraph_text}",
     },
 )
 @pytest.mark.parametrize(
     "model",
     [
         RandomManuscriptRevisionModel(),
         # GPT3CompletionModel(None, None),
     ],
 )
-def test_revise_entire_manuscript_non_standard_filenames_with_custom_prompt(tmp_path, model):
+def test_revise_entire_manuscript_non_standard_filenames_with_custom_prompt(
+    tmp_path, model
+):
     # in this case, the list of selected files is empty but there is a custom prompt, so all files are revised
     print(f"\n{str(tmp_path)}\n")
 
     me = ManuscriptEditor(
         content_dir=MANUSCRIPTS_DIR / "ccc_non_standard_filenames",
     )
 
@@ -1054,7 +1060,41 @@
     output_folder = tmp_path
     assert output_folder.exists()
 
     me.revise_manuscript(output_folder, model)
 
     output_md_files = list(output_folder.glob("*.md"))
     assert len(output_md_files) == 5
+
+
+@mock.patch.dict(
+    "os.environ",
+    {env_vars.FILENAMES_TO_REVISE: "", env_vars.CUSTOM_PROMPT: ""},
+)
+@pytest.mark.parametrize(
+    "model",
+    [
+        RandomManuscriptRevisionModel(),
+        # GPT3CompletionModel(None, None),
+    ],
+)
+def test_revise_entire_manuscript_non_standard_filenames_with_empty_custom_prompt(
+    tmp_path, model
+):
+    # in this case, the list of selected files is empty and the custom prompt env variable is there but it's empty,
+    # this use case is when the custom prompt is not provided in the workflow interface
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
```

### Comparing `manubot-ai-editor-0.4.3/tests/test_model_get_prompt.py` & `manubot-ai-editor-0.4.4/tests/test_model_get_prompt.py`

 * *Files identical despite different names*

