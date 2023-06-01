# Comparing `tmp/tika_client-0.0.1.tar.gz` & `tmp/tika_client-0.0.2.tar.gz`

## Comparing `tika_client-0.0.1.tar` & `tika_client-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 tika_client-0.0.1/.editorconfig
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 tika_client-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 tika_client-0.0.1/CHANGELOG.md
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 tika_client-0.0.1/.docker/docker-compose.ci-test.yml
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 tika_client-0.0.1/.github/dependabot.yml
--rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 tika_client-0.0.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 tika_client-0.0.1/.github/workflows/codeql.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tika_client-0.0.1/src/tika_client/__about__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 tika_client-0.0.1/src/tika_client/__init__.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 tika_client-0.0.1/src/tika_client/_resource_meta.py
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 tika_client-0.0.1/src/tika_client/_resource_recursive.py
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 tika_client-0.0.1/src/tika_client/_resource_tika.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 tika_client-0.0.1/src/tika_client/_utils.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 tika_client-0.0.1/src/tika_client/client.py
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 tika_client-0.0.1/src/tika_client/data_models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tika_client-0.0.1/src/tika_client/py.typed
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 tika_client-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 tika_client-0.0.1/tests/conftest.py
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 tika_client-0.0.1/tests/test_resource_metadata.py
--rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 tika_client-0.0.1/tests/test_resource_recursive_metadata.py
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 tika_client-0.0.1/tests/test_resource_tika.py
--rw-r--r--   0        0        0    14164 2020-02-02 00:00:00.000000 tika_client-0.0.1/tests/samples/microsoft-sample.docx
--rw-r--r--   0        0        0     8843 2020-02-02 00:00:00.000000 tika_client-0.0.1/tests/samples/sample-spreadsheet.ods
--rw-r--r--   0        0        0     4743 2020-02-02 00:00:00.000000 tika_client-0.0.1/tests/samples/sample-spreadsheet.xlsx
--rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 tika_client-0.0.1/tests/samples/sample.docx
--rw-r--r--   0        0        0     8271 2020-02-02 00:00:00.000000 tika_client-0.0.1/tests/samples/sample.odt
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 tika_client-0.0.1/.gitignore
--rw-r--r--   0        0        0    34670 2020-02-02 00:00:00.000000 tika_client-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 tika_client-0.0.1/README.md
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 tika_client-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 tika_client-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 tika_client-0.0.2/.editorconfig
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 tika_client-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 tika_client-0.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 tika_client-0.0.2/.docker/docker-compose.ci-test.yml
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 tika_client-0.0.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 tika_client-0.0.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 tika_client-0.0.2/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tika_client-0.0.2/src/tika_client/__about__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 tika_client-0.0.2/src/tika_client/__init__.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 tika_client-0.0.2/src/tika_client/_resource_meta.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 tika_client-0.0.2/src/tika_client/_resource_recursive.py
+-rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 tika_client-0.0.2/src/tika_client/_resource_tika.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 tika_client-0.0.2/src/tika_client/_utils.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 tika_client-0.0.2/src/tika_client/client.py
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 tika_client-0.0.2/src/tika_client/data_models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tika_client-0.0.2/src/tika_client/py.typed
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 tika_client-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 tika_client-0.0.2/tests/conftest.py
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 tika_client-0.0.2/tests/test_resource_metadata.py
+-rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 tika_client-0.0.2/tests/test_resource_recursive_metadata.py
+-rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 tika_client-0.0.2/tests/test_resource_tika.py
+-rw-r--r--   0        0        0    14164 2020-02-02 00:00:00.000000 tika_client-0.0.2/tests/samples/microsoft-sample.docx
+-rw-r--r--   0        0        0     8843 2020-02-02 00:00:00.000000 tika_client-0.0.2/tests/samples/sample-spreadsheet.ods
+-rw-r--r--   0        0        0     4743 2020-02-02 00:00:00.000000 tika_client-0.0.2/tests/samples/sample-spreadsheet.xlsx
+-rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 tika_client-0.0.2/tests/samples/sample.docx
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 tika_client-0.0.2/tests/samples/sample.html
+-rw-r--r--   0        0        0     8271 2020-02-02 00:00:00.000000 tika_client-0.0.2/tests/samples/sample.odt
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 tika_client-0.0.2/.gitignore
+-rw-r--r--   0        0        0    34670 2020-02-02 00:00:00.000000 tika_client-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 tika_client-0.0.2/README.md
+-rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 tika_client-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 tika_client-0.0.2/PKG-INFO
```

### Comparing `tika_client-0.0.1/.editorconfig` & `tika_client-0.0.2/.editorconfig`

 * *Files identical despite different names*

### Comparing `tika_client-0.0.1/.pre-commit-config.yaml` & `tika_client-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tika_client-0.0.1/CHANGELOG.md` & `tika_client-0.0.2/CHANGELOG.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,28 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.0.2] - 2023-05-31
+
+### Added
+
+- Print of the Python version to the test coverage running
+- Optional dependencies for HTTP/2 and Brotli support in httpx
+- `add_headers` to allow users to update the client's headers
+- Support for Tika endpoint with a string or byte buffer instead of a file
+- Built wheels are now retained for 7 days instead of 90 days
+
+### Fixed
+
+- Reduces the frequency of CodeQL runs
+
 ## [0.0.1] - 2023-05-25
 
 ### Added
 
 - Support for Tika metadata, tika and recursive metadata endpoints
 - Full test coverage
 - Full typing
