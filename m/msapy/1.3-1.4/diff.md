# Comparing `tmp/msapy-1.3.tar.gz` & `tmp/msapy-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msapy-1.3.tar", last modified: Wed May 17 10:52:23 2023, max compression
+gzip compressed data, was "msapy-1.4.tar", last modified: Thu Jun  1 13:35:59 2023, max compression
```

## Comparing `msapy-1.3.tar` & `msapy-1.4.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxrwxr-x   0 kayson    (1000) kayson    (1000)        0 2023-05-17 10:52:23.025582 msapy-1.3/
--rw-rw-r--   0 kayson    (1000) kayson    (1000)     1069 2021-10-28 14:21:00.000000 msapy-1.3/LICENSE
--rw-rw-r--   0 kayson    (1000) kayson    (1000)    11446 2023-05-17 10:52:23.025582 msapy-1.3/PKG-INFO
-drwxrwxr-x   0 kayson    (1000) kayson    (1000)        0 2023-05-17 10:52:23.021582 msapy-1.3/msapy/
--rw-rw-r--   0 kayson    (1000) kayson    (1000)       66 2023-05-17 10:42:09.000000 msapy-1.3/msapy/__init__.py
--rw-rw-r--   0 kayson    (1000) kayson    (1000)     4423 2023-02-13 13:04:08.000000 msapy-1.3/msapy/checks.py
--rw-rw-r--   0 kayson    (1000) kayson    (1000)     3630 2023-05-17 10:42:09.000000 msapy-1.3/msapy/datastructures.py
--rw-rw-r--   0 kayson    (1000) kayson    (1000)    51816 2023-05-17 10:42:09.000000 msapy-1.3/msapy/msa.py
--rw-rw-r--   0 kayson    (1000) kayson    (1000)     3248 2022-03-30 13:09:51.000000 msapy-1.3/msapy/plottings.py
--rw-rw-r--   0 kayson    (1000) kayson    (1000)    14020 2023-05-17 10:42:09.000000 msapy-1.3/msapy/utils.py
-drwxrwxr-x   0 kayson    (1000) kayson    (1000)        0 2023-05-17 10:52:23.025582 msapy-1.3/msapy.egg-info/
--rw-rw-r--   0 kayson    (1000) kayson    (1000)    11446 2023-05-17 10:52:22.000000 msapy-1.3/msapy.egg-info/PKG-INFO
--rw-rw-r--   0 kayson    (1000) kayson    (1000)      442 2023-05-17 10:52:22.000000 msapy-1.3/msapy.egg-info/SOURCES.txt
--rw-rw-r--   0 kayson    (1000) kayson    (1000)        1 2023-05-17 10:52:22.000000 msapy-1.3/msapy.egg-info/dependency_links.txt
--rw-rw-r--   0 kayson    (1000) kayson    (1000)      180 2023-05-17 10:52:22.000000 msapy-1.3/msapy.egg-info/requires.txt
--rw-rw-r--   0 kayson    (1000) kayson    (1000)       12 2023-05-17 10:52:22.000000 msapy-1.3/msapy.egg-info/top_level.txt
--rw-rw-r--   0 kayson    (1000) kayson    (1000)       38 2023-05-17 10:52:23.025582 msapy-1.3/setup.cfg
--rw-rw-r--   0 kayson    (1000) kayson    (1000)      990 2023-05-17 10:42:09.000000 msapy-1.3/setup.py
-drwxrwxr-x   0 kayson    (1000) kayson    (1000)        0 2023-05-17 10:52:23.025582 msapy-1.3/tests/
--rw-rw-r--   0 kayson    (1000) kayson    (1000)        0 2021-10-28 15:26:21.000000 msapy-1.3/tests/__init__.py
--rw-rw-r--   0 kayson    (1000) kayson    (1000)     2125 2022-08-09 14:21:40.000000 msapy-1.3/tests/test_bad_inputs.py
--rw-rw-r--   0 kayson    (1000) kayson    (1000)     3747 2023-02-13 13:04:08.000000 msapy-1.3/tests/test_ground_truth.py
--rw-rw-r--   0 kayson    (1000) kayson    (1000)     1660 2023-02-13 13:04:08.000000 msapy-1.3/tests/test_ground_truth_multiscores.py
--rw-rw-r--   0 kayson    (1000) kayson    (1000)     1334 2023-02-13 13:04:08.000000 msapy-1.3/tests/test_ground_truth_nd.py
--rw-rw-r--   0 kayson    (1000) kayson    (1000)     2856 2023-02-13 13:04:08.000000 msapy-1.3/tests/test_ground_truth_timeseries.py
+drwxrwxr-x   0 kayson    (1000) kayson    (1000)        0 2023-06-01 13:35:59.393521 msapy-1.4/
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)     1069 2021-10-28 14:21:00.000000 msapy-1.4/LICENSE
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)    11446 2023-06-01 13:35:59.393521 msapy-1.4/PKG-INFO
+drwxrwxr-x   0 kayson    (1000) kayson    (1000)        0 2023-06-01 13:35:59.393521 msapy-1.4/msapy/
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)       66 2023-06-01 13:35:28.000000 msapy-1.4/msapy/__init__.py
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)     4070 2023-06-01 13:35:28.000000 msapy-1.4/msapy/checks.py
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)     2949 2023-06-01 13:35:28.000000 msapy-1.4/msapy/datastructures.py
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)    55110 2023-06-01 13:35:28.000000 msapy-1.4/msapy/msa.py
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)     3248 2022-03-30 13:09:51.000000 msapy-1.4/msapy/plottings.py
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)    14020 2023-05-17 10:42:09.000000 msapy-1.4/msapy/utils.py
+drwxrwxr-x   0 kayson    (1000) kayson    (1000)        0 2023-06-01 13:35:59.393521 msapy-1.4/msapy.egg-info/
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)    11446 2023-06-01 13:35:59.000000 msapy-1.4/msapy.egg-info/PKG-INFO
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)      403 2023-06-01 13:35:59.000000 msapy-1.4/msapy.egg-info/SOURCES.txt
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)        1 2023-06-01 13:35:59.000000 msapy-1.4/msapy.egg-info/dependency_links.txt
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)      180 2023-06-01 13:35:59.000000 msapy-1.4/msapy.egg-info/requires.txt
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)       12 2023-06-01 13:35:59.000000 msapy-1.4/msapy.egg-info/top_level.txt
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)       38 2023-06-01 13:35:59.393521 msapy-1.4/setup.cfg
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)      990 2023-06-01 13:35:28.000000 msapy-1.4/setup.py
+drwxrwxr-x   0 kayson    (1000) kayson    (1000)        0 2023-06-01 13:35:59.393521 msapy-1.4/tests/
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)        0 2021-10-28 15:26:21.000000 msapy-1.4/tests/__init__.py
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)     2107 2023-06-01 13:35:28.000000 msapy-1.4/tests/test_bad_inputs.py
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)     3717 2023-06-01 13:35:28.000000 msapy-1.4/tests/test_ground_truth.py
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)     2727 2023-06-01 13:35:28.000000 msapy-1.4/tests/test_ground_truth_nd.py
+-rw-rw-r--   0 kayson    (1000) kayson    (1000)     2882 2023-06-01 13:35:28.000000 msapy-1.4/tests/test_ground_truth_timeseries.py
```

### Comparing `msapy-1.3/LICENSE` & `msapy-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `msapy-1.3/PKG-INFO` & `msapy-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msapy
-Version: 1.3
+Version: 1.4
 Summary: Multi-perturbation Shapley value Analysis (MSA)
 Home-page: https://github.com/kuffmode/msa
 Author: Kayson Fakhar, Shrey Dixit
 Author-email: kayson.fakhar@gmail.com, shrey.akshaj@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `msapy-1.3/msapy/checks.py` & `msapy-1.4/msapy/checks.py`

 * *Files 11% similar despite different names*

```diff
@@ -54,24 +54,16 @@
 
     if not _is_homogeneous_list(list(contributions.values())):
         raise ValueError(
             "Objective function returned values of different data types")
 
     arbitrary_contribution = next(iter(contributions.values()))
 
