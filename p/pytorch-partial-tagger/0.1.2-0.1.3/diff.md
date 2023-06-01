# Comparing `tmp/pytorch_partial_tagger-0.1.2.tar.gz` & `tmp/pytorch_partial_tagger-0.1.3.tar.gz`

## Comparing `pytorch_partial_tagger-0.1.2.tar` & `pytorch_partial_tagger-0.1.3.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/__about__.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/embedders.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/matchers.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/recognizer.py
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/tagger.py
--rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/training.py
--rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/utils.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/crf/__init__.py
--rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/crf/functional.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/crf/nn.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/data/__init__.py
--rw-r--r--   0        0        0     8618 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/data/batch.py
--rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/data/core.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/decoders/__init__.py
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/decoders/viterbi.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/encoders/__init__.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/encoders/base.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/encoders/linear.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/tests/conftest.py
--rw-r--r--   0        0        0     7368 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/tests/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/tests/crf/__init__.py
--rw-r--r--   0        0        0    10349 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/tests/crf/test_functional.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/tests/crf/test_nn.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/tests/data/__init__.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/tests/data/test_batch.py
--rw-r--r--   0        0        0     5605 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/tests/data/test_core.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/LICENSE
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/README.md
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0    14871 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/notebooks/basic.ipynb
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/__about__.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/embedders.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/matchers.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/recognizer.py
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/tagger.py
+-rw-r--r--   0        0        0     6685 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/training.py
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/utils.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/crf/__init__.py
+-rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/crf/functional.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/crf/nn.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/data/__init__.py
+-rw-r--r--   0        0        0     8725 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/data/batch.py
+-rw-r--r--   0        0        0     7441 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/data/core.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/decoders/__init__.py
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/decoders/viterbi.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/encoders/__init__.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/encoders/base.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/encoders/linear.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/tests/conftest.py
+-rw-r--r--   0        0        0     7257 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/tests/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/tests/crf/__init__.py
+-rw-r--r--   0        0        0    10350 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/tests/crf/test_functional.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/tests/crf/test_nn.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/tests/data/__init__.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/tests/data/test_batch.py
+-rw-r--r--   0        0        0     5606 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/tests/data/test_core.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/README.md
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/PKG-INFO
```

### Comparing `pytorch_partial_tagger-0.1.2/.github/workflows/ci.yml` & `pytorch_partial_tagger-0.1.3/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.10", "3.11"]
+        python-version: [3.8, 3.9, "3.10", "3.11"]
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `pytorch_partial_tagger-0.1.2/.github/workflows/pypi-publish.yml` & `pytorch_partial_tagger-0.1.3/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.2/src/partial_tagger/embedders.py` & `pytorch_partial_tagger-0.1.3/src/partial_tagger/embedders.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.2/src/partial_tagger/matchers.py` & `pytorch_partial_tagger-0.1.3/src/partial_tagger/matchers.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.2/src/partial_tagger/recognizer.py` & `pytorch_partial_tagger-0.1.3/src/partial_tagger/recognizer.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.2/src/partial_tagger/tagger.py` & `pytorch_partial_tagger-0.1.3/src/partial_tagger/tagger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import torch
 from torch.nn import Module
 
 from .crf.nn import CRF
 from .data.batch import TaggerInputs
 from .decoders import ViterbiDecoder
 from .embedders import BaseEmbedder
```

### Comparing `pytorch_partial_tagger-0.1.2/src/partial_tagger/training.py` & `pytorch_partial_tagger-0.1.3/src/partial_tagger/training.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import io
 import logging
 from logging import Logger
 from typing import cast
 
 import torch
 from torch.utils.data import DataLoader
```

### Comparing `pytorch_partial_tagger-0.1.2/src/partial_tagger/utils.py` & `pytorch_partial_tagger-0.1.3/src/partial_tagger/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from transformers import AutoModel, AutoTokenizer
 
 from .data import LabelSet, Span, Tag
 from .data.batch import CharBasedTagsCollection, Collator, TransformerBatchFactory
 from .decoders.viterbi import Contrainer, ViterbiDecoder
 from .embedders import TransformerEmbedder
 from .encoders.linear import LinearEncoder
@@ -74,15 +76,15 @@
         self.__fn = 0
 
     def __call__(
         self,
         predictions: CharBasedTagsCollection,
         ground_truths: CharBasedTagsCollection,
     ) -> None:
