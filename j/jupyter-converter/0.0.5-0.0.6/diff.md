# Comparing `tmp/jupyter_converter-0.0.5-py3-none-any.whl.zip` & `tmp/jupyter_converter-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 11008 bytes, number of entries: 10
+Zip file size: 11166 bytes, number of entries: 10
 -rw-r--r--  2.0 unx       21 b- defN 23-May-27 19:33 jupyter-converter/__init__.py
 -rw-r--r--  2.0 unx     8663 b- defN 23-May-27 19:29 jupyter-converter/cells.py
 -rw-r--r--  2.0 unx     3400 b- defN 23-May-27 19:29 jupyter-converter/converter.py
--rw-r--r--  2.0 unx       45 b- defN 23-May-27 19:59 jupyter_converter/__init__.py
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-01 13:31 jupyter_converter/__init__.py
 -rw-r--r--  2.0 unx     8663 b- defN 23-May-27 19:29 jupyter_converter/cells.py
--rw-r--r--  2.0 unx    12015 b- defN 23-May-27 19:58 jupyter_converter/converter.py
--rw-r--r--  2.0 unx      519 b- defN 23-May-27 19:59 jupyter_converter-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-27 19:59 jupyter_converter-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-May-27 19:59 jupyter_converter-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      846 b- defN 23-May-27 19:59 jupyter_converter-0.0.5.dist-info/RECORD
-10 files, 34282 bytes uncompressed, 9550 bytes compressed:  72.1%
+-rw-r--r--  2.0 unx    13017 b- defN 23-Jun-01 14:36 jupyter_converter/converter.py
+-rw-r--r--  2.0 unx      519 b- defN 23-Jun-01 14:37 jupyter_converter-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 14:37 jupyter_converter-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-Jun-01 14:37 jupyter_converter-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      846 b- defN 23-Jun-01 14:37 jupyter_converter-0.0.6.dist-info/RECORD
+10 files, 35284 bytes uncompressed, 9708 bytes compressed:  72.5%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: jupyter_converter/cells.py
 Comment: 
 
 Filename: jupyter_converter/converter.py
 Comment: 
 
-Filename: jupyter_converter-0.0.5.dist-info/METADATA
+Filename: jupyter_converter-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: jupyter_converter-0.0.5.dist-info/WHEEL
+Filename: jupyter_converter-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: jupyter_converter-0.0.5.dist-info/top_level.txt
+Filename: jupyter_converter-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: jupyter_converter-0.0.5.dist-info/RECORD
+Filename: jupyter_converter-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jupyter_converter/__init__.py

```diff
@@ -1,2 +1,2 @@
-__version__ = '0.0.5'
+__version__ = '0.0.6'
 __all__ = ["converter"]
```

## jupyter_converter/converter.py

