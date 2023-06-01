# Comparing `tmp/docs-ranking-metrics-0.0.4.dev2.tar.gz` & `tmp/docs-ranking-metrics-0.0.4.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docs-ranking-metrics-0.0.4.dev2.tar", last modified: Fri May 19 16:10:03 2023, max compression
+gzip compressed data, was "dist\docs-ranking-metrics-0.0.4.dev3.tar", last modified: Thu Jun  1 05:54:32 2023, max compression
```

## Comparing `docs-ranking-metrics-0.0.4.dev2.tar` & `docs-ranking-metrics-0.0.4.dev3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 16:10:03.852362 docs-ranking-metrics-0.0.4.dev2/
--rw-rw-rw-   0        0        0     2332 2023-05-19 16:10:03.852362 docs-ranking-metrics-0.0.4.dev2/PKG-INFO
--rw-rw-rw-   0        0        0     2694 2023-05-19 13:43:59.000000 docs-ranking-metrics-0.0.4.dev2/README.md
--rw-rw-rw-   0        0        0       97 2023-05-19 13:43:59.000000 docs-ranking-metrics-0.0.4.dev2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-19 16:10:03.852362 docs-ranking-metrics-0.0.4.dev2/setup.cfg
--rw-rw-rw-   0        0        0     8957 2023-05-19 13:43:59.000000 docs-ranking-metrics-0.0.4.dev2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 16:10:03.843389 docs-ranking-metrics-0.0.4.dev2/src/
-drwxrwxrwx   0        0        0        0 2023-05-19 16:10:03.845383 docs-ranking-metrics-0.0.4.dev2/src/docs_ranking_metrics/
--rw-rw-rw-   0        0        0      147 2023-05-19 16:10:00.000000 docs-ranking-metrics-0.0.4.dev2/src/docs_ranking_metrics/__init__.py
--rw-rw-rw-   0        0        0     9860 2023-05-19 13:43:59.000000 docs-ranking-metrics-0.0.4.dev2/src/docs_ranking_metrics/evaluation_metrics.py
--rw-rw-rw-   0        0        0     1535 2023-05-19 14:39:57.000000 docs-ranking-metrics-0.0.4.dev2/src/docs_ranking_metrics/models.py
--rw-rw-rw-   0        0        0     9668 2023-05-19 16:10:00.000000 docs-ranking-metrics-0.0.4.dev2/src/docs_ranking_metrics/ranking_metrics.py
-drwxrwxrwx   0        0        0        0 2023-05-19 16:10:03.852362 docs-ranking-metrics-0.0.4.dev2/src/docs_ranking_metrics.egg-info/
--rw-rw-rw-   0        0        0     2332 2023-05-19 16:10:03.000000 docs-ranking-metrics-0.0.4.dev2/src/docs_ranking_metrics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      435 2023-05-19 16:10:03.000000 docs-ranking-metrics-0.0.4.dev2/src/docs_ranking_metrics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 16:10:03.000000 docs-ranking-metrics-0.0.4.dev2/src/docs_ranking_metrics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2023-05-19 16:10:03.000000 docs-ranking-metrics-0.0.4.dev2/src/docs_ranking_metrics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-19 16:10:03.000000 docs-ranking-metrics-0.0.4.dev2/src/docs_ranking_metrics.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 05:54:32.784800 docs-ranking-metrics-0.0.4.dev3/
+-rw-rw-rw-   0        0        0     3432 2023-06-01 05:54:32.783801 docs-ranking-metrics-0.0.4.dev3/PKG-INFO
+-rw-rw-rw-   0        0        0     2694 2023-06-01 05:54:20.000000 docs-ranking-metrics-0.0.4.dev3/README.md
+-rw-rw-rw-   0        0        0       97 2023-05-31 06:23:53.000000 docs-ranking-metrics-0.0.4.dev3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-01 05:54:32.784800 docs-ranking-metrics-0.0.4.dev3/setup.cfg
+-rw-rw-rw-   0        0        0     8957 2023-05-31 06:23:53.000000 docs-ranking-metrics-0.0.4.dev3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:54:32.639148 docs-ranking-metrics-0.0.4.dev3/src/
+drwxrwxrwx   0        0        0        0 2023-06-01 05:54:32.696510 docs-ranking-metrics-0.0.4.dev3/src/docs_ranking_metrics/
+-rw-rw-rw-   0        0        0      195 2023-06-01 05:51:41.000000 docs-ranking-metrics-0.0.4.dev3/src/docs_ranking_metrics/__init__.py
+-rw-rw-rw-   0        0        0    17858 2023-06-01 04:47:09.000000 docs-ranking-metrics-0.0.4.dev3/src/docs_ranking_metrics/evaluation_metrics.py
+-rw-rw-rw-   0        0        0     1534 2023-06-01 04:57:10.000000 docs-ranking-metrics-0.0.4.dev3/src/docs_ranking_metrics/models.py
+-rw-rw-rw-   0        0        0    16333 2023-06-01 04:57:10.000000 docs-ranking-metrics-0.0.4.dev3/src/docs_ranking_metrics/ranking_metrics.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:54:32.781799 docs-ranking-metrics-0.0.4.dev3/src/docs_ranking_metrics.egg-info/
+-rw-rw-rw-   0        0        0     3432 2023-06-01 05:54:32.000000 docs-ranking-metrics-0.0.4.dev3/src/docs_ranking_metrics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      435 2023-06-01 05:54:32.000000 docs-ranking-metrics-0.0.4.dev3/src/docs_ranking_metrics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 05:54:32.000000 docs-ranking-metrics-0.0.4.dev3/src/docs_ranking_metrics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2023-06-01 05:54:32.000000 docs-ranking-metrics-0.0.4.dev3/src/docs_ranking_metrics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-01 05:54:32.000000 docs-ranking-metrics-0.0.4.dev3/src/docs_ranking_metrics.egg-info/top_level.txt
```

### Comparing `docs-ranking-metrics-0.0.4.dev2/PKG-INFO` & `docs-ranking-metrics-0.0.4.dev3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 Metadata-Version: 2.1
 Name: docs-ranking-metrics
