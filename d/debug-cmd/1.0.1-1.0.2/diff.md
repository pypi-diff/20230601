# Comparing `tmp/debug_cmd-1.0.1-py3-none-any.whl.zip` & `tmp/debug_cmd-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5801 bytes, number of entries: 8
+Zip file size: 5954 bytes, number of entries: 8
 -rw-r--r--  2.0 unx        0 b- defN 23-May-31 11:25 debug_cmd/__init__.py
--rw-r--r--  2.0 unx     8346 b- defN 23-May-31 14:37 debug_cmd/debug_cmd.py
--rw-r--r--  2.0 unx     1071 b- defN 23-May-31 14:43 debug_cmd-1.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      762 b- defN 23-May-31 14:43 debug_cmd-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-31 14:43 debug_cmd-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       55 b- defN 23-May-31 14:43 debug_cmd-1.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-May-31 14:43 debug_cmd-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      646 b- defN 23-May-31 14:43 debug_cmd-1.0.1.dist-info/RECORD
-8 files, 10982 bytes uncompressed, 4663 bytes compressed:  57.5%
+-rw-r--r--  2.0 unx     8765 b- defN 23-Jun-01 00:53 debug_cmd/debug_cmd.py
+-rw-r--r--  2.0 unx     1071 b- defN 23-Jun-01 00:56 debug_cmd-1.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      762 b- defN 23-Jun-01 00:56 debug_cmd-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 00:56 debug_cmd-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-01 00:56 debug_cmd-1.0.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-01 00:56 debug_cmd-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      646 b- defN 23-Jun-01 00:56 debug_cmd-1.0.2.dist-info/RECORD
+8 files, 11401 bytes uncompressed, 4816 bytes compressed:  57.8%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: debug_cmd/__init__.py
 Comment: 
 
 Filename: debug_cmd/debug_cmd.py
 Comment: 
 
-Filename: debug_cmd-1.0.1.dist-info/LICENSE
+Filename: debug_cmd-1.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: debug_cmd-1.0.1.dist-info/METADATA
+Filename: debug_cmd-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: debug_cmd-1.0.1.dist-info/WHEEL
+Filename: debug_cmd-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: debug_cmd-1.0.1.dist-info/entry_points.txt
+Filename: debug_cmd-1.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: debug_cmd-1.0.1.dist-info/top_level.txt
+Filename: debug_cmd-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: debug_cmd-1.0.1.dist-info/RECORD
+Filename: debug_cmd-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## debug_cmd/debug_cmd.py

```diff
@@ -46,15 +46,15 @@
     if return_code == 0 and not force:
         print('\n-------- コマンドは成功しました --------')
         return
 
     # ask llm about error.
     print('\n-------- エラー原因を解析中 --------')
     cmd_str = ' '.join(commands) if type(commands) is list else commands
-    answer = _ask_llm_about_error(cmd=cmd_str, error_message=cmd_out)
+    answer = _ask_llm_about_error(cmd=cmd_str, return_code=return_code, error_message=cmd_out)
     print(answer)
 
 
 def _assert_environment_variables() -> None:
     """
     ensure essential environment variables.
     """
@@ -125,25 +125,26 @@
 
         if not line and proc.poll() is not None:
             break
 
         yield line.decode(_CLI_ENCODING)
 
 
-def _ask_llm_about_error(cmd: str, error_message: str) -> str:
+def _ask_llm_about_error(cmd: str, return_code: int, error_message: str) -> str:
     """
     :param str cmd: command line arguments.
+    :param int return_code: return code.
     :param str error_message: error message.
     :return: an answer.
     """
     # split error message.
     docs = _split_error_message(error_message)
 
     # create a prompt.
-    query_text = _get_question(cmd)
+    query_text = _get_question(cmd, return_code)
 
     # using refine.
     question_prompt = _get_prompt_template(query_text)
     refine_prompt = _get_refine_template(query_text)
     chain = load_summarize_chain(_LLM, chain_type="refine", question_prompt=question_prompt, refine_prompt=refine_prompt)  # nopep8
 
     return chain.run(docs)
@@ -164,23 +165,33 @@
     )
     texts = text_splitter.split_text(error_message)
     documents = [Document(page_content=t) for t in texts]
 
     return documents
 
 
-def _get_question(cmd: str) -> str:
+def _get_question(cmd: str, return_code: int) -> str:
     """
     :param cmd: command line arguments.
+    :param return_code: return code.
     :return: llm prompt.
     """
+    arch = platform.machine()
+    cwd = os.getcwd()
+    env_str = ','.join(os.environ.keys())
+
     return (
-        'あなたは Mac, Unix, Linux のターミナル上で発生したコマンドのエラーの解消を手助けする AI アシスタントです\n'
-        f'質問者が使っているパソコンの OS名, OSバージョン: {_get_os()}\n'
-        f'質問者のパソコンでエラーが発生したコマンド: {cmd}\n'
+        'あなたは Mac, Unix, Linux のターミナル上で発生したコマンドのエラーの解消を手助けする AI アシスタントです。'
+        '質問者が使っているパソコンの情報は次の通りです。\n'
+        f'エラーが発生したコマンド: {cmd}\n'
+        f'コマンドの終了コード: {return_code}\n'
+        f'OS名, OSバージョン: {_get_os()}\n'
+        f'CPUアーキテクチャ: {arch}\n'
+        f'カレントディレクトリ: {cwd}\n'
+        f'環境変数: {env_str}\n'
         'これらの情報と与えられたエラーメッセージを元に、エラーの原因とその解決策を示して下さい: '
     )
 
 
 def _get_prompt_template(query_str: str) -> PromptTemplate:
     """
     Create new prompt template in japanese.
@@ -251,13 +262,12 @@
     """
     os_name = platform.system()
     os_version = platform.version()
 
     if os_name != 'Darwin':
         return f'{os_name} {os_version}'
 
-    mac_ver, _, arch = platform.mac_ver()
-    return f'macOS {mac_ver} ({arch})'
+    return f'macOS {platform.mac_ver()[0]}'
 
 
 if __name__ == '__main__':
     main()
```

