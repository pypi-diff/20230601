# Comparing `tmp/ab-test-simulator-0.0.1.tar.gz` & `tmp/ab-test-simulator-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ab-test-simulator-0.0.1.tar", last modified: Thu Jun  1 10:28:56 2023, max compression
+gzip compressed data, was "ab-test-simulator-0.0.2.tar", last modified: Thu Jun  1 11:42:54 2023, max compression
```

## Comparing `ab-test-simulator-0.0.1.tar` & `ab-test-simulator-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-01 10:28:56.710019 ab-test-simulator-0.0.1/
--rw-rw-r--   0 koljakleineberg   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ab-test-simulator-0.0.1/LICENSE
--rw-rw-r--   0 koljakleineberg   (501) staff       (20)      111 2023-04-27 10:12:58.000000 ab-test-simulator-0.0.1/MANIFEST.in
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     3193 2023-06-01 10:28:56.709909 ab-test-simulator-0.0.1/PKG-INFO
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     1610 2023-06-01 10:21:29.000000 ab-test-simulator-0.0.1/README.md
-drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-01 10:28:56.708871 ab-test-simulator-0.0.1/ab_test_simulator/
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       22 2023-06-01 10:25:19.000000 ab-test-simulator-0.0.1/ab_test_simulator/__init__.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     2847 2023-06-01 10:25:19.000000 ab-test-simulator-0.0.1/ab_test_simulator/_modidx.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     2746 2023-06-01 10:25:19.000000 ab-test-simulator-0.0.1/ab_test_simulator/generator.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     9755 2023-06-01 10:25:19.000000 ab-test-simulator-0.0.1/ab_test_simulator/power.py
-drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-01 10:28:56.709702 ab-test-simulator-0.0.1/ab_test_simulator.egg-info/
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     3193 2023-06-01 10:28:56.000000 ab-test-simulator-0.0.1/ab_test_simulator.egg-info/PKG-INFO
--rw-r--r--   0 koljakleineberg   (501) staff       (20)      456 2023-06-01 10:28:56.000000 ab-test-simulator-0.0.1/ab_test_simulator.egg-info/SOURCES.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)        1 2023-06-01 10:28:56.000000 ab-test-simulator-0.0.1/ab_test_simulator.egg-info/dependency_links.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       77 2023-06-01 10:28:56.000000 ab-test-simulator-0.0.1/ab_test_simulator.egg-info/entry_points.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)        1 2023-05-31 12:40:20.000000 ab-test-simulator-0.0.1/ab_test_simulator.egg-info/not-zip-safe
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       98 2023-06-01 10:28:56.000000 ab-test-simulator-0.0.1/ab_test_simulator.egg-info/requires.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       18 2023-06-01 10:28:56.000000 ab-test-simulator-0.0.1/ab_test_simulator.egg-info/top_level.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     1054 2023-05-31 14:20:11.000000 ab-test-simulator-0.0.1/settings.ini
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       38 2023-06-01 10:28:56.710064 ab-test-simulator-0.0.1/setup.cfg
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     2711 2023-06-01 06:53:26.000000 ab-test-simulator-0.0.1/setup.py
+drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-01 11:42:54.667098 ab-test-simulator-0.0.2/
+-rw-rw-r--   0 koljakleineberg   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ab-test-simulator-0.0.2/LICENSE
+-rw-rw-r--   0 koljakleineberg   (501) staff       (20)      111 2023-04-27 10:12:58.000000 ab-test-simulator-0.0.2/MANIFEST.in
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     8762 2023-06-01 11:42:54.666899 ab-test-simulator-0.0.2/PKG-INFO
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     5899 2023-06-01 11:35:44.000000 ab-test-simulator-0.0.2/README.md
+drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-01 11:42:54.665704 ab-test-simulator-0.0.2/ab_test_simulator/
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       22 2023-06-01 11:35:25.000000 ab-test-simulator-0.0.2/ab_test_simulator/__init__.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     2847 2023-06-01 11:35:25.000000 ab-test-simulator-0.0.2/ab_test_simulator/_modidx.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     2746 2023-06-01 11:35:25.000000 ab-test-simulator-0.0.2/ab_test_simulator/generator.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     9436 2023-06-01 11:35:25.000000 ab-test-simulator-0.0.2/ab_test_simulator/power.py
+drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-01 11:42:54.666713 ab-test-simulator-0.0.2/ab_test_simulator.egg-info/
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     8762 2023-06-01 11:42:54.000000 ab-test-simulator-0.0.2/ab_test_simulator.egg-info/PKG-INFO
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)      456 2023-06-01 11:42:54.000000 ab-test-simulator-0.0.2/ab_test_simulator.egg-info/SOURCES.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)        1 2023-06-01 11:42:54.000000 ab-test-simulator-0.0.2/ab_test_simulator.egg-info/dependency_links.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       77 2023-06-01 11:42:54.000000 ab-test-simulator-0.0.2/ab_test_simulator.egg-info/entry_points.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)        1 2023-05-31 12:40:20.000000 ab-test-simulator-0.0.2/ab_test_simulator.egg-info/not-zip-safe
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       98 2023-06-01 11:42:54.000000 ab-test-simulator-0.0.2/ab_test_simulator.egg-info/requires.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       18 2023-06-01 11:42:54.000000 ab-test-simulator-0.0.2/ab_test_simulator.egg-info/top_level.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     1054 2023-06-01 11:20:27.000000 ab-test-simulator-0.0.2/settings.ini
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       38 2023-06-01 11:42:54.667128 ab-test-simulator-0.0.2/setup.cfg
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     2711 2023-06-01 06:53:26.000000 ab-test-simulator-0.0.2/setup.py
```

### Comparing `ab-test-simulator-0.0.1/LICENSE` & `ab-test-simulator-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ab-test-simulator-0.0.1/ab_test_simulator/_modidx.py` & `ab-test-simulator-0.0.2/ab_test_simulator/_modidx.py`

 * *Files identical despite different names*

### Comparing `ab-test-simulator-0.0.1/ab_test_simulator/generator.py` & `ab-test-simulator-0.0.2/ab_test_simulator/generator.py`

 * *Files identical despite different names*

### Comparing `ab-test-simulator-0.0.1/ab_test_simulator/power.py` & `ab-test-simulator-0.0.2/ab_test_simulator/power.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,25 +57,23 @@
     if one_sided == True:
         alternative = "greater"
         alternative_z = "larger"
         print("One sided.")
     else:
         alternative = "two-sided"
         print("Two sided tests, except for bayesian which is one sided.")
