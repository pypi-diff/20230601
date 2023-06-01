# Comparing `tmp/pref_voting-0.3.4.tar.gz` & `tmp/pref_voting-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pref_voting-0.3.4.tar", max compression
+gzip compressed data, was "pref_voting-0.4.tar", max compression
```

## Comparing `pref_voting-0.3.4.tar` & `pref_voting-0.4.tar`

### file list

```diff
@@ -1,31 +1,34 @@
--rw-r--r--   0        0        0     1068 2022-07-08 15:47:57.000000 pref_voting-0.3.4/LICENSE
--rw-r--r--   0        0        0     3200 2023-05-26 17:57:30.757597 pref_voting-0.3.4/README.md
--rw-r--r--   0        0        0       22 2023-05-30 21:25:26.910744 pref_voting-0.3.4/pref_voting/__init__.py
--rw-r--r--   0        0        0     9632 2023-05-24 13:13:44.583927 pref_voting-0.3.4/pref_voting/analysis.py
--rw-r--r--   0        0        0     1226 2023-05-24 13:13:43.582814 pref_voting-0.3.4/pref_voting/axiom.py
--rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-0.3.4/pref_voting/axiom_helpers.py
--rw-r--r--   0        0        0       91 2023-05-25 14:07:56.083200 pref_voting-0.3.4/pref_voting/axioms.py
--rw-r--r--   0        0        0    23065 2023-05-10 11:22:02.837497 pref_voting-0.3.4/pref_voting/c1_methods.py
--rw-r--r--   0        0        0     8551 2023-05-30 17:01:09.832556 pref_voting-0.3.4/pref_voting/combined_methods.py
--rw-r--r--   0        0        0    11517 2023-05-10 11:58:43.699679 pref_voting-0.3.4/pref_voting/dominance_axioms.py
--rw-r--r--   0        0        0    20643 2023-05-10 11:16:22.353419 pref_voting-0.3.4/pref_voting/generate_profiles.py
--rw-r--r--   0        0        0     4680 2023-05-30 19:57:47.963280 pref_voting-0.3.4/pref_voting/generate_utility_profiles.py
--rw-r--r--   0        0        0    10486 2023-05-24 13:13:45.272860 pref_voting-0.3.4/pref_voting/generate_weighted_majority_graphs.py
--rw-r--r--   0        0        0     1806 2022-08-08 19:08:16.000000 pref_voting-0.3.4/pref_voting/helper.py
--rw-r--r--   0        0        0    74050 2023-05-29 22:04:12.246564 pref_voting-0.3.4/pref_voting/iterative_methods.py
--rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-0.3.4/pref_voting/maj_graph_ex1.png
--rw-r--r--   0        0        0    59218 2023-05-26 17:44:51.542166 pref_voting-0.3.4/pref_voting/margin_based_methods.py
--rw-r--r--   0        0        0    25681 2023-05-10 11:20:32.560828 pref_voting-0.3.4/pref_voting/other_methods.py
--rw-r--r--   0        0        0    28614 2023-05-30 20:06:31.706933 pref_voting-0.3.4/pref_voting/profiles.py
--rw-r--r--   0        0        0    25273 2023-05-26 17:38:33.040884 pref_voting-0.3.4/pref_voting/profiles_with_ties.py
--rw-r--r--   0        0        0    12468 2023-05-26 10:23:18.532269 pref_voting-0.3.4/pref_voting/rankings.py
--rw-r--r--   0        0        0    11066 2023-05-26 12:19:11.420399 pref_voting-0.3.4/pref_voting/scoring_methods.py
--rw-r--r--   0        0        0     6661 2023-05-26 14:18:34.309764 pref_voting-0.3.4/pref_voting/utility_methods.py
--rw-r--r--   0        0        0    15088 2023-05-30 20:17:01.412933 pref_voting-0.3.4/pref_voting/utility_profiles.py
--rw-r--r--   0        0        0     8393 2023-05-26 10:50:34.876976 pref_voting-0.3.4/pref_voting/variable_voter_axioms.py
--rw-r--r--   0        0        0     5395 2023-05-26 10:54:32.445716 pref_voting-0.3.4/pref_voting/voting_method.py
--rw-r--r--   0        0        0      253 2022-07-31 21:02:46.000000 pref_voting-0.3.4/pref_voting/voting_methods.py
--rw-r--r--   0        0        0    53001 2023-05-26 17:56:28.071379 pref_voting-0.3.4/pref_voting/weighted_majority_graphs.py
--rw-r--r--   0        0        0      689 2023-05-30 21:25:26.909630 pref_voting-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     4153 1970-01-01 00:00:00.000000 pref_voting-0.3.4/setup.py
--rw-r--r--   0        0        0     4268 1970-01-01 00:00:00.000000 pref_voting-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-07-08 15:47:57.000000 pref_voting-0.4/LICENSE
+-rw-r--r--   0        0        0     3443 2023-06-01 01:47:00.972293 pref_voting-0.4/README.md
+-rw-r--r--   0        0        0       20 2023-06-01 01:46:15.073296 pref_voting-0.4/pref_voting/__init__.py
+-rw-r--r--   0        0        0     9632 2023-05-24 13:13:44.583927 pref_voting-0.4/pref_voting/analysis.py
+-rw-r--r--   0        0        0     1226 2023-05-24 13:13:43.582814 pref_voting-0.4/pref_voting/axiom.py
+-rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-0.4/pref_voting/axiom_helpers.py
+-rw-r--r--   0        0        0       91 2023-05-25 14:07:56.083200 pref_voting-0.4/pref_voting/axioms.py
+-rw-r--r--   0        0        0    23065 2023-05-10 11:22:02.837497 pref_voting-0.4/pref_voting/c1_methods.py
+-rw-r--r--   0        0        0     8551 2023-05-30 17:01:09.832556 pref_voting-0.4/pref_voting/combined_methods.py
+-rw-r--r--   0        0        0    11517 2023-05-10 11:58:43.699679 pref_voting-0.4/pref_voting/dominance_axioms.py
+-rw-r--r--   0        0        0    20643 2023-05-10 11:16:22.353419 pref_voting-0.4/pref_voting/generate_profiles.py
+-rw-r--r--   0        0        0     4347 2023-06-01 01:15:48.220008 pref_voting-0.4/pref_voting/generate_spatial_profiles.py
+-rw-r--r--   0        0        0     4830 2023-05-31 22:37:40.105742 pref_voting-0.4/pref_voting/generate_utility_profiles.py
+-rw-r--r--   0        0        0    10486 2023-05-24 13:13:45.272860 pref_voting-0.4/pref_voting/generate_weighted_majority_graphs.py
+-rw-r--r--   0        0        0     1806 2022-08-08 19:08:16.000000 pref_voting-0.4/pref_voting/helper.py
+-rw-r--r--   0        0        0    74763 2023-05-31 19:44:04.394759 pref_voting-0.4/pref_voting/iterative_methods.py
+-rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-0.4/pref_voting/maj_graph_ex1.png
+-rw-r--r--   0        0        0    59218 2023-05-26 17:44:51.542166 pref_voting-0.4/pref_voting/margin_based_methods.py
+-rw-r--r--   0        0        0    25681 2023-05-10 11:20:32.560828 pref_voting-0.4/pref_voting/other_methods.py
+-rw-r--r--   0        0        0    28614 2023-05-30 20:06:31.706933 pref_voting-0.4/pref_voting/profiles.py
+-rw-r--r--   0        0        0    25273 2023-05-26 17:38:33.040884 pref_voting-0.4/pref_voting/profiles_with_ties.py
+-rw-r--r--   0        0        0    12468 2023-05-26 10:23:18.532269 pref_voting-0.4/pref_voting/rankings.py
+-rw-r--r--   0        0        0    11066 2023-05-26 12:19:11.420399 pref_voting-0.4/pref_voting/scoring_methods.py
+-rw-r--r--   0        0        0     5644 2023-06-01 01:22:29.897147 pref_voting-0.4/pref_voting/spatial_profiles.py
+-rw-r--r--   0        0        0     3066 2023-05-31 23:53:43.134760 pref_voting-0.4/pref_voting/utility_functions.py
+-rw-r--r--   0        0        0     6661 2023-05-26 14:18:34.309764 pref_voting-0.4/pref_voting/utility_methods.py
+-rw-r--r--   0        0        0    15088 2023-05-31 22:37:13.253394 pref_voting-0.4/pref_voting/utility_profiles.py
+-rw-r--r--   0        0        0     8393 2023-05-26 10:50:34.876976 pref_voting-0.4/pref_voting/variable_voter_axioms.py
+-rw-r--r--   0        0        0     5395 2023-05-26 10:54:32.445716 pref_voting-0.4/pref_voting/voting_method.py
+-rw-r--r--   0        0        0      253 2022-07-31 21:02:46.000000 pref_voting-0.4/pref_voting/voting_methods.py
+-rw-r--r--   0        0        0    53001 2023-05-26 17:56:28.071379 pref_voting-0.4/pref_voting/weighted_majority_graphs.py
+-rw-r--r--   0        0        0      687 2023-06-01 01:46:15.071766 pref_voting-0.4/pyproject.toml
+-rw-r--r--   0        0        0     4396 1970-01-01 00:00:00.000000 pref_voting-0.4/setup.py
+-rw-r--r--   0        0        0     4509 1970-01-01 00:00:00.000000 pref_voting-0.4/PKG-INFO
```

### Comparing `pref_voting-0.3.4/LICENSE` & `pref_voting-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.4/README.md` & `pref_voting-0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -60,14 +60,16 @@
 - v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.
 - v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.
 - v0.2.8 (2023-5-16): Add description function to Majority Graphs.
 - v0.2.11 (2023-5-16): Update implementation of Simple Stable Voting and Stable Voting.
 - v0.2.13 (2023-5-24): Improve implementation of split_cycle; Breaking changes: split_cycle_faster renamed split_cycle_Floyd_Warshall and beat_path_faster renamed beat_path_Floyd_Warshall.
 - v0.2.17 (2023-5-25): Add to_linear_profile to ProfileWithTies
 - v0.3.3 (2023-5-26): Add implementations of UtilityProfile and a number of different utility methods.