-        for tags1, tags2 in zip(predictions, ground_truths, strict=True):
+        for tags1, tags2 in zip(predictions, ground_truths):
             tag_set1 = {(tag1.start, tag1.length, tag1.label) for tag1 in tags1}
             tag_set2 = {(tag2.start, tag2.length, tag2.label) for tag2 in tags2}
 
             self.__tp += len(tag_set1 & tag_set2)
             self.__fp += len(tag_set1 - tag_set2)
             self.__fn += len(tag_set2 - tag_set1)
```

### Comparing `pytorch_partial_tagger-0.1.2/src/partial_tagger/crf/functional.py` & `pytorch_partial_tagger-0.1.3/src/partial_tagger/crf/functional.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.2/src/partial_tagger/crf/nn.py` & `pytorch_partial_tagger-0.1.3/src/partial_tagger/crf/nn.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.2/src/partial_tagger/data/batch.py` & `pytorch_partial_tagger-0.1.3/src/partial_tagger/data/batch.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,30 @@
+from __future__ import annotations
+
 from abc import ABCMeta, abstractmethod
 from itertools import groupby
-from typing import Optional
+from typing import Dict, List, Optional, Tuple
 
 import torch
 from transformers.tokenization_utils import PreTrainedTokenizer
 
 from ..crf.functional import to_tag_bitmap
 from . import CharBasedTags, LabelSet, Span, SubwordBasedTags, Tag, TokenizedText
 
-Texts = tuple[str, ...]
-TokenizedTexts = tuple[TokenizedText, ...]
+# https://bugs.python.org/issue45117
+# type alias for tuple, dict, list is no longer supported in py38.
+Texts = Tuple[str, ...]
+TokenizedTexts = Tuple[TokenizedText, ...]
 
-CharBasedTagsCollection = tuple[CharBasedTags, ...]
-SubwordBasedTagsCollection = tuple[SubwordBasedTags, ...]
+CharBasedTagsCollection = Tuple[CharBasedTags, ...]
+SubwordBasedTagsCollection = Tuple[SubwordBasedTags, ...]
 
-Dataset = list[tuple[str, CharBasedTags]]
+Dataset = List[Tuple[str, CharBasedTags]]
 
-TaggerInputs = dict[str, torch.Tensor]
+TaggerInputs = Dict[str, torch.Tensor]
 
 
 def pad(batch: list[list[int]], fill_value: int) -> torch.Tensor:
     max_length = max(map(len, batch))
     return torch.tensor([x + [fill_value] * (max_length - len(x)) for x in batch])
 
 
@@ -49,15 +53,15 @@
         self, tag_indices: torch.Tensor, padding_index: int = -1
     ) -> SubwordBasedTagsCollection:
         label_set = self.__label_set
 
         batched_tags = []
 
         for text, indices in zip(
-            self.__tokenized_texts, unpad(tag_indices, padding_index), strict=True
+            self.__tokenized_texts, unpad(tag_indices, padding_index)
         ):
             tags = []
             now = 0
             for label, group in groupby(
                 label_set.get_label(index) for index in indices
             ):
                 length = len(list(group))
@@ -77,15 +81,15 @@
         device: torch.device,
         padding_index: int = -1,
         unknown_index: int = -100,
     ) -> torch.Tensor:
         tag_indices = []
         label_set = self.__label_set
 
-        for text, tags in zip(self.__tokenized_texts, tags_collection, strict=True):
+        for text, tags in zip(self.__tokenized_texts, tags_collection):
             indices = [unknown_index] * text.num_tokens
 
             for token_index in range(text.num_tokens):
                 span = text.get_char_span(token_index)
                 if span is None:
                     indices[token_index] = label_set.get_outside_index()
 
@@ -211,15 +215,15 @@
 
         mappings = batch_encoding.pop("offset_mapping").tolist()
         pad_token_id = self.__tokenizer.pad_token_id
         tokenized_text_lengths = (batch_encoding.input_ids != pad_token_id).sum(dim=1)
 
         tokenized_texts = []
         for tokenized_text_length, mapping, text in zip(
-            tokenized_text_lengths, mappings, texts, strict=True
+            tokenized_text_lengths, mappings, texts
         ):
             char_spans = tuple(
                 Span(start, end - start) if start != end else None
                 for start, end in mapping[:tokenized_text_length]
             )
             token_indices = [-1] * len(text)
             for token_index, char_span in enumerate(char_spans):