-    if isinstance(arbitrary_contribution, dict):
-        return "multi_scores", arbitrary_contribution
-    
     if isinstance(arbitrary_contribution, np.ndarray):
-        if len(arbitrary_contribution.shape) > 1:
-            return "nd", arbitrary_contribution
-        return "timeseries", arbitrary_contribution
-
-    if _is_iterable(arbitrary_contribution) and _is_number(arbitrary_contribution[0]):
-        return "timeseries", arbitrary_contribution
+        return "nd", arbitrary_contribution
 
     if not _is_number(arbitrary_contribution):
         raise ValueError("Objective function should return a value that is either"
                          " a Number, a dictionary or Numbers, iterable of numbers, or a numpy array."
                          f" Returned {type(arbitrary_contribution)} instead.")
 
     return "scaler", arbitrary_contribution
@@ -86,14 +78,15 @@
             raise ValueError(
                 "A contributions dictionacontributions_excludingry is not required in case of lazy calculation of shapely table")
     else:
         if contributions is None:
             raise ValueError(
                 "A contributions dictionary is neccessary for the calculation of shapley table if lazy is set to False")
 
+
 def _is_number(x) -> bool:
     return isinstance(x, (Number, np.number))
 
 
 @typechecked
 def _are_lists_same_length(lists: list):
     return len({len(i) for i in lists}) == 1