-    approaches = ["fisher", "chi", "z", "bayes"]
+    approaches = ["fisher", "z", "bayes"]
     pvs = dict()
     pvs_fisher = dict()
     pvs_z = dict()
-    pvs_chi = dict()
     # run simulations for each sample size
     for idx, size in enumerate(sizes):
         pvs[idx] = []
         pvs_fisher[idx] = []
         pvs_z[idx] = []
-        pvs_chi[idx] = []
         for realization in range(0, realizations):
             df_binary = generate_binary_data(N=size, cr0=cr0, cr1=cr1)
             df_contingency = data_to_contingency(df_binary)
             test = BinaryDataTest()
             for group in [0, 1]:
                 nUser = df_contingency.loc[group].users
                 nConverted = df_contingency.loc[group].converted
@@ -94,24 +92,17 @@
                     df_contingency.loc[1].converted,
                     df_contingency.loc[0].converted,
                 ],
                 nobs=size,
                 alternative=alternative_z,
             )
             pvs_z[idx].append(p_z)
-            p_chi = chi2_contingency(
-                np.array(df_contingency[["not_converted", "converted"]])
-            ).pvalue
-            if one_sided == True:
-                p_chi = p_chi / 2.0
-            pvs_chi[idx].append(p_chi)
         print(f"{idx} done")
     pvalues_results = {
         "fisher": pvs_fisher,
-        "chi": pvs_chi,
         "bayes": pvs,
         "z": pvs_z,
     }
     # compute power lines
     power_lines = dict()
     power_lines["bayes"] = [
         (np.array(pvalues_results["bayes"][i]) > 1.0 - alpha).sum()
```

### Comparing `ab-test-simulator-0.0.1/settings.ini` & `ab-test-simulator-0.0.2/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = ab-test-simulator
 lib_name = %(repo)s
-version = 0.0.1
+version = 0.0.2
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = ab_test_simulator
```

### Comparing `ab-test-simulator-0.0.1/setup.py` & `ab-test-simulator-0.0.2/setup.py`

 * *Files identical despite different names*