@@ -246,9 +250,9 @@
 
 
 class Collator:
     def __init__(self, batch_factory: BaseBatchFactory):
         self.batch_factory = batch_factory
 
     def __call__(self, examples: Dataset) -> tuple[Batch, CharBasedTagsCollection]:
-        texts, tags_collection = zip(*examples, strict=True)
+        texts, tags_collection = zip(*examples)
         return self.batch_factory.create(texts), tags_collection
```

### Comparing `pytorch_partial_tagger-0.1.2/src/partial_tagger/data/core.py` & `pytorch_partial_tagger-0.1.3/src/partial_tagger/data/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from bisect import bisect_left
 from collections.abc import Iterator
 from dataclasses import dataclass
 
 
 @dataclass(frozen=True, eq=True)
 class Span:
@@ -148,15 +150,15 @@
             *range(
                 self.__status_kind,
                 self.get_tag_size(),
                 self.__status_kind,
             )
         ]
 
-        self.__label_ids = dict(zip(self.__labels, self.__start_indices, strict=True))
+        self.__label_ids = dict(zip(self.__labels, self.__start_indices))
 
     def get_outside_index(self) -> int:
         return 0
 
     def get_start_index(self, label: str) -> int:
         if label not in self.__label_ids:
             raise ValueError("Invalid label is given.")
```

### Comparing `pytorch_partial_tagger-0.1.2/src/partial_tagger/decoders/viterbi.py` & `pytorch_partial_tagger-0.1.3/src/partial_tagger/decoders/viterbi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from abc import ABCMeta, abstractmethod
 from typing import Optional
 
 import torch
 from torch.nn import Module, Parameter
 
 from ..crf import functional as F
```

### Comparing `pytorch_partial_tagger-0.1.2/src/partial_tagger/encoders/base.py` & `pytorch_partial_tagger-0.1.3/src/partial_tagger/encoders/base.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.2/src/partial_tagger/encoders/linear.py` & `pytorch_partial_tagger-0.1.3/src/partial_tagger/encoders/linear.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.2/tests/conftest.py` & `pytorch_partial_tagger-0.1.3/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
 import torch
+
 from partial_tagger.crf import NINF
 
 
 @pytest.fixture
 def num_tags() -> int:
     return 5
```

### Comparing `pytorch_partial_tagger-0.1.2/tests/helpers.py` & `pytorch_partial_tagger-0.1.3/tests/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from itertools import product
 from typing import Generator, Tuple
 
 import torch
+
 from partial_tagger.crf import NINF
 from partial_tagger.crf import functional as F
 
 
 def iterate_possible_tag_indices(
     sequence_length: int, num_tags: int
 ) -> Generator[tuple, None, None]:
@@ -26,17 +27,15 @@
 
 def compute_log_normalizer_by_brute_force(log_potentials: torch.Tensor) -> torch.Tensor:
     batch_size, sequence_length, num_tags, _ = log_potentials.size()
     log_Z = torch.tensor([NINF] * batch_size)
     for b in range(batch_size):
         for tag_indices in iterate_possible_tag_indices(sequence_length + 1, num_tags):
             tag_indices_score = torch.tensor(0.0)
-            for i, (j, k) in enumerate(
-                zip(tag_indices[:-1], tag_indices[1:], strict=True)
-            ):
+            for i, (j, k) in enumerate(zip(tag_indices[:-1], tag_indices[1:])):
                 tag_indices_score += log_potentials[b, i, j, k]
             log_Z[b] = torch.logaddexp(log_Z[b], tag_indices_score)
     return log_Z
 
 
 def compute_best_tag_indices_by_brute_force(
     log_potentials: torch.Tensor,
@@ -46,17 +45,15 @@
     max_scores = torch.tensor([NINF] * batch_size)
     for b in range(batch_size):
         max_score = torch.tensor(NINF)
         for tag_indices in iterate_possible_tag_indices(sequence_length, num_tags):
             tag_indices_score = (
                 log_potentials[b, 0, tag_indices[0], tag_indices[0]].detach().clone()
             )
-            for i, (j, k) in enumerate(
-                zip(tag_indices[:-1], tag_indices[1:], strict=True), 1
-            ):
+            for i, (j, k) in enumerate(zip(tag_indices[:-1], tag_indices[1:]), 1):
                 tag_indices_score += log_potentials[b, i, j, k]
             if tag_indices_score.gt(max_score):
                 # Ignore the dummy initial state
                 best_tag_indices[b] = torch.tensor(tag_indices)
                 max_score = tag_indices_score
         max_scores[b] = max_score
     return max_scores, best_tag_indices
@@ -111,15 +108,15 @@
 ) -> bool:
     num_tags = used_mask.size(-1)
     lengths = mask.sum(dim=-1)
     for b, real_sequence_length in enumerate(lengths):
         # only (i, j) is True, otherwise False
         tags = tag_indices[b, :real_sequence_length].tolist()
         tags = [tags[0]] + tags
