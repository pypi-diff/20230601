# Comparing `tmp/miniscutil-0.2.4.tar.gz` & `tmp/miniscutil-0.2.5.tar.gz`

## Comparing `miniscutil-0.2.4.tar` & `miniscutil-0.2.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/__about__.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/__init__.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/adapt.py
--rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/asyncio_helpers.py
--rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/config.py
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/current.py
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/deep.py
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/deepeq.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/dictdiff.py
--rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/dispatch.py
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/misc.py
--rw-r--r--   0        0        0    13850 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/ofdict.py
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/sum.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/type_util.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/lsp/README.md
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/lsp/__init__.py
--rw-r--r--   0        0        0     7224 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/lsp/document.py
--rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/lsp/server.py
--rw-r--r--   0        0        0    12751 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/lsp/types.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/rpc/__init__.py
--rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/rpc/extrarpc.py
--rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/rpc/io_transport.py
--rw-r--r--   0        0        0    19268 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/rpc/jsonrpc.py
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/rpc/starlette_ws_transport.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/rpc/transport.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/rpc/websocket_transport.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 miniscutil-0.2.4/tests/__init__.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 miniscutil-0.2.4/tests/test_classdispatch.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 miniscutil-0.2.4/tests/test_config.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 miniscutil-0.2.4/tests/test_current.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 miniscutil-0.2.4/tests/test_deepeq.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 miniscutil-0.2.4/tests/test_humansize.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 miniscutil-0.2.4/tests/test_lsp.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 miniscutil-0.2.4/tests/test_ofdict.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 miniscutil-0.2.4/tests/test_typing.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 miniscutil-0.2.4/tests/test_util.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 miniscutil-0.2.4/tests/snapshots/test_humansize/test_human_size/bytes
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 miniscutil-0.2.4/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 miniscutil-0.2.4/LICENSE.txt
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 miniscutil-0.2.4/README.md
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 miniscutil-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 miniscutil-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 miniscutil-0.2.5/miniscutil/__about__.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 miniscutil-0.2.5/miniscutil/__init__.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 miniscutil-0.2.5/miniscutil/adapt.py
+-rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 miniscutil-0.2.5/miniscutil/asyncio_helpers.py
+-rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 miniscutil-0.2.5/miniscutil/config.py
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 miniscutil-0.2.5/miniscutil/current.py
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 miniscutil-0.2.5/miniscutil/deep.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 miniscutil-0.2.5/miniscutil/deepeq.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 miniscutil-0.2.5/miniscutil/dictdiff.py
+-rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 miniscutil-0.2.5/miniscutil/dispatch.py
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 miniscutil-0.2.5/miniscutil/misc.py
+-rw-r--r--   0        0        0    13850 2020-02-02 00:00:00.000000 miniscutil-0.2.5/miniscutil/ofdict.py
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 miniscutil-0.2.5/miniscutil/sum.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 miniscutil-0.2.5/miniscutil/type_util.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 miniscutil-0.2.5/miniscutil/lsp/README.md
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 miniscutil-0.2.5/miniscutil/lsp/__init__.py
+-rw-r--r--   0        0        0     7291 2020-02-02 00:00:00.000000 miniscutil-0.2.5/miniscutil/lsp/document.py
+-rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 miniscutil-0.2.5/miniscutil/lsp/server.py
+-rw-r--r--   0        0        0    12751 2020-02-02 00:00:00.000000 miniscutil-0.2.5/miniscutil/lsp/types.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 miniscutil-0.2.5/miniscutil/rpc/__init__.py
+-rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 miniscutil-0.2.5/miniscutil/rpc/extrarpc.py
+-rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 miniscutil-0.2.5/miniscutil/rpc/io_transport.py
+-rw-r--r--   0        0        0    19268 2020-02-02 00:00:00.000000 miniscutil-0.2.5/miniscutil/rpc/jsonrpc.py
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 miniscutil-0.2.5/miniscutil/rpc/starlette_ws_transport.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 miniscutil-0.2.5/miniscutil/rpc/transport.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 miniscutil-0.2.5/miniscutil/rpc/websocket_transport.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 miniscutil-0.2.5/tests/__init__.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 miniscutil-0.2.5/tests/test_classdispatch.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 miniscutil-0.2.5/tests/test_config.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 miniscutil-0.2.5/tests/test_current.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 miniscutil-0.2.5/tests/test_deepeq.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 miniscutil-0.2.5/tests/test_humansize.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 miniscutil-0.2.5/tests/test_lsp.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 miniscutil-0.2.5/tests/test_ofdict.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 miniscutil-0.2.5/tests/test_typing.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 miniscutil-0.2.5/tests/test_util.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 miniscutil-0.2.5/tests/snapshots/test_humansize/test_human_size/bytes
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 miniscutil-0.2.5/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 miniscutil-0.2.5/LICENSE.txt
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 miniscutil-0.2.5/README.md
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 miniscutil-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 miniscutil-0.2.5/PKG-INFO
```

### Comparing `miniscutil-0.2.4/miniscutil/__init__.py` & `miniscutil-0.2.5/miniscutil/__init__.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.4/miniscutil/adapt.py` & `miniscutil-0.2.5/miniscutil/adapt.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.4/miniscutil/asyncio_helpers.py` & `miniscutil-0.2.5/miniscutil/asyncio_helpers.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.4/miniscutil/config.py` & `miniscutil-0.2.5/miniscutil/config.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.4/miniscutil/current.py` & `miniscutil-0.2.5/miniscutil/current.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.4/miniscutil/deep.py` & `miniscutil-0.2.5/miniscutil/deep.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.4/miniscutil/deepeq.py` & `miniscutil-0.2.5/miniscutil/deepeq.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.4/miniscutil/dispatch.py` & `miniscutil-0.2.5/miniscutil/dispatch.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.4/miniscutil/misc.py` & `miniscutil-0.2.5/miniscutil/misc.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.4/miniscutil/ofdict.py` & `miniscutil-0.2.5/miniscutil/ofdict.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.4/miniscutil/sum.py` & `miniscutil-0.2.5/miniscutil/sum.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.4/miniscutil/type_util.py` & `miniscutil-0.2.5/miniscutil/type_util.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.4/miniscutil/lsp/document.py` & `miniscutil-0.2.5/miniscutil/lsp/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,20 +53,20 @@
     @classmethod
     def of_offset(cls, offset: int):
         return document_context.get().offset_to_position(offset)
 
     def to_offset(self):
         return document_context.get().position_to_offset(self)
 
