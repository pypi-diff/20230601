# Comparing `tmp/ab-test-simulator-0.0.2.tar.gz` & `tmp/ab-test-simulator-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ab-test-simulator-0.0.2.tar", last modified: Thu Jun  1 11:42:54 2023, max compression
+gzip compressed data, was "ab-test-simulator-0.0.3.tar", last modified: Thu Jun  1 14:41:44 2023, max compression
```

## Comparing `ab-test-simulator-0.0.2.tar` & `ab-test-simulator-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-01 11:42:54.667098 ab-test-simulator-0.0.2/
--rw-rw-r--   0 koljakleineberg   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ab-test-simulator-0.0.2/LICENSE
--rw-rw-r--   0 koljakleineberg   (501) staff       (20)      111 2023-04-27 10:12:58.000000 ab-test-simulator-0.0.2/MANIFEST.in
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     8762 2023-06-01 11:42:54.666899 ab-test-simulator-0.0.2/PKG-INFO
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     5899 2023-06-01 11:35:44.000000 ab-test-simulator-0.0.2/README.md
-drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-01 11:42:54.665704 ab-test-simulator-0.0.2/ab_test_simulator/
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       22 2023-06-01 11:35:25.000000 ab-test-simulator-0.0.2/ab_test_simulator/__init__.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     2847 2023-06-01 11:35:25.000000 ab-test-simulator-0.0.2/ab_test_simulator/_modidx.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     2746 2023-06-01 11:35:25.000000 ab-test-simulator-0.0.2/ab_test_simulator/generator.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     9436 2023-06-01 11:35:25.000000 ab-test-simulator-0.0.2/ab_test_simulator/power.py
-drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-01 11:42:54.666713 ab-test-simulator-0.0.2/ab_test_simulator.egg-info/
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     8762 2023-06-01 11:42:54.000000 ab-test-simulator-0.0.2/ab_test_simulator.egg-info/PKG-INFO
--rw-r--r--   0 koljakleineberg   (501) staff       (20)      456 2023-06-01 11:42:54.000000 ab-test-simulator-0.0.2/ab_test_simulator.egg-info/SOURCES.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)        1 2023-06-01 11:42:54.000000 ab-test-simulator-0.0.2/ab_test_simulator.egg-info/dependency_links.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       77 2023-06-01 11:42:54.000000 ab-test-simulator-0.0.2/ab_test_simulator.egg-info/entry_points.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)        1 2023-05-31 12:40:20.000000 ab-test-simulator-0.0.2/ab_test_simulator.egg-info/not-zip-safe
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       98 2023-06-01 11:42:54.000000 ab-test-simulator-0.0.2/ab_test_simulator.egg-info/requires.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       18 2023-06-01 11:42:54.000000 ab-test-simulator-0.0.2/ab_test_simulator.egg-info/top_level.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     1054 2023-06-01 11:20:27.000000 ab-test-simulator-0.0.2/settings.ini
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       38 2023-06-01 11:42:54.667128 ab-test-simulator-0.0.2/setup.cfg
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     2711 2023-06-01 06:53:26.000000 ab-test-simulator-0.0.2/setup.py
+drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-01 14:41:44.814565 ab-test-simulator-0.0.3/
+-rw-rw-r--   0 koljakleineberg   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ab-test-simulator-0.0.3/LICENSE
+-rw-rw-r--   0 koljakleineberg   (501) staff       (20)      111 2023-04-27 10:12:58.000000 ab-test-simulator-0.0.3/MANIFEST.in
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     7419 2023-06-01 14:41:44.814458 ab-test-simulator-0.0.3/PKG-INFO
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     5020 2023-06-01 14:37:46.000000 ab-test-simulator-0.0.3/README.md
+drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-01 14:41:44.813158 ab-test-simulator-0.0.3/ab_test_simulator/
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       22 2023-06-01 14:39:35.000000 ab-test-simulator-0.0.3/ab_test_simulator/__init__.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     3218 2023-06-01 14:39:35.000000 ab-test-simulator-0.0.3/ab_test_simulator/_modidx.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     2198 2023-06-01 14:39:35.000000 ab-test-simulator-0.0.3/ab_test_simulator/generator.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     3539 2023-06-01 14:39:35.000000 ab-test-simulator-0.0.3/ab_test_simulator/plotting.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     7904 2023-06-01 14:39:35.000000 ab-test-simulator-0.0.3/ab_test_simulator/power.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)      475 2023-06-01 14:32:32.000000 ab-test-simulator-0.0.3/ab_test_simulator/wrappers.py
+drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-01 14:41:44.814254 ab-test-simulator-0.0.3/ab_test_simulator.egg-info/
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     7419 2023-06-01 14:41:44.000000 ab-test-simulator-0.0.3/ab_test_simulator.egg-info/PKG-INFO
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)      516 2023-06-01 14:41:44.000000 ab-test-simulator-0.0.3/ab_test_simulator.egg-info/SOURCES.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)        1 2023-06-01 14:41:44.000000 ab-test-simulator-0.0.3/ab_test_simulator.egg-info/dependency_links.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       77 2023-06-01 14:41:44.000000 ab-test-simulator-0.0.3/ab_test_simulator.egg-info/entry_points.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)        1 2023-05-31 12:40:20.000000 ab-test-simulator-0.0.3/ab_test_simulator.egg-info/not-zip-safe
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       98 2023-06-01 14:41:44.000000 ab-test-simulator-0.0.3/ab_test_simulator.egg-info/requires.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       18 2023-06-01 14:41:44.000000 ab-test-simulator-0.0.3/ab_test_simulator.egg-info/top_level.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     1054 2023-06-01 14:38:46.000000 ab-test-simulator-0.0.3/settings.ini
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       38 2023-06-01 14:41:44.814600 ab-test-simulator-0.0.3/setup.cfg
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     2711 2023-06-01 06:53:26.000000 ab-test-simulator-0.0.3/setup.py
```

### Comparing `ab-test-simulator-0.0.2/LICENSE` & `ab-test-simulator-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ab-test-simulator-0.0.2/PKG-INFO` & `ab-test-simulator-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ab-test-simulator
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple library to simulate AB tests.
 Home-page: https://github.com/k111git/ab-test-simulator
 Author: Kolja
 Author-email: 
 License: Apache Software License 2.0
 Description: # ab-test-simulator
         