-        for pos, (i, j) in enumerate(zip(tags[:-1], tags[1:], strict=True)):
+        for pos, (i, j) in enumerate(zip(tags[:-1], tags[1:])):
             if not used_mask[b, pos, i, j]:
                 return False
             for x in range(num_tags):
                 for y in range(num_tags):
                     if x == i and y == j:
                         continue
                     if used_mask[b, pos, x, y]:
@@ -140,15 +137,15 @@
     partial_index: int,
 ) -> bool:
     num_tags = log_potentials.size(-1)
     lengths = mask.sum(dim=-1)
     for b, real_sequence_length in enumerate(lengths):
         tags = tag_indices[b, :real_sequence_length].tolist()
         tags = [tags[0]] + tags
-        for pos, (i, j) in enumerate(zip(tags[:-1], tags[1:], strict=True)):
+        for pos, (i, j) in enumerate(zip(tags[:-1], tags[1:])):
             if i == partial_index and j == partial_index:
                 x = constrained_log_potentials[b, pos]
                 y = log_potentials[b, pos]
             elif i == partial_index:
                 for n in range(num_tags):
                     if n == j:
                         continue
```

### Comparing `pytorch_partial_tagger-0.1.2/tests/crf/test_functional.py` & `pytorch_partial_tagger-0.1.3/tests/crf/test_functional.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from unittest.mock import patch
 
 import pytest
 import torch
+
 from partial_tagger.crf import NINF
 from partial_tagger.crf import functional as F
 
 from .. import helpers
 
 
 def test_log_likelihood_valid_as_probability(test_data_small: tuple) -> None:
```

### Comparing `pytorch_partial_tagger-0.1.2/tests/crf/test_nn.py` & `pytorch_partial_tagger-0.1.3/tests/crf/test_nn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
 import torch
+
 from partial_tagger.crf.nn import CRF
 
 from .. import helpers
 
 
 @pytest.fixture
 def crf(num_tags: int) -> CRF:
```

### Comparing `pytorch_partial_tagger-0.1.2/tests/data/test_batch.py` & `pytorch_partial_tagger-0.1.3/tests/data/test_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
 import torch
+from transformers import AutoTokenizer
+
 from partial_tagger.data import CharBasedTags, LabelSet, Span, Tag
 from partial_tagger.data.batch import TransformerBatchFactory