-Version: 0.0.4.dev2
+Version: 0.0.4.dev3
 Summary: The package contains functions for calculating ranking metrics
 Home-page: https://github.com/betepok506/RankingMetrics
 Author: Andrey Rotanov
 Author-email: rotanov07@mail.ru
+License: UNKNOWN
 Keywords: test
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: test
 
 # Описание
-Данный репозиторий содержит реализацию алгоритмов ранжирования Bm25, LaBSE 
+Данный репозиторий содержит реализацию алгоритмов ранжирования Bm25, LaBSE, MsMarcoST, MsMarcoCE 
 с подсчетом метрик: 
 * Top@1;
 * Top@3;
 * Top@5;
 * Средняя позиция в выдачах (AverageLoc);
-* Оценка как часто фейковый документ выше релевантных (FDARO)
+* Cредняя относительная позиция в выдачах (AverageRelLoc);
+* Оценка как часто фейковый документ выше всех релевантных (FDARO@v1);
+* Оценка как часто фейковый документ выше хотя бы одного релевантного (FDARO@v2);
+* Частота попадания фейкового документа в топ 25% (UpQuartile).
+
 
 
 # Установка
 Для установки пакета воспользуйтесь командой
 ```
 pip install docs-ranking-metrics
 ```
@@ -50,14 +56,16 @@
 labels - метки документов
 '''
 rank_metrics.update(query, sentences, labels)
 
 ...
 # Получение значений подсчитанных метрик ввиде словаря
 rank_metrics.get()
+# Получение значений метрик при помощи функции show_metrics
+rank_metrics.show_metrics()
 ```
 
 Возможный вывод метода get:
 ```
 {
     'LaBSE_AverageLoc': 10.5, 
     'Bm25_AverageLoc': 1.13513, 
@@ -67,7 +75,25 @@
     'Bm25_Top@1': 0.91891, 
     'Bm25_Top@3': 1.0, 
     'Bm25_Top@5': 1.0, 
     'LaBSE_FDARO': 0.6216, 
     'Bm25_FDARO': 1.0
 }
 ```
+
+Возможный вывод метода show_metrics():
+```
+LaBSE_AverageLoc: 4.5   Bm25_AverageLoc: 3.0   
+-----------------------------
+LaBSE_AverageRelLoc: 0.75   Bm25_AverageRelLoc: 0.5   
+-----------------------------
+LaBSE_Top@1: 0.0   Bm25_Top@1: 0.5   
+LaBSE_Top@3: 0.5   Bm25_Top@3: 0.5   
+LaBSE_Top@5: 0.5   Bm25_Top@5: 1.0   
+-----------------------------
+LaBSE_FDARO@v1: 0.5   Bm25_FDARO@v1: 0.5   
+LaBSE_FDARO@v2: 0.5   Bm25_FDARO@v2: 0.5   
+-----------------------------
+LaBSE_UpQuartile: 0.5   Bm25_UpQuartile: 0.5 
+```
+
+
```

### Comparing `docs-ranking-metrics-0.0.4.dev2/README.md` & `docs-ranking-metrics-0.0.4.dev3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,11 +37,11 @@
 Будет запущен docker-контейнер, который сгенерирует документацию в папку `docs`.
 
 # Улучшения
 
 Что можно сделать (идеи приветствуются):
 
 - [X] Исправить подсчет метрик под документы разной релевантности
-- [ ] Внедрить модель https://huggingface.co/cross-encoder/ms-marco-MiniLM-L-6-v2
-- [ ] Придумать дополнительные метрики
+- [X] Внедрить модель https://huggingface.co/cross-encoder/ms-marco-MiniLM-L-6-v2
+- [X] Придумать дополнительные метрики
 - [X] Завернуть все в пакет
 - [X] Написать тесты, workflows
```

### Comparing `docs-ranking-metrics-0.0.4.dev2/setup.py` & `docs-ranking-metrics-0.0.4.dev3/setup.py`

 * *Files identical despite different names*

### Comparing `docs-ranking-metrics-0.0.4.dev2/src/docs_ranking_metrics/models.py` & `docs-ranking-metrics-0.0.4.dev3/src/docs_ranking_metrics/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                                                                     memory_limit=1024)])
         self.model = hub.load("https://tfhub.dev/google/universal-sentence-encoder-multilingual-large/3")
 
     def encode(self, sentences: List[str]):
         """
         Функция для векторизации списка текстов
 
-         Parameters
+        Parameters
         ------------
         sentences: `List[str]`
             Список  текстов
 
         Returns
         ------------
         `List[List[int]]`
```

### Comparing `docs-ranking-metrics-0.0.4.dev2/src/docs_ranking_metrics/ranking_metrics.py` & `docs-ranking-metrics-0.0.4.dev3/src/docs_ranking_metrics/ranking_metrics.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
+import numpy as np
+
 from rank_bm25 import BM25Okapi
 from typing import List, Dict, Tuple, Union
-from sentence_transformers import SentenceTransformer, util
+from sentence_transformers import SentenceTransformer, util, CrossEncoder
 from .evaluation_metrics import (
-    TopK, AverageLoc, FDARO
+    TopK, AverageLoc, FDARO, UpQuartile, AverageRelLoc
 )
 from .models import ModelUSE
-import tensorflow as tf
-from tensorflow import convert_to_tensor
 import torch
 
 class Bm25:
     """Класс метрики ранжирования bm25"""
 
     def __init__(self):
         pass
@@ -134,14 +134,124 @@
         Returns
         ------------
         `List[Tuple[float, int]]`
             Отсортированный список ранжируемых элементов по релевантности
         """
         return sorted([item for item in zip(scores, labels)], key=lambda x: x[0], reverse=True)
 
+
+
+class MsMarcoST:
+    """Класс метрики ранжирования MS MARCO из sentence-transformers"""
+
+    def __init__(self) -> None:
+        self.model = SentenceTransformer('sentence-transformers/msmarco-bert-base-dot-v5')
+
+    def name(self) -> str:
+        return "MsMarcoST"
+
+    def ranking(self, query: str, sentences: List[str], labels: List[int]) -> List[Tuple[float, int]]:
+        """
+        Функция ранжирования MsMarcoST
+
+        Parameters
+        ------------
+        query: `str`
+            Строка запроса
+        sentences: `List[str]`
+            Список строк текстов
+        labels: `List[int]`
+            Список меток текстов
+
+        Returns
+        ------------
+        `List[Tuple[float, int]]`
+            Список пар, где пара имеет вид (скор, метка), отсортированных по убыванию скоров
+        """
+        query = self.model.encode(query)
+        embeddings = self.model.encode(sentences)
+        scores = util.dot_score(query, embeddings).numpy()[0]
+        scores = self._sorted(scores, labels)
+        return scores
+
+    def _sorted(self, scores: List[float], labels: List[int]) -> List[Tuple[float, int]]:
+        """
+        Функция сортировки оценки и лейблов
+
+        Parameters
+        ------------
+        scores: `List[float]`
+            Массив оценок ранка присвоенных ранкером
+        labels: `List[int]`
+            Массив меток
+
+        Returns
+        ------------
+        `List[Tuple[float, int]]`
+            Отсортированный список ранжируемых элементов по релевантности
+        """
+        return sorted([item for item in zip(scores, labels)], key=lambda x: x[0], reverse=True)
+
+
+class MsMarcoCE:
+    """
+    Класс метрики ранжирования MS MARCO из cross-encoder.
+    Данная метрика более устойчива к кейсам, когда пассаж полностью повторяет запрос.
+    """
+
+    def __init__(self) -> None:
+        self.model = CrossEncoder('cross-encoder/ms-marco-TinyBERT-L-2-v2', max_length=512)
+
+    def name(self) -> str:
+        return "MsMarcoCE"
+
+    def ranking(self, query: str, sentences: List[str], labels: List[int]) -> List[Tuple[float, int]]:
+        """
+        Функция ранжирования MsMarcoCE
+
+        Parameters
+        ------------
+        query: `str`
+            Строка запроса
+        sentences: `List[str]`
+            Список строк текстов
+        labels: `List[int]`
+            Список меток текстов
+
+        Returns
+        ------------
+        `List[Tuple[float, int]]`
+            Список пар, где пара имеет вид (скор, метка), отсортированных по убыванию скоров
+        """
+
+        pairs_que_sent = []
+        for sent in sentences:
+            pairs_que_sent.append((query, sent))
+        scores = self.model.predict(pairs_que_sent)
+        scores = self._sorted(scores, labels)
+        return scores
+
+    def _sorted(self, scores: List[float], labels: List[int]) -> List[Tuple[float, int]]:
+        """
+        Функция сортировки оценки и лейблов
+
+        Parameters
+        ------------
+        scores: `List[float]`
+            Массив оценок ранка присвоенных ранкером
+        labels: `List[int]`
+            Массив меток
+
+        Returns
+        ------------
+        `List[Tuple[float, int]]`
+            Отсортированный список ранжируемых элементов по релевантности
+        """
+        return sorted([item for item in zip(scores, labels)], key=lambda x: x[0], reverse=True)
+
 class USE:
     """Класс метрики ранжирования USE"""
     def __init__(self):
         self.model = ModelUSE()
 
     def name(self) -> str:
         return "USE"
@@ -190,23 +300,38 @@
         """
         return sorted([item for item in zip(scores, labels)], key=lambda x: x[0], reverse=True)
 
 class RankingMetrics:
     """Класс аккумулирующий все метрики"""
     FAKE_DOC_LABEL: int = -1
 
-    def __init__(self, metrics) -> None:
+    def __init__(self, metrics, relevant_doc_label: Union[int, List] = 1) -> None:
+        """
+
+        Parameters
+        ------------
+        metrics: `Union[LaBSE, USE, Bm25, MsMarcoCE, MsMarcoST]`
+            Классы метрик ранжирования
+
+        relevant_doc_label: `Union[int, List]`
+            Метка или массив меток, обозначающих релевантные документы. (Используется для оценки FDARO)
+        """
         # Среднее место фейковых документов в финальной выдаче
         self.average_place_fake_doc = AverageLoc(metrics)
         # Количество случаев когда фейковый документ выше релевантного
-        self.fake_doc_above_relevant_one = FDARO(metrics)
+        self.fake_doc_above_relevant_one = FDARO(metrics, relevant_doc_label)
         # Количество случаев когда фейковый документ вошел в топ 1
         self.fake_top_k = TopK(metrics)
+        self.upper_quartile = UpQuartile(metrics)
+        # Среднее относительное место фейковых документов в выдаче
+        self.average_rel_place_fake_doc = AverageRelLoc(metrics)
         # Массив метрик для подсчета
         self.metrics = metrics
+        # Число моделей для подсчета метрик
+        self.num_metrics = len(metrics)
 
     def update(self, query: str, sentences: List[str], labels: List[int]) -> None:
         """
        Функция обновления всех метрик по переданным данным
 
        Parameters
        ------------
@@ -232,14 +357,16 @@
                 raise TypeError("The labels must be of the `List[int]` type!")
 
         for cur_metric in self.metrics:
             ranking_list = cur_metric.ranking(query, sentences, labels)
             self.fake_top_k.update(cur_metric.name(), ranking_list, RankingMetrics.FAKE_DOC_LABEL)
             self.fake_doc_above_relevant_one.update(cur_metric.name(), ranking_list, RankingMetrics.FAKE_DOC_LABEL)
             self.average_place_fake_doc.update(cur_metric.name(), ranking_list, RankingMetrics.FAKE_DOC_LABEL)
+            self.average_rel_place_fake_doc.update(cur_metric.name(), ranking_list, RankingMetrics.FAKE_DOC_LABEL)
+            self.upper_quartile.update(cur_metric.name(), ranking_list, RankingMetrics.FAKE_DOC_LABEL)
 
     def get(self) -> Dict:
         """
         Функция для получения значения всех метрик
 
         Returns
         ----------
@@ -252,8 +379,41 @@
 
         for key_, value in self.fake_top_k.get().items():
             result[key_] = value
 
         for key_, value in self.fake_doc_above_relevant_one.get().items():
             result[key_] = value
 
+        for key_, value in self.upper_quartile.get().items():
+            result[key_] = value
+
+        for key_, value in self.average_rel_place_fake_doc.get().items():
+            result[key_] = value
+
         return result
+
+    def show_metrics(self) -> None:
+        for i, (key_, value) in enumerate(self.average_place_fake_doc.get().items()):
+            print(f"{key_}: {np.round(value, 2)}", end="   ")
+
+        print("\n-----------------------------")
+        for i, (key_, value) in enumerate(self.average_rel_place_fake_doc.get().items()):
+            print(f"{key_}: {np.round(value, 2)}", end="   ")
+
+        print("\n-----------------------------")
+        fake_top_k_it = list(self.fake_top_k.get().items())
+        for i in range(3):
+            for j in range(self.num_metrics):
+                print(f"{fake_top_k_it[i + 3*j][0]}: {np.round(fake_top_k_it[i + 3*j][1], 2)}", end="   ")
+            print()
+
+        print("-----------------------------")
+        fake_doc_above_relevant_one_it = list(self.fake_doc_above_relevant_one.get().items())
+        for i in range(2):
+            for j in range(self.num_metrics):
+                print(f"{fake_doc_above_relevant_one_it[i + 2*j][0]}: {np.round(fake_doc_above_relevant_one_it[i + 2*j][1], 4)}", end="   ")
+            print()
+
+        print("-----------------------------")
+        for i, (key_, value) in enumerate(self.upper_quartile.get().items()):
+            print(f"{key_}: {np.round(value, 2)}", end="   ")
+        print("\n\n")
```

### Comparing `docs-ranking-metrics-0.0.4.dev2/src/docs_ranking_metrics.egg-info/PKG-INFO` & `docs-ranking-metrics-0.0.4.dev3/src/docs_ranking_metrics.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 Metadata-Version: 2.1
 Name: docs-ranking-metrics
-Version: 0.0.4.dev2
+Version: 0.0.4.dev3
 Summary: The package contains functions for calculating ranking metrics
 Home-page: https://github.com/betepok506/RankingMetrics
 Author: Andrey Rotanov
 Author-email: rotanov07@mail.ru
+License: UNKNOWN
 Keywords: test
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: test
 
 # Описание
-Данный репозиторий содержит реализацию алгоритмов ранжирования Bm25, LaBSE 
+Данный репозиторий содержит реализацию алгоритмов ранжирования Bm25, LaBSE, MsMarcoST, MsMarcoCE 
 с подсчетом метрик: 
 * Top@1;
 * Top@3;
 * Top@5;
 * Средняя позиция в выдачах (AverageLoc);
-* Оценка как часто фейковый документ выше релевантных (FDARO)
+* Cредняя относительная позиция в выдачах (AverageRelLoc);
+* Оценка как часто фейковый документ выше всех релевантных (FDARO@v1);
+* Оценка как часто фейковый документ выше хотя бы одного релевантного (FDARO@v2);
+* Частота попадания фейкового документа в топ 25% (UpQuartile).
+
 
 
 # Установка
 Для установки пакета воспользуйтесь командой
 ```
 pip install docs-ranking-metrics
 ```
@@ -50,14 +56,16 @@
 labels - метки документов
 '''
 rank_metrics.update(query, sentences, labels)
 
 ...
 # Получение значений подсчитанных метрик ввиде словаря
 rank_metrics.get()