```

### Comparing `msapy-1.3/msapy/msa.py` & `msapy-1.4/msapy/msa.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typeguard import typechecked
 from tqdm import tqdm
 from fastprogress.fastprogress import master_bar, progress_bar, MasterBar
 from tqdm_joblib import tqdm_joblib
 
 from msapy import utils as ut
 from msapy.checks import _check_get_shapley_table_args, _check_valid_combination_space, _check_valid_elements, _check_valid_n_permutations, _check_valid_permutation_space, _get_contribution_type, _is_number
-from msapy.datastructures import ShapleyModeND, ShapleyTable, ShapleyTableMultiScores, ShapleyTableTimeSeries
+from msapy.datastructures import ShapleyModeND, ShapleyTable, ShapleyTableND
 
 
 @typechecked
 def make_permutation_space(*,
                            elements: list,
                            n_permutations: int,
                            pair: Optional[Tuple] = None,
@@ -288,15 +288,16 @@
 def get_shapley_table(*,
                       permutation_space: list,
                       contributions: Optional[Dict] = None,
                       lesioned: Optional[any] = None,
                       objective_function: Optional[Callable] = None,
                       objective_function_params: Optional[Dict] = None,
                       lazy=False,
-                      dual_progress_bars: bool=True,
+                      save_permutations: bool = False,
+                      dual_progress_bars: bool = True,
                       mbar: Optional[MasterBar] = None,) -> pd.DataFrame:
     """
     Calculates Shapley values based on the filled contribution_space.
     Briefly, for a permutation (A,B,C) it will be:
 
     (A,B,C) - (B,C) = Contribution of A to the coalition (B,C).
     (B,C) - (C) = Contribution of B to the coalition formed with (C).
@@ -311,98 +312,142 @@
 
         permutation_space (list):
             Should be the same passed to make_combination_space.
 
         lesioned (Optional[any]):
             leseioned element that will not be present in any combination
 
+        objective_function (Callable):
+            The game (in-silico experiment). It should get the complement set and return one numeric value
+            either int or float.
+            This function is just calling it as: objective_function(complement, **objective_function_params)
+
+            An example using networkx with some tips:
+            (you sometimes need to specify what should happen during edge-cases like an all-lesioned network)
+
+            def local_efficiency(complements, graph):
+                if len(complements) < 0:
+                    # the network is intact so:
+                    return nx.local_efficiency(graph)
+
+                elif len(complements) == len(graph):
+                    # the network is fully lesioned so:
+                    return 0.0
+
+                else:
+                    # lesion the system, calculate things
+                    lesioned = graph.copy()
+                    lesioned.remove_nodes_from(complements)
+                    return nx.local_efficiency(lesioned)
+
+        objective_function_params (Dict):
+            Kwargs for the objective_function.
+
+        lesioned (Optional[any]):
+            leseioned element that will not be present in any combination
+
+        multiprocessing_method (str):
+            So far, two methods of parallelization is implemented, 'joblib' and 'ray' and the default method is joblib.
+            If using ray tho, you need to decorate your objective function with @ray.remote decorator. Visit their
+            documentations to see how to go for it. I guess ray works better on HPC clusters (if they support it tho!)
+            and probably doesn't suffer from the sneaky "memory leakage" of joblib. But just by playing around,
+            I realized joblib is faster for tasks that are small themselves. Remedies are here:
+            https://docs.ray.io/en/latest/auto_examples/tips-for-first-time.html
+
+            Note: Generally, multiprocessing isn't always faster as explained above. Use it when the function itself
+            takes some like each game takes longer than 0.5 seconds or so. For example, a function that sleeps for a
+            second on a set of 10 elements with 1000 permutations each (1024 games) performs as follows:
+
+                - no parallel: 1020 sec
+                - joblib: 63 sec
+                - ray: 65 sec
+
+            That makes sense since I have 16 cores and 1000/16 is around 62.
+
+        rng (Optional[np.random.Generator]): Numpy random generator object used for reproducable results. Default is None.
+
+        random_seed (Optional[int]):
+            sets the random seed of the sampling process. Only used when `rng` is None. Default is None.
+
+        n_parallel_games (int):
+            Number of parallel jobs (number of to-be-occupied cores),
+            -1 means all CPU cores and 1 means a serial process.
+            I suggest using 1 for debugging since things get messy in parallel!
+
+        lazy (bool): if set to True, objective function will be called lazily instead of calling it all at once and storing the outputs in a dict.
+            Setting it to True saves a lot of memory and might even be faster in certain cases.
+
+        save_permutations (bool): If set to True, the shapley values are calculated by calculating the running mean of the permutations instead of
+            storing the permutations. This parameter is ignored in case the objective function returns a scaler.
+
+        dual_progress_bar (bool): If set to true, you will have two progress bars. One parent that will track the permutations, other child that
+            will track the elements. Its ignored in case the mbar is provided
+
+        mbar (MasterBar): A Fastprogress MasterBar. Use it in case you're calling the interface multiple times to have a nester progress bar.
+
     Returns:
         pd.DataFrame: Shapley table or a dict of Shapely tables, columns will be 
         elements and indices will be samples (permutations). 
-        It will be a Multi-Index DataFrame if the contributions are a dict
-        i.e. the objective function returns multiple score functions (eg. accuracy, f1_score, etc.)
         It will be a Multi-Index DataFrame if the contributions are a timeseries.
         The index at `level=1` will be the timestamps
     """
     _check_get_shapley_table_args(contributions, objective_function, lazy)
     _check_valid_permutation_space(permutation_space)
 
     contributions = {tuple(): objective_function(tuple(), **objective_function_params)} if lazy else contributions
 
-    contribution_type, arbitrary_contrib = _get_contribution_type(
-        contributions)
-
-    # if it's a multi score problem, then we make all the contributions to numpy arrays for efficient calculations later
-    if contribution_type == 'multi_scores':
-        scores = list(arbitrary_contrib.keys())
-        contributions = {k: np.array(list(v.values()))
-                         for k, v in contributions.items()}
+    contribution_type, arbitrary_contrib = _get_contribution_type(contributions)
 
     lesioned = set(lesioned) if lesioned else set()
-    shapley_table = {} if contribution_type != 'nd' else 0
+    shapley_table = 0 if (contribution_type == 'nd' and not save_permutations) else {}
 
     if not lazy:
         parent_bar = enumerate(set(permutation_space))
     elif (not dual_progress_bars) or mbar:
-        parent_bar = progress_bar(enumerate(set(permutation_space)), total=len(permutation_space), leave=False, parent=mbar)
+        parent_bar = progress_bar(enumerate(set(permutation_space)), total=len(
+            permutation_space), leave=False, parent=mbar)
     elif lazy:
-        parent_bar = master_bar(enumerate(set(permutation_space)), total=len(permutation_space))
-        
+        parent_bar = master_bar(
+            enumerate(set(permutation_space)), total=len(permutation_space))
 
     for i, permutation in parent_bar:
         isolated_contributions = []  # got to be a better way!
-        child_bar = enumerate(permutation) if not (dual_progress_bars and lazy) else progress_bar(enumerate(permutation), total=len(permutation), leave=False, parent=parent_bar)
+        child_bar = enumerate(permutation) if not (dual_progress_bars and lazy) else progress_bar(
+            enumerate(permutation), total=len(permutation), leave=False, parent=parent_bar)
         # iterate over all elements in the permutation to calculate their isolated contributions
         for index, _ in child_bar:
             including = frozenset(permutation[:index + 1]) - lesioned
             excluding = frozenset(permutation[:index]) - lesioned
 
             # the isolated contribution of an element is the difference of contribution with that element and without that element
             if lazy:
                 contributions_including = objective_function(tuple(excluding), **objective_function_params)
                 contributions_excluding = objective_function(tuple(including), **objective_function_params)
 
-                if contribution_type == 'multi_scores':
-                    contributions_including = np.array(list(contributions_including.values()))
-                    contributions_excluding = np.array(list(contributions_excluding.values()))
-
-                isolated_contributions.append(
-                    contributions_including - contributions_excluding)
+                isolated_contributions.append(contributions_including - contributions_excluding)
             else:
-                isolated_contributions.append(
-                    contributions[including] - contributions[excluding])
-        if contribution_type == 'nd':
-            isolated_contributions = [x for _, x in sorted(
-                zip(permutation, isolated_contributions))]
-            shapley_table += (np.array(isolated_contributions) -
-                              shapley_table) / (i + 1)
+                isolated_contributions.append(contributions[including] - contributions[excluding])
+
+        if contribution_type == 'nd' and not save_permutations:
+            isolated_contributions = [x for _, x in sorted(zip(permutation, isolated_contributions))]
+            shapley_table += (np.array(isolated_contributions) - shapley_table) / (i + 1)
         else:
             shapley_table[permutation] = np.array(isolated_contributions)
 
     # post processing of shapley values based on what type of contribution it is. The format of output will vary based on if the
     # values are multi-scores, timeseries, etc.
-    if contribution_type == 'nd':
+    if contribution_type == 'nd' and not save_permutations:
         shapley_table = shapley_table.reshape(shapley_table.shape[0], -1).T
         shapley_table = pd.DataFrame(
             shapley_table, columns=sorted(permutation))
         return ShapleyModeND(shapley_table, arbitrary_contrib.shape)
 
-    if contribution_type != 'multi_scores':
-        shapley_table = pd.DataFrame([dict(zip(permutations, shapleys))
-                                      for permutations, shapleys in shapley_table.items()])
-        return ShapleyTableTimeSeries.from_dataframe(shapley_table) if (contribution_type == "timeseries") else ShapleyTable(shapley_table)
-
-    shapley_values = []
-    for i in range(len(arbitrary_contrib)):
-        shapley_values.append(pd.DataFrame([dict(zip(permutations, shapleys[:, i]))
-                                            for permutations, shapleys in shapley_table.items()]))
-
-    shapley_table = pd.concat(shapley_values, keys=scores)
-
-    return ShapleyTableMultiScores(shapley_table)
+    shapley_table = pd.DataFrame([dict(zip(permutations, shapleys))
+                                  for permutations, shapleys in shapley_table.items()])
+    return ShapleyTableND.from_dataframe(shapley_table, shape=arbitrary_contrib.shape) if (contribution_type == "nd") else ShapleyTable(shapley_table)
 
 
 @typechecked
 def interface(*,
               n_permutations: int,
               elements: list,
               objective_function: Callable,
@@ -411,17 +456,18 @@
               pair: Optional[Tuple] = None,
               lesioned: Optional[any] = None,
               multiprocessing_method: str = 'joblib',
               rng: Optional[np.random.Generator] = None,
               random_seed: Optional[int] = None,
               n_parallel_games: int = -1,
               lazy: bool = True,
-              dual_progress_bars: bool=True,
+              save_permutations: bool = False,
+              dual_progress_bars: bool = True,
               mbar: Optional[MasterBar] = None
-              ) -> Tuple[pd.DataFrame, Dict, Dict]:
+              ) -> pd.DataFrame:
     """
     A wrapper function to call other related functions internally and produces an easy-to-use pipeline.
 
     Args:
         n_permutations (int):
             Number of permutations (samples) per element.
 
@@ -481,21 +527,33 @@
                 - ray: 65 sec
 
             That makes sense since I have 16 cores and 1000/16 is around 62.
 
         rng (Optional[np.random.Generator]): Numpy random generator object used for reproducable results. Default is None.
 
         random_seed (Optional[int]):
-            sets the random seed of tdual_progress_bars=dual_progress_bars,he sampling process. Only used when `rng` is None. Default is None.
+            sets the random seed of the sampling process. Only used when `rng` is None. Default is None.
 
         n_parallel_games (int):
             Number of parallel jobs (number of to-be-occupied cores),
             -1 means all CPU cores and 1 means a serial process.
             I suggest using 1 for debugging since things get messy in parallel!
 
+        lazy (bool): if set to True, objective function will be called lazily instead of calling it all at once and storing the outputs in a dict.
+            Setting it to True saves a lot of memory and might even be faster in certain cases.
+
+        save_permutations (bool): If set to True, the shapley values are calculated by calculating the running mean of the permutations instead of
+            storing the permutations. This parameter is ignored in case the objective function returns a scaler.
+
+        dual_progress_bar (bool): If set to true, you will have two progress bars. One parent that will track the permutations, other child that
+            will track the elements. Its ignored in case the mbar is provided
+
+        mbar (MasterBar): A Fastprogress MasterBar. Use it in case you're calling the interface multiple times to have a nester progress bar.
+
+
     Returns:
         Tuple[pd.DataFrame, Dict, Dict]: shapley_table, contributions, lesion_effects
 
     Note that contributions and lesion_effects are the same values, addressed differently. For example:
     If from a set of ABCD removing AC ends with some value x, you can say the contribution of BD=x and the
     effect of removing AC=x. So the same values are addressed differently in the two returned Dicts.
     Of course, it makes more sense to compare the lesion effects with the intact system but who am I to judge.
@@ -519,47 +577,48 @@
     if lazy:
         shapley_table = get_shapley_table(permutation_space=permutation_space,
                                           lesioned=lesioned,
                                           lazy=True,
                                           objective_function=objective_function,
                                           objective_function_params=objective_function_params,
                                           dual_progress_bars=dual_progress_bars,
+                                          save_permutations=save_permutations,
                                           mbar=mbar)[elements]
-        return shapley_table, {}, {}
-
+        return shapley_table
 
     combination_space = make_combination_space(permutation_space=permutation_space,
-                                                pair=pair,
-                                                lesioned=lesioned)
+                                               pair=pair,
+                                               lesioned=lesioned)
     complement_space = make_complement_space(combination_space=combination_space,
-                                                elements=elements,
-                                                lesioned=lesioned)
+                                             elements=elements,
+                                             lesioned=lesioned)
 
     if n_parallel_games == 1:
-        contributions, lesion_effects = take_contributions(elements=elements,
-                                                           complement_space=complement_space,
-                                                           combination_space=combination_space,
-                                                           objective_function=objective_function,
-                                                           objective_function_params=objective_function_params,
-                                                           mbar=mbar)
+        contributions, _ = take_contributions(elements=elements,
+                                              complement_space=complement_space,
+                                              combination_space=combination_space,
+                                              objective_function=objective_function,
+                                              objective_function_params=objective_function_params,
+                                              mbar=mbar)
     else:
-        contributions, lesion_effects = ut.parallelized_take_contributions(
+        contributions, _ = ut.parallelized_take_contributions(
             multiprocessing_method=multiprocessing_method,
             n_cores=n_parallel_games,
             complement_space=complement_space,
             combination_space=combination_space,
             objective_function=objective_function,
             objective_function_params=objective_function_params,
             mbar=mbar)
 
     shapley_table = get_shapley_table(contributions=contributions,
                                       permutation_space=permutation_space,
                                       dual_progress_bars=dual_progress_bars,
+                                      save_permutations=save_permutations,
                                       lesioned=lesioned, mbar=mbar)[elements]
-    return shapley_table, contributions, lesion_effects
+    return shapley_table
 
 
 @typechecked
 def interaction_2d(*,
                    n_permutations: int,
                    elements: list,
                    pair: tuple,
@@ -652,28 +711,29 @@
                       "objective_function": objective_function,
                       "n_permutations": n_permutations,
                       "objective_function_params": objective_function_params,
                       "multiprocessing_method": multiprocessing_method,
                       "rng": rng,
                       "random_seed": random_seed,
                       "n_parallel_games": n_parallel_games,
+                      "save_permutations": False,
                       "lazy": False}
 
     # calculate the shapley values with element j lesioned
-    shapley_i, _, _ = interface(**interface_args, lesioned=pair[1])
+    shapley_i = interface(**interface_args, lesioned=pair[1])
     # get the shapley value of element i with element j leasioned
     gamma_i = _get_gamma(shapley_i, pair[0]).sum()
 
     # calculate the shapley values with element i lesioned
-    shapley_j, _, _ = interface(**interface_args, lesioned=pair[0])
+    shapley_j = interface(**interface_args, lesioned=pair[0])
     # get the shapley value of element j with element i leasioned
     gamma_j = _get_gamma(shapley_j, pair[1]).sum()
 
     # calculate the shapley values with element i and j together in every combination
-    shapley_ij, _, _ = interface(**interface_args, pair=pair)
+    shapley_ij = interface(**interface_args, pair=pair)
     # get the sum of the shapley value of element i and j
     gamma_ij = _get_gamma(shapley_ij, pair).sum()
 
     return gamma_ij, gamma_i, gamma_j
 
 
 @typechecked
@@ -787,30 +847,28 @@
             raise NotImplementedError("`network_interaction_2d` does not work with"
                                       " timeseries or multiscore contributions yet.")
         interactions[x, y] = interactions[y, x] = gammaAB - gammaA - gammaB
 
     return interactions
 
 
-def _get_gamma(shapley_table, idx):
+def _get_gamma(shapley, idx):
     """returns shapley value of elements in idx
 
     Args:
         shapley_table (pd.DataFrame): shapley table with one element lesioned
         idx (_type_): element of interest
 
     Returns:
         shapley value of elements in idx
     """
-    if shapley_table.index.nlevels == 1:
-        gamma = shapley_table[list(idx)].mean()
-    elif "timestamp" in shapley_table.index.names:
-        gamma = shapley_table[list(idx)].groupby(level=1).mean()
-    else:
-        gamma = shapley_table[list(idx)].groupby(level=0).mean()
+    if isinstance(shapley, ShapleyTable):
+        gamma = shapley.shapley_values[list(idx)]
+    elif isinstance(shapley, ShapleyTableND):
+        gamma = shapley[list(idx)]
     return gamma
 
 
 @typechecked
 def estimate_causal_influences(elements: list,
                                objective_function: Callable,
                                objective_function_params: Optional[dict] = None,
@@ -913,15 +971,16 @@
 
     """
     target_elements = target_elements if target_elements else elements
     objective_function_params = objective_function_params if objective_function_params else {}
 
     if parallelize_over_games:
         # run causal_influence_single_element for all target elements.