```diff
@@ -3,21 +3,23 @@
 import codecs
 import json
 
 
 # 코드 입력 문구 (코드를 삭제하고 출력을 박제하는 Cell)
 code_input_msgs = [
     '# 코드입력',
+    '# 코드 입력',
     '# 코드를 입력하세요.',
     '# 코드를 입력해 주세요',
 ]
 
 # 검증코드 (출력 값을 삭제하지 않음)
 validation_msgs =  [
     '# 검증코드',
+    '# 검증 코드',
     '# 코드 검증',
     '# 코드검증',
 ]
 
 option_msgs = {
     'code': code_input_msgs, 
     'validation': validation_msgs,
@@ -121,24 +123,24 @@
                 if self.use_fixed_code_input_text:
                     self.json_obj['source'][0] = fixed_code_input_text + '\n'
             
         elif 'outputs' in self.json_obj and self.clear_cell_output:
             self.json_obj['outputs'].clear()
             
         # 출력창 처리
-        if self.input_type == 'code' and 'outputs' in self.json_obj and len(self.json_obj['outputs']) > 0:
+        if ((self.input_type == 'code') or (self.input_type == 'validation')) and 'outputs' in self.json_obj and len(self.json_obj['outputs']) > 0:
             if 'data' in self.json_obj['outputs'][0]:
                 # Series, DataFrame 출력
                 # data = self.json_obj['outputs'][0]['data']
                 for output_ in self.json_obj['outputs']:
                     data = output_['data']
                     if 'text/html' in data:
                         # DataFrame 출력
                         html = data['text/html']
-                        html.insert(0, '<p><strong>[출력 결과]</strong></p>')
+                        html.insert(0, '<p><strong style="background-color: #FCEAE2;  padding: 0.25rem; border-radius: 2px;">[ 출력 ]</strong></p>')
                         replaced_html = []
                         for row in html:
                             row = row.replace(r'<div>', r'<div class="output_subarea output_html rendered_html output_result">')
                             row = row.replace(r'class="dataframe"', r'class="dataframe" style="margin-left: 0; margin-right: 0;"')
                             replaced_html.append(row)
                         
                         self.outputs = replaced_html
@@ -150,51 +152,47 @@
                         plain_text = data['text/plain']
                         if len(plain_text) > 0 and plain_text[0].startswith('<Figure'):
                             self.outputs = None
                             # continue
                         else:
                             plain_text[0] = '<pre>' + plain_text[0]
                             plain_text[len(plain_text)-1] = plain_text[len(plain_text)-1] + '</pre>'
-                            plain_text.insert(0, '<p><strong>[출력 결과]</strong></p>')
+                            plain_text.insert(0, '<p><strong style="background-color: #FCEAE2;  padding: 0.25rem; border-radius: 2px;">[ 출력 ]</strong></p>')
                             self.outputs = plain_text
                             
                     if 'image/png' in data:
                         # print('IMAGE FOUND!!')
                         # pyplot 그래프
                         plain_image = data['image/png']
                         plain_image = '<img style="margin-left: 0; margin-right: 0;" src="data:image/png;base64,' + plain_image.replace('\n','') + '"/>'
                         self.outputs = []
-                        self.outputs.insert(0, '<p><strong>[출력 결과]</strong></p>')
+                        self.outputs.insert(0, '<p><strong style="background-color: #FCEAE2;  padding: 0.25rem; border-radius: 2px;">[ 출력 ]</strong></p>')
                         self.outputs.append(plain_image)
                         break
                     
             elif 'text' in self.json_obj['outputs'][0]:
                 # Series 형태의 TEXT output
                 text = self.json_obj['outputs'][0]['text']
                 if len(text) > 0 and text[0].startswith('<Figure'):
                     self.outputs = None
                 else:
                     text[0] = '<pre>' + text[0]
                     text[len(text)-1] = text[len(text)-1] + '</pre>'
-                    text.insert(0, '<p><strong>[출력 결과]</strong></p>')
+                    text.insert(0, '<p><strong style="background-color: #FCEAE2;  padding: 0.25rem; border-radius: 2px;">[ 출력 ]</strong></p>')
                     self.outputs = text
     
     def create_answer_output(self):
         if self.answer_code is not None:
             answer_output = [
-                '<details>\n',
-                '<summary>\n',
-                '<b>▼ [정답 확인] ▼</b>\n',
+                '<details style="border: 1px solid #ababab; border-radius: 2px;">\n',
+                '<summary style="font-weight: bold; padding: 0.25em; display:list-item; background-color: #FCEAE2; color: #000;">\n',
+                '<b>[ 정답 ]</b>\n',
                 '</summary>\n',
                 '<div class="markdown">\n',
-                '<span><pre><code>',
-                # import pandas as pd
-
-            # pd.read_csv('data.csv')
-                
+                '<span><pre><code>',                
             ]
             answer_output.extend(self.answer_code)
             answer_output.append('\n</code></pre></span></div></details>\n',)
             return answer_output
         else:
             return None
         
@@ -273,14 +271,27 @@
                 # 정답 출력이 존재하는 경우 (추가 Cell 생성)
                 answer_output = cell.create_answer_output()    
                 if answer_output is not None:
                     answer_output_cell = {'cell_type': 'markdown', 
                             'metadata': {},
                             'source': answer_output}
                     processed_cells.append(answer_output_cell)
+                    
+        elif cell.input_type == 'validation':
+            # 검증 코드셀에 대한 출력 값 처리
+            if cell.outputs is not None and len(cell.outputs) > 0:
+                output_cell = {'cell_type': 'markdown', 
+                            'metadata': {},
+                            'source': cell.outputs}
+                c = copy.deepcopy(cell())
+                if 'outputs' in c:
+                    c['outputs'] = []
+                processed_cells.append(c)
+                processed_cells.append(output_cell)
+                
         elif cell.input_type == 'markdown':
             # 출력 값이 없는 코드셀인 경우
             processed_cells.append(cell())  
         else:
             processed_cells.append(cell())  
             
     y['cells'] = processed_cells
```

## Comparing `jupyter_converter-0.0.5.dist-info/METADATA` & `jupyter_converter-0.0.6.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-converter
-Version: 0.0.5
+Version: 0.0.6
 Summary: Jupyter Notebook exam generator written by TeddyNote
 Home-page: https://github.com/teddylee777
 Author: teddylee777
 Author-email: teddylee777@gmail.com
 Keywords: teddynote,teddylee777,jupyter notebook converter,exam generator
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