-from transformers import AutoTokenizer
 
 
 @pytest.fixture
 def batch_factory() -> TransformerBatchFactory:
     return TransformerBatchFactory(
         AutoTokenizer.from_pretrained("distilroberta-base"),
         LabelSet({"LOC", "MISC", "ORG", "PER"}),
```

### Comparing `pytorch_partial_tagger-0.1.2/tests/data/test_core.py` & `pytorch_partial_tagger-0.1.3/tests/data/test_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+
 from partial_tagger.data import LabelSet, Span, TokenizedText
 
 
 @pytest.fixture
 def tokenized_text() -> TokenizedText:
     # Tokenized by RoBERTa
     return TokenizedText(
```

### Comparing `pytorch_partial_tagger-0.1.2/.gitignore` & `pytorch_partial_tagger-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.2/LICENSE` & `pytorch_partial_tagger-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.2/README.md` & `pytorch_partial_tagger-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 
 from partial_tagger.data import CharBasedTags
 from partial_tagger.training import Trainer
 from partial_tagger.utils import Metric, create_tag
 ```
 
 Prepare your own datasets.
-Each item of dataset must have a string and tags. A string represents the `text` below.
+Each item of dataset must have a string and tags. A string represents `text` below.
 Tags represent a collection of tags, where each tag has a start, a length, and a label, which are defined as `tags` below.
 A start represents a position in `text` where a tag starts.
-A length represents a distance in `text` between between the beginning of a tag and the end of a tag.
+A length represents a distance in `text` between the beginning of a tag and the end of a tag.
 A label represents what you want to assign to a span of `text` defined by a start and a length.
 
 ```py
 from partial_tagger.utils import create_tags, CharBasedTags
 
 
 text = "Tokyo is the capital of Japan."
@@ -40,27 +40,28 @@
 ```
 
 Here, you would train your tagger and evaluate its performance.
 
 You could train your own tagger by initializing `Trainer` and passing datasets to it.
 After training, `trainer` gives you `Recognizer` object which predicts character-based tags from given texts.
 
-Then you could evaluate the performance of your tagger using `Metric` as below.
+You could evaluate the performance of your tagger using `Metric` as below.
 
 
 ```py
 
 device = torch.device("cuda")
 
 trainer = Trainer()
 recognizer = trainer(train_dataset, validation_dataset, device)
 
 texts, ground_truths = zip(*test_dataset, strict=True)
 
-predictions = recognizer(texts)
+batch_size = 15
+predictions = recognizer(texts, batch_size, device)
 
 metric = Metric()
 metric(predictions, ground_truths)
 
 print(metric.get_scores())  # Display F1-score, Precision, Recall
 ```
```

### Comparing `pytorch_partial_tagger-0.1.2/PKG-INFO` & `pytorch_partial_tagger-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 Metadata-Version: 2.1
 Name: pytorch-partial-tagger
-Version: 0.1.2
+Version: 0.1.3
 Summary: Sequence Tagger for Partially Annotated Dataset in PyTorch
 Project-URL: Homepage, https://github.com/yasufumy/pytorch-partial-tagger
 Author-email: Yasufumi Taniguchi <yasufumi.taniguchi@gmail.com>
 License: MIT
 License-File: LICENSE
-Requires-Python: >=3.10
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Requires-Dist: torch>=2.0.1
 Requires-Dist: transformers>=4.29.2
 Provides-Extra: dev
 Requires-Dist: black>=23.3.0; extra == 'dev'
 Requires-Dist: mypy>=1.3.0; extra == 'dev'
 Requires-Dist: pytest-cov>=4.1.0; extra == 'dev'
 Requires-Dist: pytest>=7.3.1; extra == 'dev'
@@ -31,18 +36,18 @@
 
 from partial_tagger.data import CharBasedTags
 from partial_tagger.training import Trainer
 from partial_tagger.utils import Metric, create_tag
 ```
 
 Prepare your own datasets.
-Each item of dataset must have a string and tags. A string represents the `text` below.
+Each item of dataset must have a string and tags. A string represents `text` below.
 Tags represent a collection of tags, where each tag has a start, a length, and a label, which are defined as `tags` below.
 A start represents a position in `text` where a tag starts.
-A length represents a distance in `text` between between the beginning of a tag and the end of a tag.
+A length represents a distance in `text` between the beginning of a tag and the end of a tag.
 A label represents what you want to assign to a span of `text` defined by a start and a length.
 
 ```py
 from partial_tagger.utils import create_tags, CharBasedTags
 
 
 text = "Tokyo is the capital of Japan."
@@ -59,27 +64,28 @@
 ```
 
 Here, you would train your tagger and evaluate its performance.
 
 You could train your own tagger by initializing `Trainer` and passing datasets to it.
 After training, `trainer` gives you `Recognizer` object which predicts character-based tags from given texts.
 
-Then you could evaluate the performance of your tagger using `Metric` as below.
+You could evaluate the performance of your tagger using `Metric` as below.
 
 
 ```py
 
 device = torch.device("cuda")
 
 trainer = Trainer()
 recognizer = trainer(train_dataset, validation_dataset, device)
 
 texts, ground_truths = zip(*test_dataset, strict=True)
 
-predictions = recognizer(texts)
+batch_size = 15
+predictions = recognizer(texts, batch_size, device)
 
 metric = Metric()
 metric(predictions, ground_truths)
 
 print(metric.get_scores())  # Display F1-score, Precision, Recall
 ```
```