-        mbar = master_bar(enumerate(target_elements), total=len(target_elements))
+        mbar = master_bar(enumerate(target_elements),
+                          total=len(target_elements))
         results = [causal_influence_single_element(elements, objective_function,
                                                    objective_function_params, n_permutations,
                                                    n_cores, multiprocessing_method,
                                                    permutation_seed, index, element, lazy, mbar) for index, element in mbar]
 
     elif multiprocessing_method == 'ray':
         if importlib.util.find_spec("ray") is None:
@@ -947,28 +1006,26 @@
 
         results = ray.get(result_ids)
         ray.shutdown()
 
     else:
         with tqdm_joblib(desc="Doing Nodes: ", total=len(target_elements)) as pb:
             results = (Parallel(n_jobs=n_cores)(delayed(causal_influence_single_element)(elements, objective_function,
-                                                                                     objective_function_params, n_permutations,
-                                                                                     1, 'joblib',
-                                                                                     permutation_seed, index, element, lazy) for index, element in enumerate(target_elements)))
+                                                                                         objective_function_params, n_permutations,
+                                                                                         1, 'joblib',
+                                                                                         permutation_seed, index, element, lazy) for index, element in enumerate(target_elements)))
 
     _, contribution_type = results[0]
     shapley_values = [r[0] for r in results]
 
     causal_influences = pd.DataFrame(
         shapley_values, columns=elements) if contribution_type == "scaler" else pd.concat(shapley_values, keys=elements)