```

### Comparing `tika_client-0.0.1/.github/dependabot.yml` & `tika_client-0.0.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `tika_client-0.0.1/.github/workflows/ci.yml` & `tika_client-0.0.2/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     name: Python ${{ matrix.python-version }}
     runs-on: ubuntu-latest
     needs:
       - lint
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.8', '3.9', '3.10', '3.11', 'pypy3.8', 'pypy3.9']
+        python-version: ['3.8', '3.9', '3.10', '3.11', '3.12-dev', 'pypy3.8', 'pypy3.9']
 
     steps:
       -
         uses: actions/checkout@v3
       -
         name: Start containers
         run: |
@@ -112,14 +112,15 @@
           hatch build --clean
       -
         uses: actions/upload-artifact@v3
         with:
             name: artifacts
             path: dist/*
             if-no-files-found: error
+            retention-days: 7
 
   publish:
     name: Publish project
     runs-on: ubuntu-latest
     if: startsWith(github.ref, 'refs/tags/')
     permissions:
       id-token: write  # IMPORTANT: this permission is mandatory for trusted publishing
```

### Comparing `tika_client-0.0.1/.github/workflows/codeql.yml` & `tika_client-0.0.2/.github/workflows/codeql.yml`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,21 @@
 # the `language` matrix defined below to confirm you have the correct set of
 # supported CodeQL languages.
 #
 name: "CodeQL"
 
 on:
   push:
+    branches:
+      - main
+      - develop
   pull_request:
+    branches:
+      - main
+      - develop
   schedule:
     - cron: '20 0 * * 1'
 
 jobs:
   analyze:
     name: Analyze
     runs-on: ${{ (matrix.language == 'swift' && 'macos-latest') || 'ubuntu-latest' }}
```

### Comparing `tika_client-0.0.1/src/tika_client/_resource_meta.py` & `tika_client-0.0.2/src/tika_client/_resource_meta.py`

 * *Files identical despite different names*

### Comparing `tika_client-0.0.1/src/tika_client/_resource_recursive.py` & `tika_client-0.0.2/src/tika_client/_resource_recursive.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,26 +37,26 @@
         return documents
 
 
 class _RecursiveMetaHtml(_TikaRmetaBase):
     ENDPOINT: Final[str] = "/rmeta"
     MULTI_PART_ENDPOINT = "/rmeta/form/html"
 
-    def parse(self, filepath: Path, mime_type: Optional[str] = None):
+    def from_file(self, filepath: Path, mime_type: Optional[str] = None):
         """
         Returns the formatted (as HTML) document data
         """
         return self._common_call(self.MULTI_PART_ENDPOINT, filepath, mime_type)
 
 
 class _RecursiveMetaPlain(_TikaRmetaBase):
     ENDPOINT: Final[str] = "/rmeta/text"
     MULTI_PART_ENDPOINT = "/rmeta/form/text"
 
