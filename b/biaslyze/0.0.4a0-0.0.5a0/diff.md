# Comparing `tmp/biaslyze-0.0.4a0.tar.gz` & `tmp/biaslyze-0.0.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biaslyze-0.0.4a0.tar", max compression
+gzip compressed data, was "biaslyze-0.0.5a0.tar", max compression
```

## Comparing `biaslyze-0.0.4a0.tar` & `biaslyze-0.0.5a0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1495 2023-04-21 09:03:51.243806 biaslyze-0.0.4a0/LICENSE
--rw-r--r--   0        0        0     1760 2023-05-25 09:47:41.505257 biaslyze-0.0.4a0/README.md
--rw-r--r--   0        0        0        0 2023-03-09 11:50:10.881651 biaslyze-0.0.4a0/biaslyze/__init__.py
--rw-r--r--   0        0        0     6931 2023-05-25 09:48:01.453043 biaslyze-0.0.4a0/biaslyze/_plotting.py
--rw-r--r--   0        0        0      220 2023-05-19 13:34:56.156524 biaslyze-0.0.4a0/biaslyze/bias_detectors/__init__.py
--rw-r--r--   0        0        0    12739 2023-05-25 10:16:50.171622 biaslyze-0.0.4a0/biaslyze/bias_detectors/counterfactual_biasdetector.py
--rw-r--r--   0        0        0     5547 2023-05-25 09:48:01.425044 biaslyze-0.0.4a0/biaslyze/bias_detectors/lime_biasdetector.py
--rw-r--r--   0        0        0     1831 2023-05-19 13:34:56.156524 biaslyze-0.0.4a0/biaslyze/concept_detectors.py
--rw-r--r--   0        0        0    64680 2023-05-19 13:34:56.156524 biaslyze-0.0.4a0/biaslyze/concepts.py
--rw-r--r--   0        0        0    13052 2023-05-25 10:16:50.203622 biaslyze-0.0.4a0/biaslyze/results/counterfactual_detection_results.py
--rw-r--r--   0        0        0     4990 2023-05-25 08:34:39.793839 biaslyze-0.0.4a0/biaslyze/results/lime_detection_results.py
--rw-r--r--   0        0        0     1246 2023-05-25 12:53:25.993306 biaslyze-0.0.4a0/pyproject.toml
--rw-r--r--   0        0        0     2866 1970-01-01 00:00:00.000000 biaslyze-0.0.4a0/setup.py
--rw-r--r--   0        0        0     3042 1970-01-01 00:00:00.000000 biaslyze-0.0.4a0/PKG-INFO
+-rw-r--r--   0        0        0     1495 2023-04-21 09:03:51.243806 biaslyze-0.0.5a0/LICENSE
+-rw-r--r--   0        0        0     2878 2023-05-26 17:13:34.903042 biaslyze-0.0.5a0/README.md
+-rw-r--r--   0        0        0        0 2023-03-09 11:50:10.881651 biaslyze-0.0.5a0/biaslyze/__init__.py
+-rw-r--r--   0        0        0     6931 2023-05-26 17:13:34.903042 biaslyze-0.0.5a0/biaslyze/_plotting.py
+-rw-r--r--   0        0        0      220 2023-05-26 17:13:34.903042 biaslyze-0.0.5a0/biaslyze/bias_detectors/__init__.py
+-rw-r--r--   0        0        0    12495 2023-06-01 13:06:40.492303 biaslyze-0.0.5a0/biaslyze/bias_detectors/counterfactual_biasdetector.py
+-rw-r--r--   0        0        0     5547 2023-05-26 17:13:34.903042 biaslyze-0.0.5a0/biaslyze/bias_detectors/lime_biasdetector.py
+-rw-r--r--   0        0        0     1831 2023-05-26 17:13:34.903042 biaslyze-0.0.5a0/biaslyze/concept_detectors.py
+-rw-r--r--   0        0        0    64680 2023-05-26 17:13:34.903042 biaslyze-0.0.5a0/biaslyze/concepts.py
+-rw-r--r--   0        0        0    12925 2023-05-26 17:13:34.903042 biaslyze-0.0.5a0/biaslyze/results/counterfactual_detection_results.py
+-rw-r--r--   0        0        0     4990 2023-05-26 17:13:34.903042 biaslyze-0.0.5a0/biaslyze/results/lime_detection_results.py
+-rw-r--r--   0        0        0     1644 2023-06-01 13:32:30.961900 biaslyze-0.0.5a0/pyproject.toml
+-rw-r--r--   0        0        0     4502 1970-01-01 00:00:00.000000 biaslyze-0.0.5a0/setup.py
+-rw-r--r--   0        0        0     4831 1970-01-01 00:00:00.000000 biaslyze-0.0.5a0/PKG-INFO
```

### Comparing `biaslyze-0.0.4a0/LICENSE` & `biaslyze-0.0.5a0/LICENSE`

 * *Files identical despite different names*

### Comparing `biaslyze-0.0.4a0/README.md` & `biaslyze-0.0.5a0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,21 @@
-# biaslyze
-The NLP Bias Identification Toolkit
+# biaslyze - The NLP Bias Identification Toolkit
 
