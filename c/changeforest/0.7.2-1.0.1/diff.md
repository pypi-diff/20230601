# Comparing `tmp/changeforest-0.7.2.tar.gz` & `tmp/changeforest-1.0.1.tar.gz`

## Comparing `changeforest-0.7.2.tar` & `changeforest-1.0.1.tar`

### file list

```diff
@@ -1,49 +1,50 @@
--rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 changeforest-0.7.2/local_dependencies/changeforest/Cargo.toml
--rw-r--r--   0     1001      121     4928 2022-05-09 17:31:32.000000 changeforest-0.7.2/local_dependencies/changeforest/CHANGELOG.md
--rw-r--r--   0     1001      121     1506 2022-05-09 17:31:32.000000 changeforest-0.7.2/local_dependencies/changeforest/LICENSE
--rw-r--r--   0     1001      121    10675 2022-05-09 17:31:32.000000 changeforest-0.7.2/local_dependencies/changeforest/README.md
--rw-r--r--   0     1001      121    44042 2022-05-09 17:31:32.000000 changeforest-0.7.2/local_dependencies/changeforest/docs/py_cic_rf_binary_segmentation_result_plot.png
--rw-r--r--   0     1001      121   103070 2022-05-09 17:31:32.000000 changeforest-0.7.2/local_dependencies/changeforest/docs/py_cic_rf_optimizer_result_plot.png
--rw-r--r--   0     1001      121    57577 2022-05-09 17:31:32.000000 changeforest-0.7.2/local_dependencies/changeforest/docs/r_cic_rf_binary_segmentation_result_plot.png
--rw-r--r--   0     1001      121   164340 2022-05-09 17:31:32.000000 changeforest-0.7.2/local_dependencies/changeforest/docs/r_cic_rf_optimizer_result_plot.png
--rw-r--r--   0     1001      121     7089 2022-05-09 17:31:32.000000 changeforest-0.7.2/local_dependencies/changeforest/src/binary_segmentation.rs
--rw-r--r--   0     1001      121     3213 2022-05-09 17:31:32.000000 changeforest-0.7.2/local_dependencies/changeforest/src/classifier/classifier.rs
--rw-r--r--   0     1001      121     6140 2022-05-09 17:31:32.000000 changeforest-0.7.2/local_dependencies/changeforest/src/classifier/knn.rs
--rw-r--r--   0     1001      121      132 2022-05-09 17:31:32.000000 changeforest-0.7.2/local_dependencies/changeforest/src/classifier/mod.rs
--rw-r--r--   0     1001      121     3489 2022-05-09 17:31:32.000000 changeforest-0.7.2/local_dependencies/changeforest/src/classifier/random_forest.rs
--rw-r--r--   0     1001      121     4355 2022-05-09 17:31:32.000000 changeforest-0.7.2/local_dependencies/changeforest/src/control.rs
--rw-r--r--   0     1001      121     5942 2022-05-09 17:31:32.000000 changeforest-0.7.2/local_dependencies/changeforest/src/fmt.rs
--rw-r--r--   0     1001      121     3918 2022-05-09 17:31:32.000000 changeforest-0.7.2/local_dependencies/changeforest/src/gain/change_in_mean.rs
--rw-r--r--   0     1001      121     7756 2022-05-09 17:31:32.000000 changeforest-0.7.2/local_dependencies/changeforest/src/gain/classifier_gain.rs
--rw-r--r--   0     1001      121     4067 2022-05-09 17:31:32.000000 changeforest-0.7.2/local_dependencies/changeforest/src/gain/gain.rs
--rw-r--r--   0     1001      121     3213 2022-05-09 17:31:32.000000 changeforest-0.7.2/local_dependencies/changeforest/src/gain/gain_result.rs
--rw-r--r--   0     1001      121      276 2022-05-09 17:31:32.000000 changeforest-0.7.2/local_dependencies/changeforest/src/gain/mod.rs
--rw-r--r--   0     1001      121      675 2022-05-09 17:31:32.000000 changeforest-0.7.2/local_dependencies/changeforest/src/lib.rs
--rw-r--r--   0     1001      121      927 2022-05-09 17:31:32.000000 changeforest-0.7.2/local_dependencies/changeforest/src/model_selection_result.rs
--rw-r--r--   0     1001      121     2421 2022-05-09 17:31:32.000000 changeforest-0.7.2/local_dependencies/changeforest/src/optimizer/grid_search.rs
--rw-r--r--   0     1001      121      223 2022-05-09 17:31:32.000000 changeforest-0.7.2/local_dependencies/changeforest/src/optimizer/mod.rs
--rw-r--r--   0     1001      121     1140 2022-05-09 17:31:32.000000 changeforest-0.7.2/local_dependencies/changeforest/src/optimizer/optimizer.rs
--rw-r--r--   0     1001      121      660 2022-05-09 17:31:32.000000 changeforest-0.7.2/local_dependencies/changeforest/src/optimizer/optimizer_result.rs
--rw-r--r--   0     1001      121     4938 2022-05-09 17:31:32.000000 changeforest-0.7.2/local_dependencies/changeforest/src/optimizer/two_step_search.rs
--rw-r--r--   0     1001      121     8360 2022-05-09 17:31:32.000000 changeforest-0.7.2/local_dependencies/changeforest/src/segmentation.rs
--rw-r--r--   0     1001      121     8543 2022-05-09 17:31:32.000000 changeforest-0.7.2/local_dependencies/changeforest/src/testing.rs
--rw-r--r--   0     1001      121      387 2022-05-09 17:31:32.000000 changeforest-0.7.2/local_dependencies/changeforest/src/utils.rs
--rw-r--r--   0     1001      121     3162 2022-05-09 17:31:32.000000 changeforest-0.7.2/local_dependencies/changeforest/src/wrapper.rs
--rw-r--r--   0     1001      121     1792 2022-05-09 17:31:32.000000 changeforest-0.7.2/local_dependencies/changeforest/tests/test_integration.rs
--rw-r--r--   0        0        0      362 1970-01-01 00:00:00.000000 changeforest-0.7.2/Cargo.toml
--rw-r--r--   0     1001      121       35 2022-05-09 17:31:32.000000 changeforest-0.7.2/.gitignore
--rw-r--r--   0     1001      121     1506 2022-05-09 17:31:32.000000 changeforest-0.7.2/LICENSE
--rw-r--r--   0     1001      121     5621 2022-05-09 17:31:32.000000 changeforest-0.7.2/README.md
--rw-r--r--   0     1001      121      218 2022-05-09 17:31:32.000000 changeforest-0.7.2/changeforest/__init__.py
--rw-r--r--   0     1001      121     1780 2022-05-09 17:31:32.000000 changeforest-0.7.2/changeforest/control.py
--rw-r--r--   0     1001      121     6048 2022-05-09 17:31:32.000000 changeforest-0.7.2/changeforest/plotting.py
--rw-r--r--   0     1001      121      147 2022-05-09 17:31:32.000000 changeforest-0.7.2/environment.yml
--rw-r--r--   0     1001      121     2023 2022-05-09 17:31:32.000000 changeforest-0.7.2/pyproject.toml
--rw-r--r--   0     1001      121     5039 2022-05-09 17:31:32.000000 changeforest-0.7.2/src/control.rs
--rw-r--r--   0     1001      121     1180 2022-05-09 17:31:32.000000 changeforest-0.7.2/src/lib.rs
--rw-r--r--   0     1001      121     5789 2022-05-09 17:31:32.000000 changeforest-0.7.2/src/result.rs
--rw-r--r--   0     1001      121     1270 2022-05-09 17:31:32.000000 changeforest-0.7.2/tests/conftest.py
--rw-r--r--   0     1001      121      987 2022-05-09 17:31:32.000000 changeforest-0.7.2/tests/test_changeforest.py
--rw-r--r--   0     1001      121     4502 2022-05-09 17:31:32.000000 changeforest-0.7.2/tests/test_control.py
--rw-r--r--   0     1001      121      903 2022-05-09 17:31:32.000000 changeforest-0.7.2/tests/test_plotting.py
--rw-r--r--   0        0        0     6018 1970-01-01 00:00:00.000000 changeforest-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 changeforest-1.0.1/local_dependencies/changeforest/Cargo.toml
+-rw-r--r--   0     1001      123     5182 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/CHANGELOG.md
+-rw-r--r--   0     1001      123     1506 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/LICENSE
+-rw-r--r--   0     1001      123    10533 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/README.md
+-rw-r--r--   0     1001      123    44744 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/docs/py_cic_rf_binary_segmentation_result_plot.png
+-rw-r--r--   0     1001      123    85452 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/docs/py_cic_rf_optimizer_result_plot.png
+-rw-r--r--   0     1001      123    57577 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/docs/r_cic_rf_binary_segmentation_result_plot.png
+-rw-r--r--   0     1001      123   164340 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/docs/r_cic_rf_optimizer_result_plot.png
+-rw-r--r--   0     1001      123     7089 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/binary_segmentation.rs
+-rw-r--r--   0     1001      123     3213 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/classifier/classifier.rs
+-rw-r--r--   0     1001      123     6140 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/classifier/knn.rs
+-rw-r--r--   0     1001      123      132 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/classifier/mod.rs
+-rw-r--r--   0     1001      123     3489 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/classifier/random_forest.rs
+-rw-r--r--   0     1001      123     4379 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/control.rs
+-rw-r--r--   0     1001      123     5940 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/fmt.rs
+-rw-r--r--   0     1001      123     3918 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/gain/change_in_mean.rs
+-rw-r--r--   0     1001      123     7755 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/gain/classifier_gain.rs
+-rw-r--r--   0     1001      123     4067 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/gain/gain.rs
+-rw-r--r--   0     1001      123     3213 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/gain/gain_result.rs
+-rw-r--r--   0     1001      123      276 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/gain/mod.rs
+-rw-r--r--   0     1001      123      675 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/lib.rs
+-rw-r--r--   0     1001      123      927 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/model_selection_result.rs
+-rw-r--r--   0     1001      123     2421 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/optimizer/grid_search.rs
+-rw-r--r--   0     1001      123      223 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/optimizer/mod.rs
+-rw-r--r--   0     1001      123     1140 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/optimizer/optimizer.rs
+-rw-r--r--   0     1001      123      660 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/optimizer/optimizer_result.rs
+-rw-r--r--   0     1001      123     4938 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/optimizer/two_step_search.rs
+-rw-r--r--   0     1001      123     8349 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/segmentation.rs
+-rw-r--r--   0     1001      123     8543 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/testing.rs
+-rw-r--r--   0     1001      123      387 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/utils.rs
+-rw-r--r--   0     1001      123     3127 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/wrapper.rs
+-rw-r--r--   0     1001      123     1792 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/tests/test_integration.rs
+-rw-r--r--   0        0        0      362 1970-01-01 00:00:00.000000 changeforest-1.0.1/Cargo.toml
+-rw-r--r--   0     1001      123       35 2023-06-01 09:03:02.000000 changeforest-1.0.1/.gitignore
+-rw-r--r--   0     1001      123     1506 2023-06-01 09:03:02.000000 changeforest-1.0.1/LICENSE
+-rw-r--r--   0     1001      123     5416 2023-06-01 09:03:02.000000 changeforest-1.0.1/README.md
+-rw-r--r--   0     1001      123      218 2023-06-01 09:03:02.000000 changeforest-1.0.1/changeforest/__init__.py
+-rw-r--r--   0     1001      123     1780 2023-06-01 09:03:02.000000 changeforest-1.0.1/changeforest/control.py
+-rw-r--r--   0     1001      123     6047 2023-06-01 09:03:02.000000 changeforest-1.0.1/changeforest/plotting.py
+-rw-r--r--   0     1001      123      147 2023-06-01 09:03:02.000000 changeforest-1.0.1/environment.yml
+-rw-r--r--   0     1001      123     1838 2023-06-01 09:03:02.000000 changeforest-1.0.1/pyproject.toml
+-rw-r--r--   0     1001      123     5039 2023-06-01 09:03:02.000000 changeforest-1.0.1/src/control.rs
+-rw-r--r--   0     1001      123     1180 2023-06-01 09:03:02.000000 changeforest-1.0.1/src/lib.rs
+-rw-r--r--   0     1001      123     5789 2023-06-01 09:03:02.000000 changeforest-1.0.1/src/result.rs
+-rw-r--r--   0     1001      123     1270 2023-06-01 09:03:02.000000 changeforest-1.0.1/tests/conftest.py
+-rw-r--r--   0     1001      123      987 2023-06-01 09:03:02.000000 changeforest-1.0.1/tests/test_changeforest.py
+-rw-r--r--   0     1001      123     4502 2023-06-01 09:03:02.000000 changeforest-1.0.1/tests/test_control.py
+-rw-r--r--   0     1001      123      903 2023-06-01 09:03:02.000000 changeforest-1.0.1/tests/test_plotting.py
+-rw-r--r--   0     1001      123    13024 2023-06-01 09:04:42.000000 changeforest-1.0.1/Cargo.lock
+-rw-r--r--   0        0        0     5800 1970-01-01 00:00:00.000000 changeforest-1.0.1/PKG-INFO
```