## Comparing `debug_cmd-1.0.1.dist-info/LICENSE` & `debug_cmd-1.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `debug_cmd-1.0.1.dist-info/METADATA` & `debug_cmd-1.0.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debug-cmd
-Version: 1.0.1
+Version: 1.0.2
 Summary: Debug linux command error by using GPT/LLM.
 Home-page: https://github.com/megmogmog1965/debug_cmd
 Author: Yusuke Kawatsu
 Author-email: mail@sample.com
 License: MIT
 Keywords: gpt debug
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `debug_cmd-1.0.1.dist-info/RECORD` & `debug_cmd-1.0.2.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 debug_cmd/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-debug_cmd/debug_cmd.py,sha256=GnL9lCrZqX7zn980CNqF6o4YEYGhy-8-11nJ5Fzr9XA,8346
-debug_cmd-1.0.1.dist-info/LICENSE,sha256=u8EpYn6Vw79WHlICc-rMtlgUrA-0AcSlcF94AJD0FB0,1071
-debug_cmd-1.0.1.dist-info/METADATA,sha256=3UuAh65m7IRUpPCeWW6kPBJG3ZbYf8-jCz-8ZRGHCh4,762
-debug_cmd-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-debug_cmd-1.0.1.dist-info/entry_points.txt,sha256=OpigP5xJALw-yWnPmoncGyEYycqqPHPbTynH5GEWcvs,55
-debug_cmd-1.0.1.dist-info/top_level.txt,sha256=8XGxPpLiDBklKXrkfYGxBz7GGXCtB7NT_VfjI2SJBoI,10
-debug_cmd-1.0.1.dist-info/RECORD,,
+debug_cmd/debug_cmd.py,sha256=rUtc55t8r1VxL7CwC8g_dvjFOB9nBahNkZvsIqKjPBk,8765
+debug_cmd-1.0.2.dist-info/LICENSE,sha256=u8EpYn6Vw79WHlICc-rMtlgUrA-0AcSlcF94AJD0FB0,1071
+debug_cmd-1.0.2.dist-info/METADATA,sha256=esRLcMHdNELCUJlnL2OINh4DiUnv81tU2btBHPhnEF8,762
+debug_cmd-1.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+debug_cmd-1.0.2.dist-info/entry_points.txt,sha256=OpigP5xJALw-yWnPmoncGyEYycqqPHPbTynH5GEWcvs,55
+debug_cmd-1.0.2.dist-info/top_level.txt,sha256=8XGxPpLiDBklKXrkfYGxBz7GGXCtB7NT_VfjI2SJBoI,10
+debug_cmd-1.0.2.dist-info/RECORD,,
```