+Bias is often subtle and difficult to detect in NLP models, as the protected attributes are less obvious and can take many forms in language (e.g. proxies, double meanings, ambiguities etc.). Therefore, technical bias testing is a key step in avoiding algorithmically mediated discrimination. However, it is currently conducted too rarely due to the effort involved, missing resources or lack of awareness for the problem.
 
-## Usage example
+Biaslyze helps to get started with the analysis of bias within NLP models and offers a concrete entry point for further impact assessments and mitigation measures. Especially for young developers, students and teams with limited resources, our toolbox offers a low-effort approach to bias testing in NLP use cases.
+
+## Installation
+
+Installation can be done using pypi:
+```bash
+pip install biaslyze
+```
+
+## Quickstart
 
 ```python
 from biaslyze.bias_detectors import CounterfactualBiasDetector
 
 bias_detector = CounterfactualBiasDetector()
 
 # detect bias in the model based on the given texts
@@ -23,14 +32,17 @@
 detection_res.visualize_counterfactual_scores(concept="religion", top_n=10)
 ```
 
 Example output:
 ![](resources/hatespeech_dl_scores_religion.png)
 
 
+You can see a more detailed example in the [tutorial](tutorials/tutorial-toxic-comments/).
+
+
 ## Development setup
 
 - First you need to install poetry to manage your python environment: https://python-poetry.org/docs/#installation
 - Run `make install` to install the dependencies and get the spacy basemodels.
 - Now you can use `biaslyze` in your jupyter notebooks.
 
 
@@ -56,7 +68,10 @@
 
 ## Contributing
 
 Follow the google style guide for python: https://google.github.io/styleguide/pyguide.html
 
 This project uses black, isort and ruff to enforce style. Apply it by running `make style` and `make lint`.
 
+## Acknowledgements
+
+* Funded from March 2023 until August 2023 by ![logos of the "Bundesministerium für Bildung und Forschung", Prodotype Fund and OKFN-Deutschland](resources/pf_funding_logos.svg)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `biaslyze-0.0.4a0/biaslyze/_plotting.py` & `biaslyze-0.0.5a0/biaslyze/_plotting.py`

 * *Files identical despite different names*

### Comparing `biaslyze-0.0.4a0/biaslyze/bias_detectors/counterfactual_biasdetector.py` & `biaslyze-0.0.5a0/biaslyze/bias_detectors/counterfactual_biasdetector.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,31 +2,32 @@
 import random
 from typing import Callable, List, Optional
 
 import numpy as np
 import pandas as pd
 from loguru import logger
 from tqdm import tqdm