+# Получение значений метрик при помощи функции show_metrics
+rank_metrics.show_metrics()
 ```
 
 Возможный вывод метода get:
 ```
 {
     'LaBSE_AverageLoc': 10.5, 
     'Bm25_AverageLoc': 1.13513, 
@@ -67,7 +75,25 @@
     'Bm25_Top@1': 0.91891, 
     'Bm25_Top@3': 1.0, 
     'Bm25_Top@5': 1.0, 
     'LaBSE_FDARO': 0.6216, 
     'Bm25_FDARO': 1.0
 }
 ```
+
+Возможный вывод метода show_metrics():
+```
+LaBSE_AverageLoc: 4.5   Bm25_AverageLoc: 3.0   
+-----------------------------
+LaBSE_AverageRelLoc: 0.75   Bm25_AverageRelLoc: 0.5   
+-----------------------------
+LaBSE_Top@1: 0.0   Bm25_Top@1: 0.5   
+LaBSE_Top@3: 0.5   Bm25_Top@3: 0.5   
+LaBSE_Top@5: 0.5   Bm25_Top@5: 1.0   
+-----------------------------
+LaBSE_FDARO@v1: 0.5   Bm25_FDARO@v1: 0.5   
+LaBSE_FDARO@v2: 0.5   Bm25_FDARO@v2: 0.5   
+-----------------------------
+LaBSE_UpQuartile: 0.5   Bm25_UpQuartile: 0.5 
+```
+
+
```