@@ -18,23 +18,27 @@
         
         ## imports
         
         ``` python
         from ab_test_simulator.generator import (
             generate_binary_data,
             generate_continuous_data,
-            plot_distribution,
+            data_to_contingency,
         )
         from ab_test_simulator.power import (
             simulate_power_binary,
             sample_size_chi2,
-            plot_power,
             simulate_power_continuous,
             continuous_sample_size,
         )
+        from ab_test_simulator.plotting import (
+            plot_power,
+            plot_distribution,
+            plot_betas,
+        )
         ```
         
         ## Binary target (e.g. conversion rate experiments)
         
         ### Sample size:
         
         We can calculate the sample size required with the function
@@ -101,84 +105,24 @@
         Let us analyze the statistical power with synthethic data. We can do
         this with the simulate_power_binary function. We are using some default
         argument here, see [this
         page](https://k111git.github.io/ab-test-simulator/power.html) for more
         information.
         
         ``` python
-        simulation = simulate_power_binary()
+        # simulation = simulate_power_binary()
         ```
         
-            One sided.
-            0 done
-            1 done
-            2 done
-            3 done
-            4 done
-            5 done
-            6 done
-            7 done
-            8 done
-            9 done
-        
         Note: The simulation object return the total sample size, so we need to
         split it per variant.
         
         ``` python
-        simulation
+        # simulation
         ```
         
-            {'sizes': array([ 10000,  20000,  30000,  40000,  50000,  60000,  70000,  80000,
-                     90000, 100000]),
-             'approaches': ['fisher', 'chi', 'z', 'bayes'],
-             'power_fisher': [0.212,
-              0.381,
-              0.493,
-              0.576,
-              0.686,
-              0.759,
-              0.789,
-              0.849,
-              0.899,
-              0.913],
-             'sample_size_fisher': 72282.01499480086,
-             'power_chi': [0.213,
-              0.383,
-              0.492,
-              0.576,
-              0.686,
-              0.759,
-              0.789,
-              0.849,
-              0.899,
-              0.913],
-             'sample_size_chi': 72282.58033018697,
-             'power_z': [0.242,
-              0.401,
-              0.518,
-              0.604,
-              0.704,
-              0.77,
-              0.795,
-              0.864,
-              0.9,
-              0.916],
-             'sample_size_z': 70976.35907745312,
-             'power_bayes': [0.237,
-              0.395,
-              0.524,
-              0.596,
-              0.701,
-              0.766,
-              0.796,
-              0.861,
-              0.902,
-              0.919],
-             'sample_size_bayes': 70798.83069867057}
-        
         Finally, we can plot the results (note: the plot function show the
         sample size per variant):
         
         ``` python
         # plot_power(
         #     simulation,
         #     added_lines=[{"sample_size": sample_size_chi2(), "label": "Chi2"}],
@@ -221,29 +165,17 @@
         
             Required sample size per variant is 4946.
         
         Let us also do some simulations. These show results for the t-test as
         well as bayesian testing (only 1-sided).
         
         ``` python
-        simulation = simulate_power_continuous()
+        # simulation = simulate_power_continuous()
         ```
         
-            One sided.
-            0 done
-            1 done
-            2 done
-            3 done
-            4 done
-            5 done
-            6 done
-            7 done
-            8 done
-            9 done
-        
         ``` python
         # plot_power(
         #     simulation,
         #     added_lines=[
         #         {"sample_size": continuous_sample_size(), "label": "Formula"}
         #     ],
         # )
@@ -264,14 +196,24 @@
         Distribution with effect:
         
         ``` python
         df_continuous = generate_continuous_data(effect=1)
         # plot_distribution(df_continuous)
         ```
         
+        ## Visualizations
+        
+        Plot beta distributions for a contingency table:
+        
+        ``` python
+        df = generate_binary_data()
+        df_contingency = data_to_contingency(df)
+        # plot_betas(df_contingency, xmin=0, xmax=0.04)
+        ```
+        
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ab-test-simulator-0.0.2/README.md` & `ab-test-simulator-0.0.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -10,23 +10,27 @@
 
 ## imports
 
 ``` python
 from ab_test_simulator.generator import (
     generate_binary_data,
     generate_continuous_data,
-    plot_distribution,
+    data_to_contingency,
 )
 from ab_test_simulator.power import (
     simulate_power_binary,
     sample_size_chi2,
-    plot_power,
     simulate_power_continuous,
     continuous_sample_size,
 )
+from ab_test_simulator.plotting import (
+    plot_power,
+    plot_distribution,
+    plot_betas,
+)
 ```
 
 ## Binary target (e.g. conversion rate experiments)
 
 ### Sample size:
 
 We can calculate the sample size required with the function
@@ -93,84 +97,24 @@
 Let us analyze the statistical power with synthethic data. We can do
 this with the simulate_power_binary function. We are using some default
 argument here, see [this
 page](https://k111git.github.io/ab-test-simulator/power.html) for more
 information.
 
 ``` python
-simulation = simulate_power_binary()
+# simulation = simulate_power_binary()
 ```
 
-    One sided.
-    0 done
-    1 done
-    2 done
-    3 done
-    4 done
-    5 done
-    6 done
-    7 done
-    8 done
-    9 done
-
 Note: The simulation object return the total sample size, so we need to
 split it per variant.
 
 ``` python
-simulation
+# simulation
 ```
 
-    {'sizes': array([ 10000,  20000,  30000,  40000,  50000,  60000,  70000,  80000,
-             90000, 100000]),
-     'approaches': ['fisher', 'chi', 'z', 'bayes'],
-     'power_fisher': [0.212,
-      0.381,
-      0.493,
-      0.576,
-      0.686,
-      0.759,
-      0.789,
-      0.849,
-      0.899,
-      0.913],
-     'sample_size_fisher': 72282.01499480086,
-     'power_chi': [0.213,
-      0.383,
-      0.492,
-      0.576,
-      0.686,
-      0.759,
-      0.789,
-      0.849,
-      0.899,
-      0.913],
-     'sample_size_chi': 72282.58033018697,
-     'power_z': [0.242,
-      0.401,
-      0.518,
-      0.604,
-      0.704,
-      0.77,
-      0.795,
-      0.864,
-      0.9,
-      0.916],
-     'sample_size_z': 70976.35907745312,
-     'power_bayes': [0.237,
-      0.395,
-      0.524,
-      0.596,
-      0.701,
-      0.766,
-      0.796,
-      0.861,
-      0.902,
-      0.919],
-     'sample_size_bayes': 70798.83069867057}
-
 Finally, we can plot the results (note: the plot function show the
 sample size per variant):
 
 ``` python
 # plot_power(
 #     simulation,
 #     added_lines=[{"sample_size": sample_size_chi2(), "label": "Chi2"}],
@@ -213,29 +157,17 @@
 
     Required sample size per variant is 4946.
 
 Let us also do some simulations. These show results for the t-test as
 well as bayesian testing (only 1-sided).
 
 ``` python
-simulation = simulate_power_continuous()
+# simulation = simulate_power_continuous()
 ```
 
-    One sided.
-    0 done
-    1 done
-    2 done
-    3 done
-    4 done
-    5 done
-    6 done
-    7 done
-    8 done
-    9 done
-
 ``` python
 # plot_power(
 #     simulation,
 #     added_lines=[
 #         {"sample_size": continuous_sample_size(), "label": "Formula"}
 #     ],
 # )
@@ -255,7 +187,17 @@
 
 Distribution with effect:
 
 ``` python
 df_continuous = generate_continuous_data(effect=1)
 # plot_distribution(df_continuous)
 ```
+
+## Visualizations
+
+Plot beta distributions for a contingency table:
+
+``` python
+df = generate_binary_data()
+df_contingency = data_to_contingency(df)
+# plot_betas(df_contingency, xmin=0, xmax=0.04)
+```
```

### Comparing `ab-test-simulator-0.0.2/ab_test_simulator/generator.py` & `ab-test-simulator-0.0.3/ab_test_simulator/generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_data_generation.ipynb.
 
 # %% auto 0
-__all__ = ['generate_binary_data', 'generate_continuous_data', 'data_to_contingency', 'plot_distribution']
+__all__ = ['generate_binary_data', 'generate_continuous_data', 'data_to_contingency']
 
 # %% ../nbs/00_data_generation.ipynb 4
 import numpy as np
 from scipy.stats import binom
 import pandas as pd
 
 import plotly.graph_objects as go
@@ -40,45 +40,23 @@
     """
     Generates synthethic data for a continuous experiement with two groups (0: Control, 1: Variant).
     Inputs:
     N: Sample size (total number of users)
     """
     i = range(1, N + 1)
     d = np.random.binomial(1, split, N)
-#     y0 = base + effect * d + noise * np.random.normal(0, std, N)
+    #     y0 = base + effect * d + noise * np.random.normal(0, std, N)
     y0 = np.random.normal(base + effect * d, std, N)
     df = pd.DataFrame({"individual": i, "group": d, "target": y0})
     return df
 
 # %% ../nbs/00_data_generation.ipynb 10
 def data_to_contingency(df):
     """
     Converts output from generate_binary_data to a contingency table
     """
     df_result = df.groupby("group").agg(
         users=("target", "size"), converted=("target", "sum")
     )
     df_result["not_converted"] = df_result["users"] - df_result["converted"]
+    df_result["cvr"] = df_result["converted"] / df_result["users"]
     return df_result
-
-# %% ../nbs/00_data_generation.ipynb 11
-def plot_distribution(df):
-    """
-    Plots the distribution for both groups of generate_continuous_data
-    """
-    fig = ff.create_distplot(
-        [
-            df[df["group"] == 0]["target"].values,
-            df[df["group"] == 1]["target"].values,
-        ],
-        ["Control", "Variant"],
-        show_hist=False,
-        show_rug=True,
-    )
-
-    fig.update_layout(
-        template="simple_white",
-        xaxis_title="Target",
-        yaxis_title="PDF",
-        legend=dict(yanchor="top", y=0.99, xanchor="right", x=0.95),
-    )
-    return fig
```

### Comparing `ab-test-simulator-0.0.2/ab_test_simulator/power.py` & `ab-test-simulator-0.0.3/ab_test_simulator/power.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/01_power.ipynb.
 
 # %% auto 0
-__all__ = ['simulate_power_binary', 'sample_size_chi2', 'plot_power', 'simulate_power_continuous', 'continuous_sample_size']
+__all__ = ['simulate_power_binary', 'sample_size_chi2', 'simulate_power_continuous', 'continuous_sample_size']
 
 # %% ../nbs/01_power.ipynb 6
 import numpy as np
 import pandas as pd
 
 from scipy import interpolate
 
@@ -142,64 +142,15 @@
 
     required_n = sms.NormalIndPower().solve_power(
         effect_size, power=power, alpha=alpha, ratio=1, alternative=alternative
     )
 
     return required_n
 
-# %% ../nbs/01_power.ipynb 10
-def plot_power(simulation, added_lines=[]):
-    """
-    Takes simulation dict and plots the power over sample sizes
-    Added lines: plot horizontal lines for additional sample size estimations, takes a list of dicts with sample_size=sample_size,label=label
-    """
-    approaches = simulation["approaches"]
-    fig = go.Figure()
-    for approach in approaches:
-        fig.add_trace(
-            go.Scatter(
-                x=simulation["sizes"] / 2.0,
-                y=simulation[f"power_{approach}"],
-                mode="lines+markers",
-                name=approach,
-            )
-        )
-
-    for approach in approaches:
-        fig.add_trace(
-            go.Scatter(
-                x=2 * [simulation[f"sample_size_{approach}"] / 2.0],
-                y=[0, 1],
-                mode="lines",
-                line_dash="dash",
-                name=f"Sample size ({approach})",
-            )
-        )
-    for added_line in added_lines:
-        fig.add_trace(
-            go.Scatter(
-                x=2 * [added_line["sample_size"]],
-                y=[0, 1],
-                mode="lines",
-                line_dash="dash",
-                name=added_line["label"],
-            )
-        )
-
-    fig.update_layout(
-        template="simple_white",
-        xaxis_title="Sample size per variation",
-        yaxis_title="PDF",
-        yaxis_range=[0, 1],
-        legend=dict(yanchor="top", y=1, xanchor="left", x=0.0),
-    )
-    # fig.update_layout(showlegend=True)
-    return fig
-
-# %% ../nbs/01_power.ipynb 13
+# %% ../nbs/01_power.ipynb 11
 def simulate_power_continuous(
     sizes=np.arange(1000, 20001, 2000),
     effect=0.05,
     realizations=1000,
     alpha=0.05,
     one_sided=True,
     power=0.8,
@@ -261,15 +212,15 @@
     out["sizes"] = sizes
     out["approaches"] = approaches
     for approach in approaches:
         out[f"power_{approach}"] = power_lines[approach]
         out[f"sample_size_{approach}"] = sample_sizes[approach]
     return out
 
-# %% ../nbs/01_power.ipynb 16
+# %% ../nbs/01_power.ipynb 14
 def continuous_sample_size(
     mu1=5.00, mu2=5.05, sigma=1, alpha=0.05, power=0.8, one_sided=True
 ):
     """
     forumla: https://towardsdatascience.com/required-sample-size-for-a-b-testing-6f6608dd330a
     web calulator: https://www.stat.ubc.ca/~rollin/stats/ssize/n2.html
     returns sample size per variant
```

### Comparing `ab-test-simulator-0.0.2/ab_test_simulator.egg-info/PKG-INFO` & `ab-test-simulator-0.0.3/ab_test_simulator.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ab-test-simulator
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple library to simulate AB tests.
 Home-page: https://github.com/k111git/ab-test-simulator
 Author: Kolja
 Author-email: 
 License: Apache Software License 2.0
 Description: # ab-test-simulator
         
@@ -18,23 +18,27 @@
         
         ## imports
         
         ``` python
         from ab_test_simulator.generator import (
             generate_binary_data,
             generate_continuous_data,
-            plot_distribution,
+            data_to_contingency,
         )
         from ab_test_simulator.power import (
             simulate_power_binary,
             sample_size_chi2,
-            plot_power,
             simulate_power_continuous,
             continuous_sample_size,
         )
+        from ab_test_simulator.plotting import (
+            plot_power,
+            plot_distribution,
+            plot_betas,
+        )
         ```
         
         ## Binary target (e.g. conversion rate experiments)
         
         ### Sample size:
         
         We can calculate the sample size required with the function
@@ -101,84 +105,24 @@
         Let us analyze the statistical power with synthethic data. We can do
         this with the simulate_power_binary function. We are using some default
         argument here, see [this
         page](https://k111git.github.io/ab-test-simulator/power.html) for more
         information.
         
         ``` python
-        simulation = simulate_power_binary()
+        # simulation = simulate_power_binary()
         ```
         
-            One sided.
-            0 done
-            1 done
-            2 done
-            3 done
-            4 done
-            5 done
-            6 done
-            7 done
-            8 done
-            9 done
-        
         Note: The simulation object return the total sample size, so we need to
         split it per variant.
         
         ``` python
-        simulation
+        # simulation
         ```
         
-            {'sizes': array([ 10000,  20000,  30000,  40000,  50000,  60000,  70000,  80000,
-                     90000, 100000]),
-             'approaches': ['fisher', 'chi', 'z', 'bayes'],
-             'power_fisher': [0.212,
-              0.381,
-              0.493,
-              0.576,
-              0.686,
-              0.759,
-              0.789,
-              0.849,
-              0.899,
-              0.913],
-             'sample_size_fisher': 72282.01499480086,
-             'power_chi': [0.213,
-              0.383,
-              0.492,
-              0.576,
-              0.686,
-              0.759,
-              0.789,
-              0.849,
-              0.899,
-              0.913],
-             'sample_size_chi': 72282.58033018697,
-             'power_z': [0.242,
-              0.401,
-              0.518,
-              0.604,
-              0.704,
-              0.77,
-              0.795,
-              0.864,
-              0.9,
-              0.916],
-             'sample_size_z': 70976.35907745312,
-             'power_bayes': [0.237,
-              0.395,
-              0.524,
-              0.596,
-              0.701,
-              0.766,
-              0.796,
-              0.861,
-              0.902,
-              0.919],
-             'sample_size_bayes': 70798.83069867057}
-        
         Finally, we can plot the results (note: the plot function show the
         sample size per variant):
         
         ``` python
         # plot_power(
         #     simulation,
         #     added_lines=[{"sample_size": sample_size_chi2(), "label": "Chi2"}],
@@ -221,29 +165,17 @@
         
             Required sample size per variant is 4946.
         
         Let us also do some simulations. These show results for the t-test as
         well as bayesian testing (only 1-sided).
         
         ``` python
-        simulation = simulate_power_continuous()
+        # simulation = simulate_power_continuous()
         ```
         
-            One sided.
-            0 done
-            1 done
-            2 done
-            3 done
-            4 done
-            5 done
-            6 done
-            7 done
-            8 done
-            9 done
-        
         ``` python
         # plot_power(
         #     simulation,
         #     added_lines=[
         #         {"sample_size": continuous_sample_size(), "label": "Formula"}
         #     ],
         # )
@@ -264,14 +196,24 @@
         Distribution with effect:
         
         ``` python
         df_continuous = generate_continuous_data(effect=1)
         # plot_distribution(df_continuous)
         ```
         
+        ## Visualizations
+        
+        Plot beta distributions for a contingency table:
+        
+        ``` python
+        df = generate_binary_data()
+        df_contingency = data_to_contingency(df)
+        # plot_betas(df_contingency, xmin=0, xmax=0.04)
+        ```
+        
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ab-test-simulator-0.0.2/settings.ini` & `ab-test-simulator-0.0.3/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = ab-test-simulator
 lib_name = %(repo)s
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = ab_test_simulator
```

### Comparing `ab-test-simulator-0.0.2/setup.py` & `ab-test-simulator-0.0.3/setup.py`

 * *Files identical despite different names*