-    
+
     if contribution_type == "scaler":
         return causal_influences
-    if contribution_type == "multi_scores":
-        return causal_influences.swaplevel().sort_index(level=0) 
     return causal_influences[causal_influences.index.levels[0]]
 
 
 def causal_influence_single_element(elements, objective_function,
                                     objective_function_params, n_permutations,
                                     n_parallel_games, multiprocessing_method,
                                     permutation_seed, index, element, lazy=True, mbar=None):
@@ -1039,21 +1096,22 @@
     """
 
     objective_function_params['index'] = index
 
     # Takes the target out of the to_be_lesioned list
     without_target = set(elements).difference({element})
 
-    shapley_output, _, _ = interface(n_permutations=n_permutations,
-                                                elements=list(without_target),
-                                                dual_progress_bars= False,
-                                                objective_function=objective_function,
-                                                objective_function_params=objective_function_params,
-                                                n_parallel_games=n_parallel_games,
-                                                multiprocessing_method=multiprocessing_method,
-                                                random_seed=permutation_seed,
-                                                lazy=lazy,
-                                                mbar=mbar)
+    shapley_output = interface(n_permutations=n_permutations,
+                               elements=list(without_target),
+                               dual_progress_bars=False,
+                               objective_function=objective_function,
+                               objective_function_params=objective_function_params,
+                               n_parallel_games=n_parallel_games,
+                               multiprocessing_method=multiprocessing_method,
+                               random_seed=permutation_seed,
+                               lazy=lazy,
+                               save_permutations=False,
+                               mbar=mbar)
 
-    if shapley_output.contribution_type in ("scaler", "multi_scores"):
+    if shapley_output.contribution_type == "scaler":
         return shapley_output.shapley_values, shapley_output.contribution_type
-    return shapley_output.shapley_modes, shapley_output.contribution_type
+    return shapley_output, shapley_output.contribution_type
```

### Comparing `msapy-1.3/msapy/plottings.py` & `msapy-1.4/msapy/plottings.py`

 * *Files identical despite different names*

### Comparing `msapy-1.3/msapy/utils.py` & `msapy-1.4/msapy/utils.py`

 * *Files identical despite different names*

### Comparing `msapy-1.3/msapy.egg-info/PKG-INFO` & `msapy-1.4/msapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msapy
-Version: 1.3
+Version: 1.4
 Summary: Multi-perturbation Shapley value Analysis (MSA)
 Home-page: https://github.com/kuffmode/msa
 Author: Kayson Fakhar, Shrey Dixit
 Author-email: kayson.fakhar@gmail.com, shrey.akshaj@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `msapy-1.3/setup.py` & `msapy-1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open("requirements.txt", "r") as f:
     base_packages = f.read().split("\n")
 
 test_packages = ["pytest~=6.2.5"]
 
 setup(name="msapy",
-      version="1.3",
+      version="1.4",
       description=DESCRIPTION,
       long_description=LONG_DESCRIPTION,
       long_description_content_type='text/markdown',
       author='Kayson Fakhar, Shrey Dixit',
       author_email='kayson.fakhar@gmail.com, shrey.akshaj@gmail.com',
       url="https://github.com/kuffmode/msa",
       packages=find_packages(),
```

### Comparing `msapy-1.3/tests/test_bad_inputs.py` & `msapy-1.4/tests/test_bad_inputs.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,13 +43,13 @@
 @pytest.mark.parametrize("p_value", [0, -1])
 def test_zero_negative_pvalue(p_value):
     elements = ['a', 'b', 'c']
 
     def one(complements):
         return 1
 
-    for_bootstrap, _, _ = msa.interface(elements=elements,
-                                        n_permutations=100,
-                                        objective_function=one)
+    for_bootstrap = msa.interface(elements=elements,
+                                  n_permutations=100,
+                                  objective_function=one)
     with pytest.raises(ValueError):
         ut.bootstrap_hypothesis_testing(dataset=for_bootstrap,
                                         p_value=p_value)
```

### Comparing `msapy-1.3/tests/test_ground_truth.py` & `msapy-1.4/tests/test_ground_truth.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     return sum(contrib_dict.values()) - sum(contrib_dict[k] for k in complements)
 
 
 # ------------------------------#
 elements = ['a', 'b', 'c']
 cause = 'a'
-shapley_table, contributions, lesions = msa.interface(
+shapley_table = msa.interface(
     elements=elements,
     n_permutations=300,
     objective_function=simple,
     n_parallel_games=1,
     objective_function_params={'causes': cause},
     random_seed=111)
 
@@ -89,15 +89,15 @@
 
     np.fill_diagonal(calculated_causal_influences, 0)
 
     assert np.allclose(calculated_causal_influences, true_causal_influences)
 
 
 def test_interface_parallel_joblib():
-    shapley_table_parallel, _, _ = msa.interface(
+    shapley_table_parallel = msa.interface(
         elements=elements,
         n_permutations=300,
         objective_function=simple,
         n_parallel_games=-1,
         objective_function_params={'causes': cause},
         random_seed=111)
```

### Comparing `msapy-1.3/tests/test_ground_truth_timeseries.py` & `msapy-1.4/tests/test_ground_truth_timeseries.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,19 +17,20 @@
 @pytest.mark.parametrize("n_parallel_games", [1, -1])
 def test_contributions(n_parallel_games):
     data, final_wave, elements = prepare_data()
 
     def score_function(complements):
         return final_wave - data[complements, :].sum(0)
 
-    shapley_table, _, _ = msa.interface(
+    shapley_table = msa.interface(
         elements=elements,
         n_permutations=5_000,
         objective_function=score_function,
-        n_parallel_games=n_parallel_games)
+        n_parallel_games=n_parallel_games,
+        save_permutations=True)
 
     assert np.allclose(shapley_table.groupby(level=1).mean(), data.T)
 
 
 @pytest.mark.parametrize("n_cores, multiprocessing_method, parallelize_over_games",
                          [(1, 'joblib', True), (-1, 'joblib', True), (1, 'joblib', False), (-1, 'joblib', False)])
 def test_estimate_causal_influence(n_cores, multiprocessing_method, parallelize_over_games):
```