-    def __add__(self, offset: Union[int, tuple[int, int]]):
+    def __add__(self, offset: Union[int, tuple[int, int]]) -> "Position":
         if isinstance(offset, int):
             return document_context.get().add_position(self, offset)
         elif isinstance(offset, tuple):
             line, col = offset
-            return replace(self, self.line + line, self.character + col)
+            return replace(self, line=self.line + line, character=self.character + col)
         else:
             raise TypeError(
                 f"unsupported operand type(s) for +: 'Position' and '{type(offset)}'"
             )
 
     def __le__(self, other: "Position"):
         assert isinstance(other, Position)
@@ -227,14 +227,16 @@
 
     def range_to_offsets(self, range: Range) -> tuple[int, int]:
         return (
             self.position_to_offset(range.start),
             self.position_to_offset(range.end),
         )
 
+    # [todo] enter, exit does setdoc
+
 
 @dataclass
 class TextDocumentItem(DocumentContext):
     uri: DocumentUri
     languageId: str
     version: int
```

### Comparing `miniscutil-0.2.4/miniscutil/lsp/server.py` & `miniscutil-0.2.5/miniscutil/lsp/server.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.4/miniscutil/lsp/types.py` & `miniscutil-0.2.5/miniscutil/lsp/types.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.4/miniscutil/rpc/extrarpc.py` & `miniscutil-0.2.5/miniscutil/rpc/extrarpc.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.4/miniscutil/rpc/io_transport.py` & `miniscutil-0.2.5/miniscutil/rpc/io_transport.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.4/miniscutil/rpc/jsonrpc.py` & `miniscutil-0.2.5/miniscutil/rpc/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.4/miniscutil/rpc/starlette_ws_transport.py` & `miniscutil-0.2.5/miniscutil/rpc/starlette_ws_transport.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.4/miniscutil/rpc/transport.py` & `miniscutil-0.2.5/miniscutil/rpc/transport.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.4/miniscutil/rpc/websocket_transport.py` & `miniscutil-0.2.5/miniscutil/rpc/websocket_transport.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.4/tests/test_classdispatch.py` & `miniscutil-0.2.5/tests/test_classdispatch.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.4/tests/test_config.py` & `miniscutil-0.2.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.4/tests/test_current.py` & `miniscutil-0.2.5/tests/test_current.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.4/tests/test_deepeq.py` & `miniscutil-0.2.5/tests/test_deepeq.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.4/tests/test_lsp.py` & `miniscutil-0.2.5/tests/test_lsp.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.4/tests/test_ofdict.py` & `miniscutil-0.2.5/tests/test_ofdict.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.4/tests/test_typing.py` & `miniscutil-0.2.5/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.4/.gitignore` & `miniscutil-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.4/LICENSE.txt` & `miniscutil-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.4/README.md` & `miniscutil-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.4/pyproject.toml` & `miniscutil-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.4/PKG-INFO` & `miniscutil-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniscutil
-Version: 0.2.4
+Version: 0.2.5
 Project-URL: Documentation, https://github.com/EdAyers/sss/miniscutil#readme
 Project-URL: Issues, https://github.com/EdAyers/sss/miniscutil/issues
 Project-URL: Source, https://github.com/EdAyers/sss/miniscutil
 Author-email: "E.W.Ayers" <contact@edayers.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