+import spacy
 
 from biaslyze.concept_detectors import KeywordConceptDetector
 from biaslyze.concepts import CONCEPTS
 from biaslyze.results.counterfactual_detection_results import (
     CounterfactualConceptResult,
     CounterfactualDetectionResult,
     CounterfactualSample,
 )
 
 
 class CounterfactualBiasDetector:
     """Detect hints of bias by calculating counterfactual token scores for protected concepts.
 
     The counterfactual score is defined as the difference between the predicted
-    p robability score for the original text and the predicted probability score for the counterfactual text.
+    probability score for the original text and the predicted probability score for the counterfactual text.
 
-    $$counterfactual_score = P(x=1|original_text) - P(x=1|counterfactual_text),$$
+    $$counterfactual_score = P(x=1|counterfactual_text) - P(x=1|original_text),$$
 
     where counterfactual text is defined as the original text where a keyword of the given concept is
     replaced by another keyword of the same concept. So a counterfactual_score > 0 means that the
     model is more likely to predict the positive class for the original text than for the counterfactual text.
 
     Usage example:
 
@@ -111,25 +112,28 @@
         results = []
         for concept, concept_keywords in CONCEPTS.items():
             if concepts_to_consider and concept not in concepts_to_consider:
                 continue
             logger.info(f"Processing concept {concept}...")
             score_dict = dict()
 
-            counterfactual_samples = self._extract_counterfactual_concept_samples(
-                texts=detected_texts, concept=concept, labels=labels
+            counterfactual_samples = _extract_counterfactual_concept_samples(
+                texts=detected_texts,
+                concept=concept,
+                tokenizer=self.concept_detector._tokenizer,
+                labels=labels,
             )
             if not counterfactual_samples:
                 logger.warning(f"No samples containing {concept} found. Skipping.")
                 continue
 
             # calculate counterfactual scores for each keyword
             for keyword in tqdm(concept_keywords):
                 # get the counterfactual scores
-                counterfactual_scores = self._calculate_counterfactual_scores(
+                counterfactual_scores = _calculate_counterfactual_scores(
                     bias_keyword=keyword.get("keyword"),
                     predict_func=predict_func,
                     samples=counterfactual_samples,
                     max_counterfactual_samples=max_counterfactual_samples,
                 )
                 # add to score dict
                 score_dict[keyword.get("keyword")] = counterfactual_scores
@@ -159,135 +163,136 @@
                     counterfactual_samples=counterfactual_samples,
                 )
             )
             logger.info("DONE")
 
         return CounterfactualDetectionResult(concept_results=results)
 
-    def _extract_counterfactual_concept_samples(
-        self, concept: str, texts: List[str], labels: Optional[List[str]] = None
-    ) -> List[CounterfactualSample]:
-        """Extract counterfactual samples for a given concept from a list of texts.
 