+- v0.3.4 (2023-5-30): Add write and from_string methods to a UtilityProfile.
+- v0.4 (2023-5-31): Add SpatialProfile class and utility functions for generating utility profiles from spatial profiles; add functions to generate a SpatialProfile.
 
 ## Questions?
 
 Feel free to [send me an email](https://pacuit.org/) if you have questions about the project.
 
 ## License
```

### Comparing `pref_voting-0.3.4/pref_voting/analysis.py` & `pref_voting-0.4/pref_voting/analysis.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.4/pref_voting/axiom.py` & `pref_voting-0.4/pref_voting/axiom.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.4/pref_voting/c1_methods.py` & `pref_voting-0.4/pref_voting/c1_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.4/pref_voting/combined_methods.py` & `pref_voting-0.4/pref_voting/combined_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.4/pref_voting/dominance_axioms.py` & `pref_voting-0.4/pref_voting/dominance_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.4/pref_voting/generate_profiles.py` & `pref_voting-0.4/pref_voting/generate_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.4/pref_voting/generate_utility_profiles.py` & `pref_voting-0.4/pref_voting/generate_utility_profiles.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,14 +6,17 @@
     
     Functions to generate utility profiles.
 '''
 
 
 from math import ceil
 import numpy as np
+from scipy.spatial import distance
+from functools import partial
+
 from pref_voting.utility_profiles import UtilityProfile
 
 # turn off future warnings.
 # getting the following warning when calling tabulate to display a profile: 
 # /Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/tabulate.py:1027: FutureWarning: elementwise comparison failed; returning scalar instead, but in the future will perform elementwise comparison
 #  if headers == "keys" and not rows:
 # see https://stackoverflow.com/questions/40659212/futurewarning-elementwise-comparison-failed-returning-scalar-but-in-the-futur
@@ -58,61 +61,83 @@
     mean_utilities = {c: np.random.uniform(0, 1) for c in range(num_candidates)}
     utilities = [{c: np.random.normal(mean_utilities[c], std) for c in range(num_candidates)} 
                  for _ in range(num_voters)]
     
     return UtilityProfile(utilities).normalize()
 
 
-def voter_utility(v_pos, c_pos, beta):
-    """Based on the Rabinowitz and Macdonald (1989) mixed model described in Section 3, pp. 745 - 747 of
-    "Voting behavior under the directional spatial model of electoral competition" by S. Merrill III.
-
-    beta = 1 is the proximity model
-    beta = 0 is the directional model
 
-    Args:
-        v_pos (numpy array): The position(s) of the voter.
-        c_pos (numpy array): The position(s) of the candidate.
-        beta (float): The beta parameter of the mixed model.
+utility_functions = {
+    "RM": {
+        "func": mixed_rm_utility,
+        "param": 1
+    },
+    "Linear": {
+        "func": linear_utility,
+        "param": None
+    },
+    "Quadratic": 
+    {   
+        "func": quadratic_utility,
+        "param": None
+    },
+    "Shepsle": {
+        "func": shepsle_utility,
+        "param": None
+    },
+    "City Block": { 
+        "func": city_block_utility,
+        "param": None
+    },
+    "Matthews": { 
+        "func": matthews_utility,
+        "param": None
+    }
+
+}
+def generate_spatial_utility_profile(num_cands, 
+                                     num_voters, 
+                                     num_dims = 2, 
+                                     utility_function = "Quadratic", 
+                                     utility_function_param = None):
     
-    Returns:
-        float: The utility of the candidate to the voter.
     """
-    return 2 * np.dot(v_pos, c_pos) - beta * (
-        np.linalg.norm(v_pos) ** 2 + np.linalg.norm(c_pos) ** 2
-    )
-
+    Create a spatial utility profile using specified utility functions. 
 
-def generate_spatial_utility_profile(num_cands, num_voters, params = None):
-    """
-    Create a spatial utility profile using the Rabinowitz and Macdonald (1989) mixed model described in Section 3, pp. 745 - 747 of "Voting behavior under the directional spatial model of electoral competition" by S. Merrill III. 
-
-    .. note:  When, beta = 1, it is the proximity model (i.e., utilities are the negative of the squared Euclidean distance), and when beta = 0, it is the directional model.
 
     Args:
         num_cands (int): The number of candidates.
         num_voters (int): The number of voters.
-        params (tuple): A tuple of the form (num_dim, beta) where num_dim is the number of dimensions and beta is the beta parameter of the mixed model. The default is (2, 1).
-
+        num_dims (int): The number of dimensions. The default is 2.
+        utility_function (str): The utility function to use. The default is "Linear".
+        utility_function_param (float): The parameter of the utility function. The default is None.
+        
     Returns:
         UtilityProfile: A spatial utility profile.
     """
-    params = params if params is not None else (2, 1)
 
     # the first component of the parameter is the number of dimensions, 
     # the second component is used to define the mixed model: 
     # beta = 1 is proximity model (i.e., squared Euclidean distance)
-    num_dim, beta = params
 
-    mean = [0] * num_dim  # mean is 0 for each dimension
-    cov = np.diag([1] * num_dim)  # diagonal covariance
+    mean = [0] * num_dims  # mean is 0 for each dimension
+    cov = np.diag([1] * num_dims)  # diagonal covariance
+
+    _utility_fnc = utility_functions[utility_function]["func"]
+
+    if utility_functions[utility_function]["param"] is not None or utility_function_param is not None: 
+        util_parm = utility_function_param  if utility_function_param is not None else utility_functions[utility_function]["param"]
+        utility_fnc = partial(_utility_fnc, util_parm)
+
+    else: 
+        utility_fnc = _utility_fnc
 
     # sample candidate/voter positions using a multivariate normal distribution
     cand_positions = np.random.multivariate_normal(np.array(mean), cov, num_cands)
     voter_positions = np.random.multivariate_normal(np.array(mean), cov, num_voters)
 
-    utilities = [{c: voter_utility(v_pos, c_pos, beta) for c, c_pos in enumerate(cand_positions)} 
+    utilities = [{c: utility_fnc(v_pos, c_pos)  for c, c_pos in enumerate(cand_positions)} 
                  for _, v_pos in enumerate(voter_positions)]
 
     return UtilityProfile(utilities)
```

### Comparing `pref_voting-0.3.4/pref_voting/generate_weighted_majority_graphs.py` & `pref_voting-0.4/pref_voting/generate_weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.4/pref_voting/helper.py` & `pref_voting-0.4/pref_voting/helper.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.4/pref_voting/iterative_methods.py` & `pref_voting-0.4/pref_voting/iterative_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
                        if not isin(cands_to_ignore,c) and _num_rank_first(rs, rcounts, cands_to_ignore, c) >= strict_maj_size]
      
     return sorted(winners)
 
 
 @vm(name = "Instant Runoff PUT")
 def instant_runoff_put(profile, curr_cands = None):
-    """Instant Runoff (:func:`instant_runoff`) with parallel universe tie-breaking (PUT), defined recursively: if there is a candidate with a strict majority of first-place votes, that candidate is the IRV-PUT winner; otherwise a candidate x is an IRV-PUT winner if there is some candidate y with minimal plurality score such that after removing y from the profile, x is an IRV-PUT winner.
+    """Instant Runoff (:func:`instant_runoff`) with parallel universe tie-breaking (PUT), defined recursively: if there is a candidate with a strict majority of first-place votes, that candidate is the IRV-PUT winner; otherwise a candidate x is an IRV-PUT winner if there is some candidate y with a minimal number of first-place votes such that after removing y from the profile, x is an IRV-PUT winner.
     
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
     Returns: 
         A sorted list of candidates
@@ -648,25 +648,25 @@
             winners = [c for c in candidates 
                        if not isin(cands_to_ignore,c) and _num_rank_first(rs, rcounts, cands_to_ignore, c) >= strict_maj_size]
 
     return sorted(winners)
 
 @vm(name = "Coombs PUT")
 def coombs_put(profile, curr_cands = None):
-    """Coombs with parallel universe tie-breaking (PUT).  Apply the Coombs method with a tie-breaker for each possible linear order over the candidates. 
+    """Coombs with parallel universe tie-breaking (PUT), defined recursively: if there is a candidate with a strict majority of first-place votes, that candidate is the Coombs-PUT winner; otherwise a candidate x is a Coombs-PUT winner if there is some candidate y with a maximal number of last-place votes such that after removing y from the profile, x is a Coombs-PUT winner.
     
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
     Returns: 
         A sorted list of candidates
 
     .. warning:: 
-        This will take a long time on profiles with many candidates. 
+        This will take a long time on profiles with many candidates having the same number of last-place votes.
 
     :Example: 
 
     .. exec_code:: 
 
         from pref_voting.profiles import Profile
         from pref_voting.iterative_methods import coombs, coombs_tb, coombs_put
@@ -688,29 +688,35 @@
         coombs_tb.display(prof, tie_breaker=[2, 0, 1])
         print("tie_breaker = [2, 1, 0]")
         coombs_tb.display(prof, tie_breaker=[2, 1, 0])
         print()
         coombs_put.display(prof)
     """
 
-    candidates = profile.candidates if curr_cands is None else curr_cands
+    candidates = profile.candidates if curr_cands is None else curr_cands 
+    cands_to_ignore = np.empty(0) if curr_cands is None else np.array([c for c in profile.candidates if c not in curr_cands])
 
     strict_maj_size = profile.strict_maj_size()
+    majority_winner = [cand for cand, value in profile.plurality_scores(candidates).items() if value >= strict_maj_size]
+
+    if len(majority_winner) > 0:
+        return majority_winner
     
     rs, rcounts = profile.rankings_counts # get all the ranking data
     
-    winners = [c for c in candidates 
-               if _num_rank_first(rs, rcounts, np.empty(0), c) >= strict_maj_size]
+    last_place_scores = {c: _num_rank_last(rs, rcounts, cands_to_ignore, c) for c in candidates}  
+    max_last_place_score = max(last_place_scores.values())
+    cands_to_remove = [c for c in last_place_scores.keys() if last_place_scores[c] == max_last_place_score]
 
-    if len(winners) == 0:
-        # run Coombs with tie-breaker for each permutation of candidates
-        for tb in permutations(candidates):
-            winners += coombs_tb(profile, curr_cands = curr_cands, tie_breaker = tb) 
-
-    return sorted(list(set(winners)))
+    winners = []
+    for cand_to_remove in cands_to_remove:
+        new_winners = coombs_put(profile, curr_cands = [c for c in candidates if not c == cand_to_remove])
+        winners = winners + new_winners
+    
+    return sorted(set(winners))
 
 def coombs_with_explanation(profile, curr_cands = None):
     """
     Coombs with an explanation. In addition to the winner(s), return the order in which the candidates are eliminated as a list of lists.    
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
```

### Comparing `pref_voting-0.3.4/pref_voting/maj_graph_ex1.png` & `pref_voting-0.4/pref_voting/maj_graph_ex1.png`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.4/pref_voting/margin_based_methods.py` & `pref_voting-0.4/pref_voting/margin_based_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.4/pref_voting/other_methods.py` & `pref_voting-0.4/pref_voting/other_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.4/pref_voting/profiles.py` & `pref_voting-0.4/pref_voting/profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.4/pref_voting/profiles_with_ties.py` & `pref_voting-0.4/pref_voting/profiles_with_ties.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.4/pref_voting/rankings.py` & `pref_voting-0.4/pref_voting/rankings.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.4/pref_voting/scoring_methods.py` & `pref_voting-0.4/pref_voting/scoring_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.4/pref_voting/utility_methods.py` & `pref_voting-0.4/pref_voting/utility_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.4/pref_voting/utility_profiles.py` & `pref_voting-0.4/pref_voting/utility_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.4/pref_voting/variable_voter_axioms.py` & `pref_voting-0.4/pref_voting/variable_voter_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.4/pref_voting/voting_method.py` & `pref_voting-0.4/pref_voting/voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.4/pref_voting/weighted_majority_graphs.py` & `pref_voting-0.4/pref_voting/weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.4/pyproject.toml` & `pref_voting-0.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "pref_voting"
-version = "0.3.4"
+version = "0.4"
 description = "pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of voting methods."
 authors = ["Eric Pacuit <epacuit@umd.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/voting-tools/pref_voting"
 repository = "https://github.com/voting-tools/pref_voting"
```

### Comparing `pref_voting-0.3.4/setup.py` & `pref_voting-0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,17 +12,17 @@
  'networkx>=3.0,<4.0',
  'random2>=1.0.1,<2.0.0',
  'scipy>=1.0.0,<2.0.0',
  'tabulate>=0.9.0,<0.10.0']
 
 setup_kwargs = {
     'name': 'pref-voting',
-    'version': '0.3.4',
+    'version': '0.4',
     'description': 'pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of voting methods.',
-    'long_description': 'pref_voting\n==========\n\n## Installation\n\nWith pip package manager:\n\n```bash\npip install pref_voting\n```\n## Documentation\n\nOnline documentation is available at [https://pref_voting.readthedocs.io](https://pref_voting.readthedocs.io).\n\n## Profiles and Voting Methods\n\nA profile (of linear orders over the candidates) is created by initializing a Profile class object.  This needs a list of rankings (each ranking is a tuple of numbers), the number of candidates, and a list giving the number of each ranking in the profile:\n\n```python\nfrom pref_voting.profiles import Profile\n\nrankings = [(0, 1, 2, 3), (2, 3, 1, 0), (3, 1, 2, 0), (1, 2, 0, 3), (1, 3, 2, 0)]\nrcounts = [5, 3, 2, 4, 3]\n\nprof = Profile(rankings, rcounts=rcounts)\n```\n\nThe function generate_profile is used to generate a profile for a given number of candidates and voters:  \n```python\nfrom pref_voting.generate_profiles import generate_profile\n\n# generate a profile using the Impartial Culture probability model\nprof = generate_profile(3, 4) # prof is a Profile object\n\n# generate a profile using the Impartial Anonymous Culture probability model\nprof = generate_profile(3, 4, probmod = "IAC") # prof is a Profile object \n```\n\n```python\nfrom pref_voting.profiles import Profile\nfrom pref_voting.voting_methods import *\n\nprof = Profile(rankings, num_cands, rcounts=rcounts)\nprint(f"{split_cycle.name} winners:  {split_cycle(prof)}")\nsplit_cycle.display(prof)\n\n```\n\n## Versions\n\n- v0.1.10 (2022-08-09): **Initial release** \n- v0.1.13 (2022-11-05): Minor updates and bug fixes \n- v0.1.14 (2022-12-19): Add plurality_scores to ProfileWithTies; add generate ceots function; bug fixes \n- v0.1.23 (2022-12-27): Add instant_runoff_for_truncated_linear_orders and functions to truncate overvotes in a ProfileWithTies, add smith_irv_put, document analysis functions\n- v0.1.25 (2023-1-11): Add condorcet_irv, condorcet_irv_put; Update documentation; add axioms.py; add display and equality to Ranking class; fix enumerate ceots functions\n- v0.1.27 (2023-2-07): Add Borda for ProfileWithTies\n- v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies\n- v0.2.1 (2023-2-15): Bug fixes\n- v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation\n- v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.\n- v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.\n- v0.2.8 (2023-5-16): Add description function to Majority Graphs.\n- v0.2.11 (2023-5-16): Update implementation of Simple Stable Voting and Stable Voting.\n- v0.2.13 (2023-5-24): Improve implementation of split_cycle; Breaking changes: split_cycle_faster renamed split_cycle_Floyd_Warshall and beat_path_faster renamed beat_path_Floyd_Warshall.\n- v0.2.17 (2023-5-25): Add to_linear_profile to ProfileWithTies\n- v0.3.3 (2023-5-26): Add implementations of UtilityProfile and a number of different utility methods.\n\n## Questions?\n\nFeel free to [send me an email](https://pacuit.org/) if you have questions about the project.\n\n## License\n\n[MIT](https://github.com/jontingvold/pyrankvote/blob/master/LICENSE.txt)\n',
+    'long_description': 'pref_voting\n==========\n\n## Installation\n\nWith pip package manager:\n\n```bash\npip install pref_voting\n```\n## Documentation\n\nOnline documentation is available at [https://pref_voting.readthedocs.io](https://pref_voting.readthedocs.io).\n\n## Profiles and Voting Methods\n\nA profile (of linear orders over the candidates) is created by initializing a Profile class object.  This needs a list of rankings (each ranking is a tuple of numbers), the number of candidates, and a list giving the number of each ranking in the profile:\n\n```python\nfrom pref_voting.profiles import Profile\n\nrankings = [(0, 1, 2, 3), (2, 3, 1, 0), (3, 1, 2, 0), (1, 2, 0, 3), (1, 3, 2, 0)]\nrcounts = [5, 3, 2, 4, 3]\n\nprof = Profile(rankings, rcounts=rcounts)\n```\n\nThe function generate_profile is used to generate a profile for a given number of candidates and voters:  \n```python\nfrom pref_voting.generate_profiles import generate_profile\n\n# generate a profile using the Impartial Culture probability model\nprof = generate_profile(3, 4) # prof is a Profile object\n\n# generate a profile using the Impartial Anonymous Culture probability model\nprof = generate_profile(3, 4, probmod = "IAC") # prof is a Profile object \n```\n\n```python\nfrom pref_voting.profiles import Profile\nfrom pref_voting.voting_methods import *\n\nprof = Profile(rankings, num_cands, rcounts=rcounts)\nprint(f"{split_cycle.name} winners:  {split_cycle(prof)}")\nsplit_cycle.display(prof)\n\n```\n\n## Versions\n\n- v0.1.10 (2022-08-09): **Initial release** \n- v0.1.13 (2022-11-05): Minor updates and bug fixes \n- v0.1.14 (2022-12-19): Add plurality_scores to ProfileWithTies; add generate ceots function; bug fixes \n- v0.1.23 (2022-12-27): Add instant_runoff_for_truncated_linear_orders and functions to truncate overvotes in a ProfileWithTies, add smith_irv_put, document analysis functions\n- v0.1.25 (2023-1-11): Add condorcet_irv, condorcet_irv_put; Update documentation; add axioms.py; add display and equality to Ranking class; fix enumerate ceots functions\n- v0.1.27 (2023-2-07): Add Borda for ProfileWithTies\n- v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies\n- v0.2.1 (2023-2-15): Bug fixes\n- v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation\n- v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.\n- v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.\n- v0.2.8 (2023-5-16): Add description function to Majority Graphs.\n- v0.2.11 (2023-5-16): Update implementation of Simple Stable Voting and Stable Voting.\n- v0.2.13 (2023-5-24): Improve implementation of split_cycle; Breaking changes: split_cycle_faster renamed split_cycle_Floyd_Warshall and beat_path_faster renamed beat_path_Floyd_Warshall.\n- v0.2.17 (2023-5-25): Add to_linear_profile to ProfileWithTies\n- v0.3.3 (2023-5-26): Add implementations of UtilityProfile and a number of different utility methods.\n- v0.3.4 (2023-5-30): Add write and from_string methods to a UtilityProfile.\n- v0.4 (2023-5-31): Add SpatialProfile class and utility functions for generating utility profiles from spatial profiles; add functions to generate a SpatialProfile.\n\n## Questions?\n\nFeel free to [send me an email](https://pacuit.org/) if you have questions about the project.\n\n## License\n\n[MIT](https://github.com/jontingvold/pyrankvote/blob/master/LICENSE.txt)\n',
     'author': 'Eric Pacuit',
     'author_email': 'epacuit@umd.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/voting-tools/pref_voting',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pref_voting-0.3.4/PKG-INFO` & `pref_voting-0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pref-voting
-Version: 0.3.4
+Version: 0.4
 Summary: pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of voting methods.
 Home-page: https://github.com/voting-tools/pref_voting
 License: MIT
 Author: Eric Pacuit
 Author-email: epacuit@umd.edu
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -85,14 +85,16 @@
 - v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.
 - v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.
 - v0.2.8 (2023-5-16): Add description function to Majority Graphs.
 - v0.2.11 (2023-5-16): Update implementation of Simple Stable Voting and Stable Voting.
 - v0.2.13 (2023-5-24): Improve implementation of split_cycle; Breaking changes: split_cycle_faster renamed split_cycle_Floyd_Warshall and beat_path_faster renamed beat_path_Floyd_Warshall.
 - v0.2.17 (2023-5-25): Add to_linear_profile to ProfileWithTies
 - v0.3.3 (2023-5-26): Add implementations of UtilityProfile and a number of different utility methods.
+- v0.3.4 (2023-5-30): Add write and from_string methods to a UtilityProfile.
+- v0.4 (2023-5-31): Add SpatialProfile class and utility functions for generating utility profiles from spatial profiles; add functions to generate a SpatialProfile.
 
 ## Questions?
 
 Feel free to [send me an email](https://pacuit.org/) if you have questions about the project.
 
 ## License
```