### Comparing `changeforest-0.7.2/local_dependencies/changeforest/CHANGELOG.md` & `changeforest-1.0.1/local_dependencies/changeforest/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 
 # Changelog
 
+## 1.0.1 - (2022-06-01)
+
+**Bug fixes:**
+
+- Python macos images are now again correctly built on GitHub runners.
+
+## 1.0.0 - (2022-05-30)
+
+First major release. There have been no changes since the last release. The manuscript is to be published in JMLR.
+
 ## 0.7.2 - (2022-05-09)
 
 **Bug fixes:**
 
 - Fixed bugs when plotting results created with `method="change_in_mean"` or `segmentation="sbs"` or `"wbs"` (Python).
 
 ## 0.7.1 - (2022-05-02)
@@ -134,15 +144,15 @@
 **New features:**
 
 - The `TwoStepSearch` now uses three initial guesses, the 0.25, 0.5 and 0.75 quantiles
   of the segment, for the first step. The the best split corresponding to the highest
   maximal gain from the three guesses is used in the second step. The permutation test
   used for model selection has also been adjusted to be consistent (#65).
 
-  This increases estimation performance for classifier based methods, especially if used
+  This increases estimation performance for classifier-based methods, especially if used
   with standard binary segmentation, i.e. for `changeforst_bs` and `changeforest_knn`.
 
 ## 0.1.1 - (2021-11-25)
 
 **Other changes:**
 
 - Added license file for compatability with conda-forge.
```

### Comparing `changeforest-0.7.2/local_dependencies/changeforest/LICENSE` & `changeforest-1.0.1/local_dependencies/changeforest/LICENSE`

 * *Files identical despite different names*

### Comparing `changeforest-0.7.2/local_dependencies/changeforest/README.md` & `changeforest-1.0.1/local_dependencies/changeforest/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 distribution of a time series. Existing methods either assume a parametric model for
 within-segment distributions or are based on ranks or distances and thus fail in
 scenarios with a reasonably large dimensionality.
 
 `changeforest` implements a classifier-based algorithm that consistently estimates
 change points without any parametric assumptions, even in high-dimensional scenarios.
 It uses the out-of-bag probability predictions of a random forest to construct a
-pseudo-log-likelihood that gets optimized using a computationally feasible two-step
+classifier log-likelihood ratio that gets optimized using a computationally feasible two-step
 method.
 
 See [1] for details.
 
 `changeforest` is available as rust crate, a Python package (on
 [`PyPI`](https://pypi.org/project/changeforest/) and
 [`conda-forge`](https://anaconda.org/conda-forge/changeforest)),
@@ -44,64 +44,64 @@
    ...: Sigma = np.full((5, 5), 0.7)
    ...: np.fill_diagonal(Sigma, 1)
    ...: 
    ...: rng = np.random.default_rng(12)
    ...: X = np.concatenate(
    ...:     (
    ...:         rng.normal(0, 1, (200, 5)),
-   ...:         rng.multivariate_normal(np.zeros(5), Sigma, 200),
+   ...:         rng.multivariate_normal(np.zeros(5), Sigma, 200, method="cholesky"),
    ...:         rng.normal(0, 1, (200, 5)),
    ...:     ),
    ...:     axis=0,
    ...: )
 ```
 
 The simulated dataset `X` coincides with the _change in covariance_ (CIC) setup
-described in [1]. Observations in the first and last segment are independently drawn
+described in [1]. Observations in the first and last segments are independently drawn
 from a standard multivariate Gaussian distribution. Observations in the second segment
 are i.i.d. normal with mean zero and unit variance, but with a covariance of ρ = 0.7
 between coordinates. This is a challenging scenario.
 
 ```python
 In [2]: from changeforest import changeforest
    ...: 
    ...: result = changeforest(X, "random_forest", "bs")
    ...: result
 Out[2]: 
                     best_split max_gain p_value
-(0, 600]                   412   19.603   0.005
- ¦--(0, 412]               201   62.981   0.005
- ¦   ¦--(0, 201]           194  -12.951    0.76
- ¦   °--(201, 412]         211   -9.211   0.545
- °--(412, 600]             418  -37.519   0.915
+(0, 600]                   400   14.814   0.005
+ ¦--(0, 400]               200   59.314   0.005
+ ¦   ¦--(0, 200]             6    -1.95    0.67
+ ¦   °--(200, 400]         393   -8.668    0.81
+ °--(400, 600]             412   -9.047    0.66
 
 In [3]: result.split_points()
-Out[3]: [201, 412]
+Out[3]: [200, 400]
 ```
 
-`changeforest` correctly identifies the change point around `t=200` but is slightly
-off at `t=412`. The `changeforest` function returns a `BinarySegmentationResult`.
-We use its `plot` method to investigate the gain curves maximized by the change point estimates:
+`changeforest` correctly identifies the change points at `t=200` and `t=400`. The
+`changeforest` function returns a `BinarySegmentationResult`. We use its `plot` method
+to investigate the gain curves maximized by the change point estimates:
 
-```
+```python
 In [4]: result.plot().show()
 ```
 <p align="center">
   <img src="docs/py_cic_rf_binary_segmentation_result_plot.png" />
 </p>
 Change point estimates are marked in red.
 
 For `method="random_forest"` and `method="knn"`, the `changeforest` algorithm uses a two-step approach to
 find an optimizer of the gain. This fits a classifier for three split candidates
 at the segment's 1/4, 1/2 and 3/4 quantiles, computes approximate gain curves using
-the resulting pseudo-log-likelihoods and selects the overall optimizer as a second guess.
+the resulting classifier log-likelihood ratios and selects the overall optimizer as a second guess.
 We can investigate the gain curves from the optimizer using the `plot` method of `OptimizerResult`.
 The initial guesses are marked in blue.
 
-```
+```python
 In [5]: result.optimizer_result.plot().show()
 ```
 <p align="center">
   <img src="docs/py_cic_rf_optimizer_result_plot.png" />
 </p>
  
 One can observe that the approximate gain curves are piecewise linear, with maxima
@@ -112,53 +112,50 @@
 These can be interesting to investigate the output of the algorithm further.
 
 The `changeforest` algorithm can be tuned with hyperparameters. See
 [here](https://github.com/mlondschien/changeforest/blob/287ac0f10728518d6a00bf698a4d5834ae98715d/src/control.rs#L3-L30)
 for their descriptions and default values. In Python, the parameters can
 be specified with the [`Control` class](https://github.com/mlondschien/changeforest/blob/b33533fe0ddf64c1ea60d0d2203e55b117811667/changeforest-py/changeforest/control.py#L1-L26),
 which can be passed to `changeforest`. The following will build random forests with
-20 trees:
+50 trees:
 
 ```python
 In [6]: from changeforest import Control
-   ...: changeforest(X, "random_forest", "bs", Control(random_forest_n_estimators=20))
+   ...: changeforest(X, "random_forest", "bs", Control(random_forest_n_estimators=50))
 Out[6]: 
-                            best_split max_gain p_value
-(0, 600]                           592  -11.786    0.01
- ¦--(0, 592]                       121    -6.26   0.015
- ¦   ¦--(0, 121]                    13  -14.219   0.615
- ¦   °--(121, 592]                 416   21.272   0.005
- ¦       ¦--(121, 416]             201   37.157   0.005
- ¦       ¦   ¦--(121, 201]         192   -17.54    0.65
- ¦       ¦   °--(201, 416]         207   -6.701    0.74
- ¦       °--(416, 592]             584  -44.054   0.935
- °--(592, 600]     
+                    best_split max_gain p_value
+(0, 600]                   416    7.463    0.01
+ ¦--(0, 416]               200   43.935   0.005
+ ¦   ¦--(0, 200]           193  -14.993   0.945
+ ¦   °--(200, 416]         217    -9.13   0.085
+ °--(416, 600]             591   -12.07       1 
 ```
 
-The `changeforest` algorithm still detects change points around `t=200, 400` but also
-returns two false positives.
+The `changeforest` algorithm still detects change points at `t=200`, but is slightly off
+with `t=416`.
 
 Due to the nature of the change, `method="change_in_mean"` is unable to detect any
 change points at all:
 ```python
 In [7]: changeforest(X, "change_in_mean", "bs")
 Out[7]: 
           best_split max_gain p_value
-(0, 600]         589    8.318 
+(0, 600]         589    8.625  
 ```
 
 ## R
 
 To install from `conda-forge`, run
 
 ```bash
 conda install -c conda-forge r-changeforest
 ```
 
-See [here](https://github.com/conda-forge/miniforge) for instructions on how to install `conda`.
+See [here](changeforest-r/Installing_R_packages_with_conda.md) for a detailed description
+on installing the `changeforest` R package with `conda`.
 
 ### Example
 
 In the following example, we perform random forest-based change point detection on
 a simulated dataset with `n=600` observations and covariance shifts at `t=200, 400`.
 
 ```R
@@ -172,15 +169,15 @@
     mvrnorm(n=200, mu=mu, Sigma=diag(5)),
     mvrnorm(n=200, mu=mu, Sigma=Sigma),
     mvrnorm(n=200, mu=mu, Sigma=diag(5))
 )
 ```
 
 The simulated dataset `X` coincides with the _change in covariance_ (CIC) setup
-described in [1]. Observations in the first and last segment are independently drawn
+described in [1]. Observations in the first and last segments are independently drawn
 from a standard multivariate Gaussian distribution. Observations in the second segment
 are i.i.d. normal with mean zero and unit variance, but with a covariance of ρ = 0.7
 between coordinates. This is a challenging scenario.
 
 
 ```R
 > library(changeforest)
@@ -198,31 +195,31 @@
 [1] 199 410
 ```
 
 `changeforest` correctly identifies the change point around `t=200` but is slightly
 off at `t=410`. The `changeforest` function returns an object of class `binary_segmentation_result`.
 We use its `plot` method to investigate the gain curves maximized by the change point estimates:
 
-```
+```R
 > plot(result)
 ```
 <p align="center">
   <img src="docs/r_cic_rf_binary_segmentation_result_plot.png" />
 </p>
 
 Change point estimates are marked in red.
 
 For `method="random_forest"` and `method="knn"`, the `changeforest` algorithm uses a two-step approach to
 find an optimizer of the gain. This fits a classifier for three split candidates
 at the segment's 1/4, 1/2 and 3/4 quantiles  computes approximate gain curves using
-the resulting pseudo-log-likelihoods and selects the overall optimizer as a second guess.
+the resulting classifier log-likelihood ratios and selects the overall optimizer as a second guess.
 We can investigate the gain curves from the optimizer using the `plot` method of `optimizer_result`.
 The initial guesses are marked in blue.
 
-```
+```R
 > plot(result$optimizer_result)
 ```
 <p align="center">
   <img src="docs/r_cic_rf_optimizer_result_plot.png" />
 </p>
  
 One can observe that the approximate gain curves are piecewise linear, with maxima
@@ -263,8 +260,8 @@
       name best_split max_gain p_value is_significant
 1 (0, 600]        498 17.29389      NA          FALSE
 ```
 
 
 ## References
 
-[1] M. Londschien, S. Kovács and P. Bühlmann (2022), "Random Forests for Change Point Detection", working paper.
+[1] M. Londschien, P. Bühlmann and S. Kovács (2023). "Random Forests for Change Point Detection" Journal of Machine Learning Research
```

### Comparing `changeforest-0.7.2/local_dependencies/changeforest/docs/r_cic_rf_binary_segmentation_result_plot.png` & `changeforest-1.0.1/local_dependencies/changeforest/docs/r_cic_rf_binary_segmentation_result_plot.png`

 * *Files identical despite different names*

### Comparing `changeforest-0.7.2/local_dependencies/changeforest/docs/r_cic_rf_optimizer_result_plot.png` & `changeforest-1.0.1/local_dependencies/changeforest/docs/r_cic_rf_optimizer_result_plot.png`

 * *Files identical despite different names*

### Comparing `changeforest-0.7.2/local_dependencies/changeforest/src/binary_segmentation.rs` & `changeforest-1.0.1/local_dependencies/changeforest/src/binary_segmentation.rs`

 * *Files identical despite different names*

### Comparing `changeforest-0.7.2/local_dependencies/changeforest/src/classifier/classifier.rs` & `changeforest-1.0.1/local_dependencies/changeforest/src/classifier/classifier.rs`

 * *Files identical despite different names*

### Comparing `changeforest-0.7.2/local_dependencies/changeforest/src/classifier/knn.rs` & `changeforest-1.0.1/local_dependencies/changeforest/src/classifier/knn.rs`

 * *Files identical despite different names*

### Comparing `changeforest-0.7.2/local_dependencies/changeforest/src/classifier/random_forest.rs` & `changeforest-1.0.1/local_dependencies/changeforest/src/classifier/random_forest.rs`

 * *Files identical despite different names*

### Comparing `changeforest-0.7.2/local_dependencies/changeforest/src/control.rs` & `changeforest-1.0.1/local_dependencies/changeforest/src/control.rs`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     /// not be split.
     pub minimal_relative_segment_length: f64,
     /// Only keep split point if the gain exceeds `minimal_gain_to_split`. Relevant for
     /// change in mean. Note that this is relative to the number of observations.
     /// Use value motivated by BIC `minimal_gain_to_split = log(n_samples) * n_features / n_samples`
     /// if `None`.
     pub minimal_gain_to_split: Option<f64>,
-    /// Type two error in model selection to be approximated. Relevant for classifier
+    /// Type two error in model selection to be approximated. Relevant for classifier-
     /// based changepoint detection.
     pub model_selection_alpha: f64,
     /// Number of permutations for model selection in classifier-based change point
     /// detection.
     pub model_selection_n_permutations: usize,
     /// Number of randomly drawn segments. Corresponds to parameter `M` in
     /// https://arxiv.org/pdf/1411.0858.pdf.
@@ -27,14 +27,15 @@
     /// Seed used for segmentation.
     pub seed: u64,
     /// Hyperparameters for random forests.
     pub random_forest_parameters: RandomForestParameters,
 }
 
 impl Control {
+    #[allow(clippy::should_implement_trait)]
     pub fn default() -> Control {
         Control {
             minimal_relative_segment_length: 0.01,
             minimal_gain_to_split: None,
             model_selection_alpha: 0.02,
             model_selection_n_permutations: 199,
             number_of_wild_segments: 100,
@@ -49,32 +50,30 @@
 
     pub fn with_minimal_relative_segment_length(
         mut self,
         minimal_relative_segment_length: f64,
     ) -> Self {
         if (minimal_relative_segment_length >= 0.5) | (minimal_relative_segment_length <= 0.) {
             panic!(
-                "minimal_relative_segment_length needs to be strictly between 0 and 0.5 Got {}",
-                minimal_relative_segment_length
+                "minimal_relative_segment_length needs to be strictly between 0 and 0.5 Got {minimal_relative_segment_length}"
             );
         }
         self.minimal_relative_segment_length = minimal_relative_segment_length;
         self
     }
 
     pub fn with_minimal_gain_to_split(mut self, minimal_gain_to_split: Option<f64>) -> Self {
         self.minimal_gain_to_split = minimal_gain_to_split;
         self
     }
 
     pub fn with_model_selection_alpha(mut self, model_selection_alpha: f64) -> Self {
         if (model_selection_alpha >= 1.) | (model_selection_alpha <= 0.) {
             panic!(
-                "model_selection_alpha needs to be strictly between 0 and 1. Got {}",
-                model_selection_alpha
+                "model_selection_alpha needs to be strictly between 0 and 1. Got {model_selection_alpha}"                
             );
         }
         self.model_selection_alpha = model_selection_alpha;
         self
     }
 
     pub fn with_model_selection_n_permutations(
@@ -89,16 +88,15 @@
         self.number_of_wild_segments = number_of_wild_segments;
         self
     }
 
     pub fn with_seeded_segments_alpha(mut self, seeded_segments_alpha: f64) -> Self {
         if (1. <= seeded_segments_alpha) | (seeded_segments_alpha <= 0.) {
             panic!(
-                "seeded_segments_alpha needs to be strictly between 0 and 1. Got {}",
-                seeded_segments_alpha
+                "seeded_segments_alpha needs to be strictly between 0 and 1. Got {seeded_segments_alpha}"                
             );
         }
         self.seeded_segments_alpha = seeded_segments_alpha;
         self
     }
 
     pub fn with_seed(mut self, seed: u64) -> Self {
```

### Comparing `changeforest-0.7.2/local_dependencies/changeforest/src/fmt.rs` & `changeforest-1.0.1/local_dependencies/changeforest/src/fmt.rs`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 }
 
 fn _display_option<T>(option: &Option<T>) -> String
 where
     T: Display,
 {
     if let Some(val) = option {
-        format!("{}", val)
+        format!("{val}")
     } else {
         "".to_string()
     }
 }
 
 fn _format_tree(result: &BinarySegmentationResult) -> Vec<Vec<String>> {
     let mut output = vec![vec![
```

### Comparing `changeforest-0.7.2/local_dependencies/changeforest/src/gain/change_in_mean.rs` & `changeforest-1.0.1/local_dependencies/changeforest/src/gain/change_in_mean.rs`

 * *Files identical despite different names*

### Comparing `changeforest-0.7.2/local_dependencies/changeforest/src/gain/classifier_gain.rs` & `changeforest-1.0.1/local_dependencies/changeforest/src/gain/classifier_gain.rs`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     T: Classifier,
 {
     /// Total number of observations.
     fn n(&self) -> usize {
         self.classifier.n()
     }
 
-    /// Return classifier-likelihood based gain when splitting segment `[start, stop)`
+    /// Return classifier log-likelihood ratio when splitting segment `[start, stop)`
     /// at `split`.
     fn gain(&self, start: usize, stop: usize, split: usize) -> f64 {
         let predictions = self.classifier.predict(start, stop, split);
         self.classifier
             .single_likelihood(&predictions, start, stop, split)
     }
 
@@ -119,15 +119,15 @@
     }
 }
 
 impl<T> ApproxGain for ClassifierGain<T>
 where
     T: Classifier,
 {
-    /// Return an approximation of the classifier-likelihood based gain when splitting
+    /// Return an approximation of the classifier log- likelihood ratio when splitting
     /// segment `[start, stop)` for each split in `split_candidates`.
     ///
     /// A single fit is generated with a split at `guess`.
     fn gain_approx(
         &self,
         start: usize,
         stop: usize,
```

### Comparing `changeforest-0.7.2/local_dependencies/changeforest/src/gain/gain.rs` & `changeforest-1.0.1/local_dependencies/changeforest/src/gain/gain.rs`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 pub trait ApproxGain {
     #[allow(unused_variables)]
     /// An approximation of the gain when splitting segment `[start, stop)` at points in `split_candidates`.
     ///
     /// Returns an `ndarray::Array1` of length `stop - start`. Entries without
     /// corresponding entry in `split_candidates` are `f64::NAN`.
     ///
-    /// This can be useful when combining classifier based gains and the two-step-search
+    /// This can be useful when combining classifier-based gains and the two-step-search
     /// optimizer.
     fn gain_approx(
         &self,
         start: usize,
         stop: usize,
         guess: usize,
         split_points: &[usize],
```

### Comparing `changeforest-0.7.2/local_dependencies/changeforest/src/gain/gain_result.rs` & `changeforest-1.0.1/local_dependencies/changeforest/src/gain/gain_result.rs`

 * *Files identical despite different names*

### Comparing `changeforest-0.7.2/local_dependencies/changeforest/src/lib.rs` & `changeforest-1.0.1/local_dependencies/changeforest/src/lib.rs`

 * *Files identical despite different names*

### Comparing `changeforest-0.7.2/local_dependencies/changeforest/src/model_selection_result.rs` & `changeforest-1.0.1/local_dependencies/changeforest/src/model_selection_result.rs`

 * *Files identical despite different names*

### Comparing `changeforest-0.7.2/local_dependencies/changeforest/src/optimizer/grid_search.rs` & `changeforest-1.0.1/local_dependencies/changeforest/src/optimizer/grid_search.rs`

 * *Files identical despite different names*

### Comparing `changeforest-0.7.2/local_dependencies/changeforest/src/optimizer/optimizer.rs` & `changeforest-1.0.1/local_dependencies/changeforest/src/optimizer/optimizer.rs`

 * *Files identical despite different names*

### Comparing `changeforest-0.7.2/local_dependencies/changeforest/src/optimizer/optimizer_result.rs` & `changeforest-1.0.1/local_dependencies/changeforest/src/optimizer/optimizer_result.rs`

 * *Files identical despite different names*

### Comparing `changeforest-0.7.2/local_dependencies/changeforest/src/optimizer/two_step_search.rs` & `changeforest-1.0.1/local_dependencies/changeforest/src/optimizer/two_step_search.rs`

 * *Files identical despite different names*

### Comparing `changeforest-0.7.2/local_dependencies/changeforest/src/segmentation.rs` & `changeforest-1.0.1/local_dependencies/changeforest/src/segmentation.rs`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
                 let mut stop: usize;
                 for k in 1..(n_layers as i32) {
                     alpha_k = optimizer.control().seeded_segments_alpha.powi(k); // (1/alpha)^(k-1)
                     segment_length = (optimizer.n() as f64) * alpha_k; // l_k
                     n_segments = 2 * ((1. / alpha_k) as f32).ceil() as usize - 1; // n_k
                     segment_step =
                         (optimizer.n() as f64 - segment_length) / (n_segments - 1) as f64; // s_k
-                    for segment_id in 0..(n_segments as usize) {
+                    for segment_id in 0..n_segments {
                         start = ((segment_id as f64 * segment_step) as f32) as usize;
                         // start + segment_length > n through floating point errors in
                         // n_segments, e.g. for n = 20'000, alpha_k = 1/sqrt(2), k=6
                         stop = (start + (segment_length as f32).ceil() as usize).min(optimizer.n());
                         segments.push(optimizer.find_best_split(start, stop).unwrap());
                     }
                 }
```

### Comparing `changeforest-0.7.2/local_dependencies/changeforest/src/testing.rs` & `changeforest-1.0.1/local_dependencies/changeforest/src/testing.rs`

 * *Files identical despite different names*

### Comparing `changeforest-0.7.2/local_dependencies/changeforest/src/wrapper.rs` & `changeforest-1.0.1/local_dependencies/changeforest/src/wrapper.rs`

 * *Files 3% similar despite different names*

```diff
@@ -45,18 +45,15 @@
         let gain = ChangeInMean::new(X, control);
         let optimizer = GridSearch { gain };
         let mut segmentation = Segmentation::new(segmentation_type_enum, &optimizer);
         tree = BinarySegmentationTree::new(X);
         tree.grow(&mut segmentation);
         BinarySegmentationResult::from_tree(tree).with_segments(segmentation)
     } else {
-        panic!(
-            "method should be one of 'knn', 'random_forest' or 'change_in_mean'. Got {}",
-            method
-        );
+        panic!("method should be one of 'knn', 'random_forest' or 'change_in_mean'. Got {method}",);
     }
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
     use crate::testing;
```

### Comparing `changeforest-0.7.2/local_dependencies/changeforest/tests/test_integration.rs` & `changeforest-1.0.1/local_dependencies/changeforest/tests/test_integration.rs`

 * *Files identical despite different names*

### Comparing `changeforest-0.7.2/LICENSE` & `changeforest-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `changeforest-0.7.2/README.md` & `changeforest-1.0.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 distribution of a time series. Existing methods either assume a parametric model for
 within-segment distributions or are based on ranks or distances and thus fail in
 scenarios with a reasonably large dimensionality.
 
 `changeforest` implements a classifier-based algorithm that consistently estimates
 change points without any parametric assumptions, even in high-dimensional scenarios.
 It uses the out-of-bag probability predictions of a random forest to construct a
-pseudo-log-likelihood that gets optimized using a computationally feasible two-step
+classifier log-likelihood ratio that gets optimized using a computationally feasible two-step
 method.
 
 See [1] for details.
 
 ## Installation
 
 To install from `conda-forge` (recommended), run
@@ -36,64 +36,64 @@
    ...: Sigma = np.full((5, 5), 0.7)
    ...: np.fill_diagonal(Sigma, 1)
    ...: 
    ...: rng = np.random.default_rng(12)
    ...: X = np.concatenate(
    ...:     (
    ...:         rng.normal(0, 1, (200, 5)),
-   ...:         rng.multivariate_normal(np.zeros(5), Sigma, 200),
+   ...:         rng.multivariate_normal(np.zeros(5), Sigma, 200, method="cholesky"),
    ...:         rng.normal(0, 1, (200, 5)),
    ...:     ),
    ...:     axis=0,
    ...: )
 ```
 
 The simulated dataset `X` coincides with the _change in covariance_ (CIC) setup
-described in [1]. Observations in the first and last segment are independently drawn
+described in [1]. Observations in the first and last segments are independently drawn
 from a standard multivariate Gaussian distribution. Observations in the second segment
 are i.i.d. normal with mean zero and unit variance, but with a covariance of ρ = 0.7
 between coordinates. This is a challenging scenario.
 
 ```python
 In [2]: from changeforest import changeforest
    ...: 
    ...: result = changeforest(X, "random_forest", "bs")
    ...: result
 Out[2]: 
                     best_split max_gain p_value
-(0, 600]                   412   19.603   0.005
- ¦--(0, 412]               201   62.981   0.005
- ¦   ¦--(0, 201]           194  -12.951    0.76
- ¦   °--(201, 412]         211   -9.211   0.545
- °--(412, 600]             418  -37.519   0.915
+(0, 600]                   400   14.814   0.005
+ ¦--(0, 400]               200   59.314   0.005
+ ¦   ¦--(0, 200]             6    -1.95    0.67
+ ¦   °--(200, 400]         393   -8.668    0.81
+ °--(400, 600]             412   -9.047    0.66
 
 In [3]: result.split_points()
-Out[3]: [201, 412]
+Out[3]: [200, 400]
 ```
 
-`changeforest` correctly identifies the change point around `t=200` but is slightly
-off at `t=412`. The `changeforest` function returns a `BinarySegmentationResult`.
-We use its `plot` method to investigate the gain curves maximized by the change point estimates:
+`changeforest` correctly identifies the change points at `t=200` and `t=400`. The
+`changeforest` function returns a `BinarySegmentationResult`. We use its `plot` method
+to investigate the gain curves maximized by the change point estimates:
 
-```
+```python
 In [4]: result.plot().show()
 ```
 <p align="center">
   <img src="../docs/py_cic_rf_binary_segmentation_result_plot.png" />
 </p>
 Change point estimates are marked in red.
 
 For `method="random_forest"` and `method="knn"`, the `changeforest` algorithm uses a two-step approach to
 find an optimizer of the gain. This fits a classifier for three split candidates
 at the segment's 1/4, 1/2 and 3/4 quantiles, computes approximate gain curves using
-the resulting pseudo-log-likelihoods and selects the overall optimizer as a second guess.
+the resulting classifier log-likelihood ratios and selects the overall optimizer as a second guess.
 We can investigate the gain curves from the optimizer using the `plot` method of `OptimizerResult`.
 The initial guesses are marked in blue.
 
-```
+```python
 In [5]: result.optimizer_result.plot().show()
 ```
 <p align="center">
   <img src="../docs/py_cic_rf_optimizer_result_plot.png" />
 </p>
  
 One can observe that the approximate gain curves are piecewise linear, with maxima
@@ -104,40 +104,36 @@
 These can be interesting to investigate the output of the algorithm further.
 
 The `changeforest` algorithm can be tuned with hyperparameters. See
 [here](https://github.com/mlondschien/changeforest/blob/287ac0f10728518d6a00bf698a4d5834ae98715d/src/control.rs#L3-L30)
 for their descriptions and default values. In Python, the parameters can
 be specified with the [`Control` class](https://github.com/mlondschien/changeforest/blob/b33533fe0ddf64c1ea60d0d2203e55b117811667/changeforest-py/changeforest/control.py#L1-L26),
 which can be passed to `changeforest`. The following will build random forests with
-20 trees:
+50 trees:
 
 ```python
 In [6]: from changeforest import Control
-   ...: changeforest(X, "random_forest", "bs", Control(random_forest_n_estimators=20))
+   ...: changeforest(X, "random_forest", "bs", Control(random_forest_n_estimators=50))
 Out[6]: 
-                            best_split max_gain p_value
-(0, 600]                           592  -11.786    0.01
- ¦--(0, 592]                       121    -6.26   0.015
- ¦   ¦--(0, 121]                    13  -14.219   0.615
- ¦   °--(121, 592]                 416   21.272   0.005
- ¦       ¦--(121, 416]             201   37.157   0.005
- ¦       ¦   ¦--(121, 201]         192   -17.54    0.65
- ¦       ¦   °--(201, 416]         207   -6.701    0.74
- ¦       °--(416, 592]             584  -44.054   0.935
- °--(592, 600]     
+                    best_split max_gain p_value
+(0, 600]                   416    7.463    0.01
+ ¦--(0, 416]               200   43.935   0.005
+ ¦   ¦--(0, 200]           193  -14.993   0.945
+ ¦   °--(200, 416]         217    -9.13   0.085
+ °--(416, 600]             591   -12.07       1 
 ```
 
-The `changeforest` algorithm still detects change points around `t=200, 400` but also
-returns two false positives.
+The `changeforest` algorithm still detects change points at `t=200`, but is slightly off
+with `t=416`.
 
 Due to the nature of the change, `method="change_in_mean"` is unable to detect any
 change points at all:
 ```python
 In [7]: changeforest(X, "change_in_mean", "bs")
 Out[7]: 
           best_split max_gain p_value
-(0, 600]         589    8.318 
+(0, 600]         589    8.625  
 ```
 
 ## References
 
-[1] M. Londschien, S. Kovács and P. Bühlmann (2022), "Random Forests for Change Point Detection", working paper.
+[1] M. Londschien, P. Bühlmann and S. Kovács (2023). "Random Forests for Change Point Detection" Journal of Machine Learning Research
```

### Comparing `changeforest-0.7.2/changeforest/control.py` & `changeforest-1.0.1/changeforest/control.py`

 * *Files identical despite different names*

### Comparing `changeforest-0.7.2/changeforest/plotting.py` & `changeforest-1.0.1/changeforest/plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,14 @@
     depth = len(gains)
 
     fig, axes = plt.subplots(nrows=depth)
     if depth == 1:
         axes = [axes]
 
     for idx in range(depth):
-
         for gain in gains[idx]:
             axes[idx].plot(gain, color="black")
 
         ymin, ymax = axes[idx].get_ylim()
         new_ymin, new_ymax = ymin - 0.05 * (ymax - ymin), ymax + 0.05 * (ymax - ymin)
 
         axes[idx].vlines(splits[idx], color="black", ymin=new_ymin, ymax=new_ymax)
```

### Comparing `changeforest-0.7.2/pyproject.toml` & `changeforest-1.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "changeforest"
-description = "Classifier based non-parametric change point detection"
+description = "Random Forests for Change Point Detection"
 readme = "README.md"
-version = "0.7.2"
+version = "1.0.1"
 requires-python = ">=3.7"
 author = "Malte Londschien <malte@londschien.ch>"
 urls = {homepage = "https://github.com/mlondschien/changeforest/"}
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python"
 ]
@@ -34,18 +34,16 @@
 # Python 3.6 build are slooow. Possibly because we also compile numpy?
 # pypi builds on macos require compilation of numpy (why?) and are thus super slow
 # fail due to https://github.com/numpy/numpy/issues/15947.
 # What is the difference between cpython and pypi builds?
 # musllinux is sloooow, >1h per build. Why?
 skip = "cp36-* pp*-macosx* pp* *-musllinux*"
 
-# Add cargobin to PATH. This is otherwise achieved by restarting the shellThis 
-# See https://github.com/pypa/pip/issues/7555 for PIP_USE_FEATURE=in-tree-build.
-# This enables relative paths, e.g. in the Cargo.toml.
-environment = { PATH="$PATH:$HOME/.cargo/bin", PIP_USE_FEATURE="in-tree-build"}
+# Add cargobin to PATH. This is otherwise achieved by restarting the shell.
+environment = { PATH="$PATH:$HOME/.cargo/bin" }
 
 [tool.cibuildwheel.linux]
 # Install rust in container before building wheels.
 before-all = "curl https://sh.rustup.rs -sSf | sh -s -- --default-toolchain stable -y && yum install -y openssl-devel"
 
 [[tool.cibuildwheel.overrides]]
 # No yum on musllinux container.
```

### Comparing `changeforest-0.7.2/src/control.rs` & `changeforest-1.0.1/src/control.rs`

 * *Files identical despite different names*

### Comparing `changeforest-0.7.2/src/lib.rs` & `changeforest-1.0.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `changeforest-0.7.2/src/result.rs` & `changeforest-1.0.1/src/result.rs`

 * *Files identical despite different names*

### Comparing `changeforest-0.7.2/tests/conftest.py` & `changeforest-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `changeforest-0.7.2/tests/test_changeforest.py` & `changeforest-1.0.1/tests/test_changeforest.py`

 * *Files identical despite different names*

### Comparing `changeforest-0.7.2/tests/test_control.py` & `changeforest-1.0.1/tests/test_control.py`

 * *Files identical despite different names*

### Comparing `changeforest-0.7.2/tests/test_plotting.py` & `changeforest-1.0.1/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `changeforest-0.7.2/PKG-INFO` & `changeforest-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: changeforest
-Version: 0.7.2
+Version: 1.0.1
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 License-File: LICENSE
-Summary: Classifier based non-parametric change point detection
+Summary: Random Forests for Change Point Detection
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: homepage, https://github.com/mlondschien/changeforest/
 
 # Random Forests for Change Point Detection
 
 Change point detection aims to identify structural breaks in the probability
 distribution of a time series. Existing methods either assume a parametric model for
 within-segment distributions or are based on ranks or distances and thus fail in
 scenarios with a reasonably large dimensionality.
 
 `changeforest` implements a classifier-based algorithm that consistently estimates
 change points without any parametric assumptions, even in high-dimensional scenarios.
 It uses the out-of-bag probability predictions of a random forest to construct a
-pseudo-log-likelihood that gets optimized using a computationally feasible two-step
+classifier log-likelihood ratio that gets optimized using a computationally feasible two-step
 method.
 
 See [1] for details.
 
 ## Installation
 
 To install from `conda-forge` (recommended), run
@@ -47,64 +47,64 @@
    ...: Sigma = np.full((5, 5), 0.7)
    ...: np.fill_diagonal(Sigma, 1)
    ...: 
    ...: rng = np.random.default_rng(12)
    ...: X = np.concatenate(
    ...:     (
    ...:         rng.normal(0, 1, (200, 5)),
-   ...:         rng.multivariate_normal(np.zeros(5), Sigma, 200),
+   ...:         rng.multivariate_normal(np.zeros(5), Sigma, 200, method="cholesky"),
    ...:         rng.normal(0, 1, (200, 5)),
    ...:     ),
    ...:     axis=0,
    ...: )
 ```
 
 The simulated dataset `X` coincides with the _change in covariance_ (CIC) setup
-described in [1]. Observations in the first and last segment are independently drawn
+described in [1]. Observations in the first and last segments are independently drawn
 from a standard multivariate Gaussian distribution. Observations in the second segment
 are i.i.d. normal with mean zero and unit variance, but with a covariance of ρ = 0.7
 between coordinates. This is a challenging scenario.
 
 ```python
 In [2]: from changeforest import changeforest
    ...: 
    ...: result = changeforest(X, "random_forest", "bs")
    ...: result
 Out[2]: 
                     best_split max_gain p_value
-(0, 600]                   412   19.603   0.005
- ¦--(0, 412]               201   62.981   0.005
- ¦   ¦--(0, 201]           194  -12.951    0.76
- ¦   °--(201, 412]         211   -9.211   0.545
- °--(412, 600]             418  -37.519   0.915
+(0, 600]                   400   14.814   0.005
+ ¦--(0, 400]               200   59.314   0.005
+ ¦   ¦--(0, 200]             6    -1.95    0.67
+ ¦   °--(200, 400]         393   -8.668    0.81
+ °--(400, 600]             412   -9.047    0.66
 
 In [3]: result.split_points()
-Out[3]: [201, 412]
+Out[3]: [200, 400]
 ```
 
-`changeforest` correctly identifies the change point around `t=200` but is slightly
-off at `t=412`. The `changeforest` function returns a `BinarySegmentationResult`.
-We use its `plot` method to investigate the gain curves maximized by the change point estimates:
+`changeforest` correctly identifies the change points at `t=200` and `t=400`. The
+`changeforest` function returns a `BinarySegmentationResult`. We use its `plot` method
+to investigate the gain curves maximized by the change point estimates:
 
-```
+```python
 In [4]: result.plot().show()
 ```
 <p align="center">
   <img src="../docs/py_cic_rf_binary_segmentation_result_plot.png" />
 </p>
 Change point estimates are marked in red.
 
 For `method="random_forest"` and `method="knn"`, the `changeforest` algorithm uses a two-step approach to
 find an optimizer of the gain. This fits a classifier for three split candidates
 at the segment's 1/4, 1/2 and 3/4 quantiles, computes approximate gain curves using
-the resulting pseudo-log-likelihoods and selects the overall optimizer as a second guess.
+the resulting classifier log-likelihood ratios and selects the overall optimizer as a second guess.
 We can investigate the gain curves from the optimizer using the `plot` method of `OptimizerResult`.
 The initial guesses are marked in blue.
 
-```
+```python
 In [5]: result.optimizer_result.plot().show()
 ```
 <p align="center">
   <img src="../docs/py_cic_rf_optimizer_result_plot.png" />
 </p>
  
 One can observe that the approximate gain curves are piecewise linear, with maxima
@@ -115,41 +115,37 @@
 These can be interesting to investigate the output of the algorithm further.
 
 The `changeforest` algorithm can be tuned with hyperparameters. See
 [here](https://github.com/mlondschien/changeforest/blob/287ac0f10728518d6a00bf698a4d5834ae98715d/src/control.rs#L3-L30)
 for their descriptions and default values. In Python, the parameters can
 be specified with the [`Control` class](https://github.com/mlondschien/changeforest/blob/b33533fe0ddf64c1ea60d0d2203e55b117811667/changeforest-py/changeforest/control.py#L1-L26),
 which can be passed to `changeforest`. The following will build random forests with
-20 trees:
+50 trees:
 
 ```python
 In [6]: from changeforest import Control
-   ...: changeforest(X, "random_forest", "bs", Control(random_forest_n_estimators=20))
+   ...: changeforest(X, "random_forest", "bs", Control(random_forest_n_estimators=50))
 Out[6]: 
-                            best_split max_gain p_value
-(0, 600]                           592  -11.786    0.01
- ¦--(0, 592]                       121    -6.26   0.015
- ¦   ¦--(0, 121]                    13  -14.219   0.615
- ¦   °--(121, 592]                 416   21.272   0.005
- ¦       ¦--(121, 416]             201   37.157   0.005
- ¦       ¦   ¦--(121, 201]         192   -17.54    0.65
- ¦       ¦   °--(201, 416]         207   -6.701    0.74
- ¦       °--(416, 592]             584  -44.054   0.935
- °--(592, 600]     
+                    best_split max_gain p_value
+(0, 600]                   416    7.463    0.01
+ ¦--(0, 416]               200   43.935   0.005
+ ¦   ¦--(0, 200]           193  -14.993   0.945
+ ¦   °--(200, 416]         217    -9.13   0.085
+ °--(416, 600]             591   -12.07       1 
 ```
 
-The `changeforest` algorithm still detects change points around `t=200, 400` but also
-returns two false positives.
+The `changeforest` algorithm still detects change points at `t=200`, but is slightly off
+with `t=416`.
 
 Due to the nature of the change, `method="change_in_mean"` is unable to detect any
 change points at all:
 ```python
 In [7]: changeforest(X, "change_in_mean", "bs")
 Out[7]: 
           best_split max_gain p_value
-(0, 600]         589    8.318 
+(0, 600]         589    8.625  
 ```
 
 ## References
 
-[1] M. Londschien, S. Kovács and P. Bühlmann (2022), "Random Forests for Change Point Detection", working paper.
+[1] M. Londschien, P. Bühlmann and S. Kovács (2023). "Random Forests for Change Point Detection" Journal of Machine Learning Research
```