-        A counterfactual sample is defined as a text where a keyword of the
-        given concept is replaced by another keyword of the same concept.
-
-        Args:
-            concept: The concept to extract counterfactual samples for.
-            texts: The texts to extract counterfactual samples from.
-            labels: Optional. Used to add labels to the counterfactual results.
-        """
-        counterfactual_samples = []
-        original_texts = []
-        text_representations = self.concept_detector._tokenizer.pipe(texts)
-        concept_keywords = set(
-            [keyword.get("keyword") for keyword in CONCEPTS[concept]]
+def _extract_counterfactual_concept_samples(
+    concept: str,
+    texts: List[str],
+    tokenizer: spacy.tokenizer.Tokenizer,
+    labels: Optional[List[str]] = None,
+) -> List[CounterfactualSample]:
+    """Extract counterfactual samples for a given concept from a list of texts.
+
+    A counterfactual sample is defined as a text where a keyword of the
+    given concept is replaced by another keyword of the same concept.
+
+    Args:
+        concept: The concept to extract counterfactual samples for.
+        texts: The texts to extract counterfactual samples from.
+        tokenizer: The tokenizer to use for tokenization.
+        labels: Optional. Used to add labels to the counterfactual results.
+    """
+    counterfactual_samples = []
+    original_texts = []
+    text_representations = tokenizer.pipe(texts)
+    concept_keywords = set([keyword.get("keyword") for keyword in CONCEPTS[concept]])
+    for idx, (text, text_representation) in tqdm(
+        enumerate(zip(texts, text_representations)), total=len(texts)
+    ):
+        present_keywords = list(
+            keyword
+            for keyword in concept_keywords
+            if keyword in (token.text.lower() for token in text_representation)
         )
-        for idx, (text, text_representation) in tqdm(
-            enumerate(zip(texts, text_representations)), total=len(texts)
-        ):
-            present_keywords = list(
-                keyword
-                for keyword in concept_keywords
-                if keyword in (token.text.lower() for token in text_representation)
-            )
-            if present_keywords:
-                original_texts.append(text)
-                for orig_keyword in present_keywords:
-                    for concept_keyword in concept_keywords:
-                        resampled_text = "".join(
-                            [
-                                concept_keyword + token.whitespace_
-                                if token.text.lower() == orig_keyword.lower()
-                                else token.text + token.whitespace_
-                                for token in text_representation
-                            ]
+        if present_keywords:
+            original_texts.append(text)
+            for orig_keyword in present_keywords:
+                for concept_keyword in concept_keywords:
+                    resampled_text = "".join(
+                        [
+                            concept_keyword + token.whitespace_
+                            if token.text.lower() == orig_keyword.lower()
+                            else token.text + token.whitespace_
+                            for token in text_representation
+                        ]
+                    )
+                    counterfactual_samples.append(
+                        CounterfactualSample(
+                            text=resampled_text,
+                            orig_keyword=orig_keyword,
+                            keyword=concept_keyword,
+                            concept=concept,
+                            tokenized=text_representation,
+                            label=labels[idx] if labels else None,
+                            source_text=text,
                         )
-                        counterfactual_samples.append(
-                            CounterfactualSample(
-                                text=resampled_text,
-                                orig_keyword=orig_keyword,
-                                keyword=concept_keyword,
-                                concept=concept,
-                                tokenized=text_representation,
-                                label=labels[idx] if labels else None,
-                                source_text=text,
-                            )
-                        )
-        logger.info(
-            f"Extracted {len(counterfactual_samples)} counterfactual sample texts for concept {concept} from {len(original_texts)} original texts."
+                    )
+    logger.info(
+        f"Extracted {len(counterfactual_samples)} counterfactual sample texts for concept {concept} from {len(original_texts)} original texts."
+    )
+    return counterfactual_samples
+
+
+def _calculate_counterfactual_scores(
+    bias_keyword: str,
+    predict_func: Callable,
+    samples: List[CounterfactualSample],
+    max_counterfactual_samples: int = None,
+    positive_classes: Optional[List] = None,
+) -> np.ndarray:
+    """Calculate the counterfactual score for a bias keyword given samples.
+
+    Args:
+        bias_keyword: The keyword to calculate the counterfactual score for.
+        predict_func: Function to run the texts through the model and get probabilities as outputs.
+        samples: A list of CounterfactualSample objects.
+        max_counterfactual_samples: The maximum number of counterfactual samples to use.
+        positive_classes: A list of classes that are considered positive.
+
+    TODO: If `positive_classes` is given, all other classes are considered non-positive and positive and negative outcomes are compared.
+    TODO: introduce neutral classes.
+
+    Returns:
+        A numpy array of differences between the original predictions and the predictions for the counterfactual samples.
+        We call this the **counterfactual score**:  counterfactual_score = P(x=1|counterfactual_text) - P(x=1|original_text).
+
+    Raises:
+        ValueError: If `positive_classes` is given but the model is not a binary classifier.
+        IndexError: If `positive_classes` is given but the model does not have the given classes.
+    """
+    # filter samples for the given bias keyword
+    original_texts = [
+        sample.source_text for sample in samples if (sample.keyword == bias_keyword)
+    ]
+    counterfactual_texts = [
+        sample.text for sample in samples if (sample.keyword == bias_keyword)
+    ]
+
+    # if max_counterfactual_samples is given, only use a random sample of the counterfactual texts
+    if max_counterfactual_samples:
+        original_texts, counterfactual_texts = zip(
+            *random.sample(
+                list(zip(original_texts, counterfactual_texts)),
+                max_counterfactual_samples,
+            )
+        )
+    # predict the scores for the original texts and the counterfactual texts
+    original_scores = predict_func(original_texts)
+    predicted_scores = predict_func(counterfactual_texts)
+
+    # check if the model is a binary classifier
+    if (not positive_classes) and (len(original_scores[0]) != 2):
+        raise NotImplementedError(
+            "Multi-class classification is not yet supported for counterfactual detection."
+            "Please use a binary classifier."
+            "If you are using a multi-class classifier, please specify the positive classes."
         )
-        return counterfactual_samples
-
-    def _calculate_counterfactual_scores(
-        self,
-        bias_keyword: str,
-        predict_func: Callable,
-        samples: List,
-        max_counterfactual_samples: int = None,
-        positive_classes: Optional[List] = None,
-    ) -> np.ndarray:
-        """Calculate the counterfactual score for a bias keyword given samples.
-
-        Args:
-            bias_keyword: The keyword to calculate the counterfactual score for.
-            predict_func: Function to run the texts through the model and get probabilities as outputs.
-            samples: A list of CounterfactualSample objects.
-            max_counterfactual_samples: The maximum number of counterfactual samples to use.
-            positive_classes: A list of classes that are considered positive.
-
-        TODO: If `positive_classes` is given, all other classes are considered non-positive and positive and negative outcomes are compared.
-        TODO: introduce neutral classes.
-
-        Returns:
-            A numpy array of differences between the original predictions and the predictions for the counterfactual samples.
-            We call this the **counterfactual score**.
-
-        Raises:
-            ValueError: If `positive_classes` is given but the model is not a binary classifier.
-            IndexError: If `positive_classes` is given but the model does not have the given classes.
-        """
-        # filter samples for the given bias keyword
-        original_texts = [
-            sample.source_text for sample in samples if (sample.keyword == bias_keyword)
-        ]
-        counterfactual_texts = [
-            sample.text for sample in samples if (sample.keyword == bias_keyword)
-        ]
 
-        # if max_counterfactual_samples is given, only use a random sample of the counterfactual texts
-        if max_counterfactual_samples:
-            original_texts, counterfactual_texts = zip(
-                *random.sample(
-                    list(zip(original_texts, counterfactual_texts)),
-                    max_counterfactual_samples,
-                )
-            )
-        # predict the scores for the original texts and the counterfactual texts
-        original_scores = predict_func(original_texts)
-        predicted_scores = predict_func(counterfactual_texts)
-
-        # check if the model is a binary classifier
-        if (not positive_classes) and (len(original_scores[0]) != 2):
-            raise NotImplementedError(
-                "Multi-class classification is not yet supported for counterfactual detection."
-                "Please use a binary classifier."
-                "If you are using a multi-class classifier, please specify the positive classes."
+    # calculate score differences
+    if positive_classes:
+        # sum up the scores for the positive classes and take the difference
+        try:
+            score_diffs = (
+                np.array(predicted_scores[:, positive_classes]).sum(axis=1),
+                -np.array(original_scores[:, positive_classes]).sum(axis=1),
             )
-
-        # calculate score differences
-        if positive_classes:
-            # sum up the scores for the positive classes and take the difference
-            try:
-                score_diffs = (
-                    np.array(original_scores[:, positive_classes]).sum(axis=1)
-                    - np.array(predicted_scores[:, positive_classes]).sum(axis=1),
-                )
-            except IndexError:
-                raise IndexError(
-                    f"Positive classes {positive_classes} not found in predictions."
-                )
-        else:
-            score_diffs = np.array(original_scores[:, 1]) - np.array(
-                predicted_scores[:, 1]
+        except IndexError:
+            raise IndexError(
+                f"Positive classes {positive_classes} not found in predictions."
             )
-        return score_diffs
+    else:
+        score_diffs = np.array(predicted_scores[:, 1]) - np.array(original_scores[:, 1])
+    return score_diffs
```

### Comparing `biaslyze-0.0.4a0/biaslyze/bias_detectors/lime_biasdetector.py` & `biaslyze-0.0.5a0/biaslyze/bias_detectors/lime_biasdetector.py`

 * *Files identical despite different names*

### Comparing `biaslyze-0.0.4a0/biaslyze/concept_detectors.py` & `biaslyze-0.0.5a0/biaslyze/concept_detectors.py`

 * *Files identical despite different names*

### Comparing `biaslyze-0.0.4a0/biaslyze/concepts.py` & `biaslyze-0.0.5a0/biaslyze/concepts.py`

 * *Files identical despite different names*

### Comparing `biaslyze-0.0.4a0/biaslyze/results/counterfactual_detection_results.py` & `biaslyze-0.0.5a0/biaslyze/results/counterfactual_detection_results.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,17 +173,14 @@
         for sample, (_, score) in zip(original_samples, dataf.iterrows()):
             counterfactual_plot_dict[sample.orig_keyword].extend(score.tolist())
 
         counterfactual_df = pd.DataFrame(
             dict([(k, pd.Series(v)) for k, v in counterfactual_plot_dict.items()])
         )
 
-        # change the sign of the scores in the dataframe
-        counterfactual_df = counterfactual_df.applymap(lambda x: -x)
-
         # plot
         ax = _plot_box_plot(counterfactual_df, top_n=top_n)
         ax.set_title(
             f"Distribution of counterfactual scores for concept '{concept}' by original keyword\nsorted by median score"
         )
         ax.set_xlabel(
             "Counterfactual scores - differences from zero indicate the direction of bias."
```

### Comparing `biaslyze-0.0.4a0/biaslyze/results/lime_detection_results.py` & `biaslyze-0.0.5a0/biaslyze/results/lime_detection_results.py`

 * *Files identical despite different names*