-    def parse(self, filepath: Path, mime_type: Optional[str] = None):
+    def from_file(self, filepath: Path, mime_type: Optional[str] = None):
         """
         Returns the plain text document data
         """
         return self._common_call(self.MULTI_PART_ENDPOINT, filepath, mime_type)
 
 
 class Recursive(BaseResource):
```

### Comparing `tika_client-0.0.1/src/tika_client/_resource_tika.py` & `tika_client-0.0.2/src/tika_client/_resource_tika.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,50 +8,80 @@
 from tika_client._utils import BaseResource
 from tika_client.data_models import KNOWN_DATA_TYPES
 from tika_client.data_models import BaseResponse
 from tika_client.data_models import Document
 
 
 class _TikaBase(BaseResource):
-    def _common_call(
+    def _common_multi_part_put(
         self,
         endpoint: str,
         filepath: Path,
         mime_type: Optional[str] = None,
     ) -> Union[BaseResponse, Document]:
         """
         Given a specific endpoint and a file, do a multipart put to the endpoint
         """
         resp = self.put_multipart(endpoint, filepath, mime_type)
         base_resp = BaseResponse(resp)
         if base_resp.type in KNOWN_DATA_TYPES:
             return KNOWN_DATA_TYPES[base_resp.type](base_resp.data)
         return base_resp  # pragma: no cover
 
+    def _common_content_put(
+        self,
+        endpoint: str,
+        content: Union[str, bytes],
+    ) -> Union[BaseResponse, Document]:
+        """
+        Preforms an HTTP PUT with the given content and returns a decoded response.
+        Includes handling of string to bytes and setting content length correctly
+        """
+        content_bytes = content.encode("utf-8") if isinstance(content, str) else content
+        resp = self.client.put(endpoint, content=content_bytes, headers={"Content-Length": str(len(content_bytes))})
+        resp.raise_for_status()
+
+        base_resp = BaseResponse(resp.json())
+        if base_resp.type in KNOWN_DATA_TYPES:
+            return KNOWN_DATA_TYPES[base_resp.type](base_resp.data)
+        return base_resp  # pragma: no cover
+
 
 class _TikaHtml(_TikaBase):
     ENDPOINT: Final[str] = "/tika"
     MULTI_PART_ENDPOINT = "/tika/form"
 
-    def parse(self, filepath: Path, mime_type: Optional[str] = None):
+    def from_file(self, filepath: Path, mime_type: Optional[str] = None):
         """
         Returns the formatted (as HTML) document data
         """
-        return self._common_call(self.MULTI_PART_ENDPOINT, filepath, mime_type)
+        return self._common_multi_part_put(self.MULTI_PART_ENDPOINT, filepath, mime_type)
+
+    def from_buffer(self, content: Union[str, bytes]) -> Union[BaseResponse, Document]:
+        """
+        Returns the HTML formatted document data from a given string of document content
+        """
+        return self._common_content_put(self.ENDPOINT, content)
 
 
 class _TikaPlain(_TikaBase):
     PLAIN_TEXT_CONTENT: Final[str] = "/tika/text"
     MULTI_PART_PLAIN_TEXT_CONTENT = "/tika/form/text"
 
-    def parse(self, filepath: Path, mime_type: Optional[str] = None):
+    def from_file(self, filepath: Path, mime_type: Optional[str] = None):
         """
         Returns the plain text document data
         """
-        return self._common_call(self.MULTI_PART_PLAIN_TEXT_CONTENT, filepath, mime_type)
+        return self._common_multi_part_put(self.MULTI_PART_PLAIN_TEXT_CONTENT, filepath, mime_type)
+
+    def from_buffer(self, content: Union[str, bytes]) -> Union[BaseResponse, Document]:
+        """
+        Returns the plain text document data from a given string of document content
+        """
+        return self._common_content_put(self.PLAIN_TEXT_CONTENT, content)
 
 
 class Tika(BaseResource):
     """
     Handles interaction with the /tika endpoint of a Tika server REST API, returning the HTML
     formatted content or the plain text, depending on how the client is accessed
```

### Comparing `tika_client-0.0.1/src/tika_client/_utils.py` & `tika_client-0.0.2/src/tika_client/_utils.py`

 * *Files identical despite different names*

### Comparing `tika_client-0.0.1/src/tika_client/client.py` & `tika_client-0.0.2/src/tika_client/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from typing import Dict
 
 from httpx import Client
 
 from tika_client._resource_meta import Metadata
 from tika_client._resource_recursive import Recursive
 from tika_client._resource_tika import Tika
 
@@ -20,12 +21,18 @@
         self._client.headers.update({"Accept": "application/json"})
 
         # Add the resources
         self.metadata = Metadata(self._client)
         self.tika = Tika(self._client)
         self.rmeta = Recursive(self._client)
 
+    def add_headers(self, header: Dict[str, str]):
+        """
+        Updates the httpx Client headers with the given values
+        """
+        self._client.headers.update(header)
+
     def __enter__(self) -> "TikaClient":
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb) -> None:
         self._client.close()
```

### Comparing `tika_client-0.0.1/src/tika_client/data_models.py` & `tika_client-0.0.2/src/tika_client/data_models.py`

 * *Files identical despite different names*

### Comparing `tika_client-0.0.1/tests/test_resource_metadata.py` & `tika_client-0.0.2/tests/test_resource_metadata.py`

 * *Files identical despite different names*

### Comparing `tika_client-0.0.1/tests/test_resource_recursive_metadata.py` & `tika_client-0.0.2/tests/test_resource_recursive_metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,80 +3,80 @@
 from tests.conftest import SAMPLE_DIR
 from tika_client.client import TikaClient
 
 
 class TestRecursiveMetadataResource:
     def test_r_metadata_from_docx(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.docx"
-        documents = tika_client.rmeta.html.parse(test_file, magic.from_file(str(test_file), mime=True))
+        documents = tika_client.rmeta.html.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
         assert len(documents) == 1
         document = documents[0]
 
         assert document.type == "application/vnd.openxmlformats-officedocument.wordprocessingml.document"
         assert "<body><p>This is an DOCX test document, also made September 14, 2022</p>\n</body>" in document.content
         assert document.metadata.created is None
 
     def test_r_metadata_from_docx_plain(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.docx"
-        documents = tika_client.rmeta.text.parse(test_file, magic.from_file(str(test_file), mime=True))
+        documents = tika_client.rmeta.text.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
         assert len(documents) == 1
         document = documents[0]
 
         assert document.type == "application/vnd.openxmlformats-officedocument.wordprocessingml.document"
         assert "This is an DOCX test document, also made September 14, 2022" in document.content
         assert document.metadata.created is None
 
     def test_r_meta_microsoft_word_docx(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "microsoft-sample.docx"
-        documents = tika_client.rmeta.html.parse(test_file, magic.from_file(str(test_file), mime=True))
+        documents = tika_client.rmeta.html.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
         assert len(documents) == 1
         document = documents[0]
 
         assert document.type == "application/vnd.openxmlformats-officedocument.wordprocessingml.document"
         assert (
             "<body><p>This is a sample document, generated by Microsoft Office on Wednesday, May 17, 2023.</p>\n<p>It is in English.</p>\n</body>"  # noqa: E501
             in document.content
         )
 
     def test_r_metadata_from_odt(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.odt"
-        documents = tika_client.rmeta.html.parse(test_file, magic.from_file(str(test_file), mime=True))
+        documents = tika_client.rmeta.html.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
         assert len(documents) == 2
         document = documents[0]
 
         assert document.type == "application/vnd.oasis.opendocument.text"
         assert "<body><p>This is an ODT test document, created September 14, 2022</p>\n</body>" in document.content
         assert document.metadata.created is None
 
     def test_r_metadata_from_odt_plain(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.odt"
-        documents = tika_client.rmeta.text.parse(test_file, magic.from_file(str(test_file), mime=True))
+        documents = tika_client.rmeta.text.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
         assert len(documents) == 2
         document = documents[0]
 
         assert document.type == "application/vnd.oasis.opendocument.text"
         assert "This is an ODT test document, created September 14, 2022" in document.content
 
     def test_r_metadata_from_ods_plain(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample-spreadsheet.ods"
-        documents = tika_client.rmeta.text.parse(test_file, magic.from_file(str(test_file), mime=True))
+        documents = tika_client.rmeta.text.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
         assert len(documents) == 2
         document = documents[0]
 
         assert "This is cell A1" in document.content
         assert "You sunk my battleship" in document.content
 
     def test_r_metadata_from_xlsx_plain(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample-spreadsheet.xlsx"
-        documents = tika_client.rmeta.text.parse(test_file, magic.from_file(str(test_file), mime=True))
+        documents = tika_client.rmeta.text.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
         assert len(documents) == 1
         document = documents[0]
 
         assert "This is cell A1" in document.content
         assert "You sunk my battleship" in document.content
```

### Comparing `tika_client-0.0.1/tests/test_resource_tika.py` & `tika_client-0.0.2/tests/test_resource_tika.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,57 +4,93 @@
 from tika_client.client import TikaClient
 from tika_client.data_models import Document
 
 
 class TestParseFormatted:
     def test_parse_docx(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.docx"
-        resp = tika_client.tika.html.parse(test_file, magic.from_file(str(test_file), mime=True))
+        resp = tika_client.tika.html.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
         assert isinstance(resp, Document)
         assert resp.type == "application/vnd.openxmlformats-officedocument.wordprocessingml.document"
         assert "<body><p>This is an DOCX test document, also made September 14, 2022</p>\n</body>" in resp.content
 
     def test_parse_docx_no_mime(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.docx"
-        resp = tika_client.tika.html.parse(test_file)
+        resp = tika_client.tika.html.from_file(test_file)
 
         assert isinstance(resp, Document)
         assert resp.type == "application/vnd.openxmlformats-officedocument.wordprocessingml.document"
         assert "<body><p>This is an DOCX test document, also made September 14, 2022</p>\n</body>" in resp.content
 
     def test_parse_microsoft_word_docx(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "microsoft-sample.docx"
-        resp = tika_client.tika.html.parse(test_file, magic.from_file(str(test_file), mime=True))
+        resp = tika_client.tika.html.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
         assert isinstance(resp, Document)
         assert resp.type == "application/vnd.openxmlformats-officedocument.wordprocessingml.document"
         assert (
             "<body><p>This is a sample document, generated by Microsoft Office on Wednesday, May 17, 2023.</p>\n<p>It is in English.</p>\n</body>"  # noqa: E501
             in resp.content
         )
 
     def test_parse_odt(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.odt"
-        resp = tika_client.tika.html.parse(test_file, magic.from_file(str(test_file), mime=True))
+        resp = tika_client.tika.html.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
         assert isinstance(resp, Document)
         assert resp.type == "application/vnd.oasis.opendocument.text"
         assert "<body><p>This is an ODT test document, created September 14, 2022</p>\n</body>" in resp.content
 
 
 class TestParsePlain:
     def test_parse_docx(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.docx"
-        resp = tika_client.tika.text.parse(test_file, magic.from_file(str(test_file), mime=True))
+
+        resp = tika_client.tika.text.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
         assert isinstance(resp, Document)
         assert resp.type == "application/vnd.openxmlformats-officedocument.wordprocessingml.document"
         assert "This is an DOCX test document, also made September 14, 2022" in resp.content
 
     def test_parse_odt(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.odt"
-        resp = tika_client.tika.text.parse(test_file, magic.from_file(str(test_file), mime=True))
+
+        resp = tika_client.tika.text.from_file(test_file, magic.from_file(str(test_file), mime=True))
+
+        assert isinstance(resp, Document)
+        assert resp.type == "application/vnd.oasis.opendocument.text"
+        assert "This is an ODT test document, created September 14, 2022" in resp.content
+
+
+class TestParseContentPlain:
+    def test_parse_docx_bytes(self, tika_client: TikaClient):
+        test_file = SAMPLE_DIR / "sample.docx"
+        buffer = test_file.read_bytes()
+
+        resp = tika_client.tika.text.from_buffer(buffer)
+
+        assert isinstance(resp, Document)
+        assert resp.type == "application/vnd.openxmlformats-officedocument.wordprocessingml.document"
+        assert "This is an DOCX test document, also made September 14, 2022" in resp.content
+
+    def test_parse_odt_bytes(self, tika_client: TikaClient):
+        test_file = SAMPLE_DIR / "sample.odt"
+        buffer = test_file.read_bytes()
+
+        resp = tika_client.tika.text.from_buffer(buffer)
 
         assert isinstance(resp, Document)
         assert resp.type == "application/vnd.oasis.opendocument.text"
         assert "This is an ODT test document, created September 14, 2022" in resp.content
+
+    def test_parse_buffer_text_content(self, tika_client: TikaClient):
+        test_file = SAMPLE_DIR / "sample.html"
+        buffer = test_file.read_text()
+
+        resp = tika_client.tika.text.from_buffer(buffer)
+
+        assert resp.type == "text/html; charset=UTF-8"
+        assert resp.parsers == ["org.apache.tika.parser.DefaultParser", "org.apache.tika.parser.html.HtmlParser"]
+        assert "Hello world! This is HTML5 content in a file for" in resp.data["X-TIKA:content"]
+        assert resp.data["dc:title"] == "This Is A Test"
+        assert resp.data["description"] == "A sample HTML file"
```

### Comparing `tika_client-0.0.1/tests/samples/microsoft-sample.docx` & `tika_client-0.0.2/tests/samples/microsoft-sample.docx`

 * *Files identical despite different names*

### Comparing `tika_client-0.0.1/tests/samples/sample-spreadsheet.ods` & `tika_client-0.0.2/tests/samples/sample-spreadsheet.ods`

 * *Files identical despite different names*

### Comparing `tika_client-0.0.1/tests/samples/sample-spreadsheet.xlsx` & `tika_client-0.0.2/tests/samples/sample-spreadsheet.xlsx`

 * *Files identical despite different names*

### Comparing `tika_client-0.0.1/tests/samples/sample.docx` & `tika_client-0.0.2/tests/samples/sample.docx`

 * *Files identical despite different names*

### Comparing `tika_client-0.0.1/tests/samples/sample.odt` & `tika_client-0.0.2/tests/samples/sample.odt`

 * *Files identical despite different names*

### Comparing `tika_client-0.0.1/.gitignore` & `tika_client-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tika_client-0.0.1/LICENSE.txt` & `tika_client-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tika_client-0.0.1/README.md` & `tika_client-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -38,26 +38,26 @@
 
 with TikaClient("http://localhost:9998) as client
 
     # Extract a document's metadata
     metadata = client.metadata.from_file(test_file)
 
     # Get the content of a document as HTML
-    data = client.tika.html.parse(test_file)
+    data = client.tika.html.from_file(test_file)
 
     # Or as plain text
-    text = client.tika.text.parse(test_file)
+    text = client.tika.text.from_file(test_file)
 
     # Content and metadata combined
-    data = client.rmeta.text.parse(test_file)
+    data = client.rmeta.text.from_file(test_file)
 
     # The mime type can also be given
     # This allows Content-Type to be set most accurately
-    text = client.tika.text.parse(test_file,
-                                  "application/vnd.openxmlformats-officedocument.wordprocessingml.document")
+    text = client.tika.text.from_file(test_file,
+                                      "application/vnd.openxmlformats-officedocument.wordprocessingml.document")
 
 ```
 
 The Tika REST API documentation can be found [here](https://cwiki.apache.org/confluence/display/TIKA/TikaServer).
 At the moment, only the metadata, tika and recursive metadata endpoints are implemented.
 
 Unfortunately, the set of possible return values of the Tika API are not very well documented. The library makes
```

### Comparing `tika_client-0.0.1/pyproject.toml` & `tika_client-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,18 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = ["httpx"]
 
+[project.optional-dependencies]
+"http2" = ["httpx[http2]"]
+"brotli" = ["httpx[brotli]"]
+
 [project.urls]
 Documentation = "https://github.com/stumpylog/tika-rest-client#readme"
 Issues = "https://github.com/stumpylog/tika-rest-client/issues"
 Source = "https://github.com/stumpylog/tika-rest-client"
 
 [tool.hatch.version]
 path = "src/tika_client/__about__.py"
@@ -39,25 +43,28 @@
   "pytest",
   "pytest-sugar",
   "pytest-cov",
   "pytest-xdist",
   "pytest-httpx",
   "python-magic",
 ]
+
 [tool.hatch.envs.default.scripts]
+version = "python3 --version"
 test = "pytest {args:tests}"
 cov-clear = "coverage erase"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "- coverage combine",
   "coverage report",
 ]
 cov-html = "coverage html"
 cov-json = "coverage json"
 cov = [
+  "version",
   "cov-clear",
   "test-cov",
   "cov-report",
   "cov-json"
 ]
 
 [[tool.hatch.envs.all.matrix]]
@@ -67,14 +74,15 @@
 detached = true
 dependencies = [
   "black>=23.1.0",
   "mypy>=1.0.0",
   "ruff>=0.0.243",
   "httpx",
 ]
+
 [tool.hatch.envs.lint.scripts]
 typing = "mypy --install-types --non-interactive {args:src/tika_client}"
 style = [
   "ruff {args:.}",
   "black --check --diff {args:.}",
 ]
 fmt = [
```

### Comparing `tika_client-0.0.1/PKG-INFO` & `tika_client-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tika-client
-Version: 0.0.1
+Version: 0.0.2
 Summary: A modern REST client for Apache Tika server
 Project-URL: Documentation, https://github.com/stumpylog/tika-rest-client#readme
 Project-URL: Issues, https://github.com/stumpylog/tika-rest-client/issues
 Project-URL: Source, https://github.com/stumpylog/tika-rest-client
 Author-email: Trenton H <797416+stumpylog@users.noreply.github.com>
 License-Expression: GPL-3.0-only
 License-File: LICENSE.txt
@@ -14,14 +14,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: httpx
+Provides-Extra: brotli
+Requires-Dist: httpx[brotli]; extra == 'brotli'
+Provides-Extra: http2
+Requires-Dist: httpx[http2]; extra == 'http2'
 Description-Content-Type: text/markdown
 
 # Tika Rest Client
 
 [![PyPI - Version](https://img.shields.io/pypi/v/tika-client.svg)](https://pypi.org/project/tika-client)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tika-client.svg)](https://pypi.org/project/tika-client)
 [![codecov](https://codecov.io/github/stumpylog/tika-client/branch/main/graph/badge.svg?token=PTESS6YUK5)](https://codecov.io/github/stumpylog/tika-client)
@@ -60,26 +64,26 @@
 
 with TikaClient("http://localhost:9998) as client
 
     # Extract a document's metadata
     metadata = client.metadata.from_file(test_file)
 
     # Get the content of a document as HTML
-    data = client.tika.html.parse(test_file)
+    data = client.tika.html.from_file(test_file)
 
     # Or as plain text
-    text = client.tika.text.parse(test_file)
+    text = client.tika.text.from_file(test_file)
 
     # Content and metadata combined
-    data = client.rmeta.text.parse(test_file)
+    data = client.rmeta.text.from_file(test_file)
 
     # The mime type can also be given
     # This allows Content-Type to be set most accurately
-    text = client.tika.text.parse(test_file,
-                                  "application/vnd.openxmlformats-officedocument.wordprocessingml.document")
+    text = client.tika.text.from_file(test_file,
+                                      "application/vnd.openxmlformats-officedocument.wordprocessingml.document")
 
 ```
 
 The Tika REST API documentation can be found [here](https://cwiki.apache.org/confluence/display/TIKA/TikaServer).
 At the moment, only the metadata, tika and recursive metadata endpoints are implemented.
 
 Unfortunately, the set of possible return values of the Tika API are not very well documented. The library makes
```

