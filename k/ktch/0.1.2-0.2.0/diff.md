# Comparing `tmp/ktch-0.1.2.tar.gz` & `tmp/ktch-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ktch-0.1.2.tar", max compression
+gzip compressed data, was "ktch-0.2.0.tar", max compression
```

## Comparing `ktch-0.1.2.tar` & `ktch-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,31 @@
--rw-r--r--   0        0        0    11356 2021-09-20 07:55:48.345883 ktch-0.1.2/LICENSE
--rw-r--r--   0        0        0      316 2023-04-13 04:50:43.332584 ktch-0.1.2/README.md
--rw-r--r--   0        0        0      929 2022-12-11 04:56:13.380102 ktch-0.1.2/ktch/__init__.py
--rw-r--r--   0        0        0     7074 2021-09-21 01:54:32.248280 ktch-0.1.2/ktch/_template.py
--rw-r--r--   0        0        0      597 2021-09-21 01:54:18.848246 ktch-0.1.2/ktch/_version.py
--rw-r--r--   0        0        0      393 2022-08-07 05:12:34.491806 ktch-0.1.2/ktch/datasets/__init__.py
--rw-r--r--   0        0        0     9685 2023-04-08 08:40:42.385256 ktch-0.1.2/ktch/datasets/_base.py
--rw-r--r--   0        0        0        0 2022-12-11 05:38:36.524177 ktch-0.1.2/ktch/datasets/data/__init__.py
--rw-r--r--   0        0        0    46290 2022-08-04 14:54:31.590989 ktch-0.1.2/ktch/datasets/data/data_landmark_mosquito_wings.csv
--rw-r--r--   0        0        0    88299 2022-08-05 14:24:20.181451 ktch-0.1.2/ktch/datasets/data/data_outline_bottles.csv
--rw-r--r--   0        0        0   285403 2022-08-04 15:02:34.740790 ktch-0.1.2/ktch/datasets/data/data_outline_mosquito_wings.csv
--rw-r--r--   0        0        0      799 2022-08-04 14:54:31.592162 ktch-0.1.2/ktch/datasets/data/meta_landmark_mosquito_wings.csv
--rw-r--r--   0        0        0      846 2022-08-05 14:24:29.858660 ktch-0.1.2/ktch/datasets/data/meta_outline_bottles.csv
--rw-r--r--   0        0        0      792 2022-12-28 15:03:59.552650 ktch-0.1.2/ktch/datasets/data/meta_outline_mosquito_wings.csv
--rw-r--r--   0        0        0    18006 2022-08-06 16:19:26.502747 ktch-0.1.2/ktch/datasets/data/test_coef_nharm_6_norm_false_outline_bottles.csv
--rw-r--r--   0        0        0    17900 2022-08-06 16:21:05.211446 ktch-0.1.2/ktch/datasets/data/test_coef_nharm_6_norm_true_outline_bottles.csv
--rw-r--r--   0        0        0        0 2022-12-11 05:38:47.499486 ktch-0.1.2/ktch/datasets/descr/__init__.py
--rw-r--r--   0        0        0       71 2022-08-04 13:17:19.062753 ktch-0.1.2/ktch/datasets/descr/data_landmark_mosquito_wings.rst
--rw-r--r--   0        0        0       68 2022-08-05 14:26:37.531493 ktch-0.1.2/ktch/datasets/descr/data_outline_bottles.rst
--rw-r--r--   0        0        0       68 2022-08-04 15:14:08.538505 ktch-0.1.2/ktch/datasets/descr/data_outline_mosquito_wings.rst
--rw-r--r--   0        0        0     3935 2023-04-08 07:02:24.214041 ktch-0.1.2/ktch/landmark/_Procrustes_analysis.py
--rw-r--r--   0        0        0      835 2023-03-24 02:11:14.247029 ktch-0.1.2/ktch/landmark/__init__.py
--rw-r--r--   0        0        0     3992 2021-09-21 01:54:55.378710 ktch-0.1.2/ktch/landmark/_landmark.py
--rw-r--r--   0        0        0        0 2022-01-15 09:33:16.901541 ktch-0.1.2/ktch/landmark/tests/__init__.py
--rw-r--r--   0        0        0     1213 2023-03-24 03:32:50.549630 ktch-0.1.2/ktch/outline/__init__.py
--rw-r--r--   0        0        0    14124 2023-04-13 04:50:43.333810 ktch-0.1.2/ktch/outline/_elliptic_Fourier_analysis.py
--rw-r--r--   0        0        0      548 2022-08-28 14:14:38.988405 ktch-0.1.2/ktch/outline/_plot/reconstructed_shapes.py
--rw-r--r--   0        0        0     7401 2023-01-07 02:23:20.969778 ktch-0.1.2/ktch/outline/_spherical_harmonic_analysis.py
--rw-r--r--   0        0        0        0 2022-01-15 09:33:16.901733 ktch-0.1.2/ktch/outline/tests/__init__.py
--rw-r--r--   0        0        0      716 2023-04-08 14:46:24.968361 ktch-0.1.2/ktch/outline/tests/test_elliptic_Fourier_analysis.py
--rw-r--r--   0        0        0        0 2021-07-21 14:32:32.343272 ktch-0.1.2/ktch/tests/__init__.py
--rw-r--r--   0        0        0     2313 2023-04-13 04:51:27.590332 ktch-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1650 1970-01-01 00:00:00.000000 ktch-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11356 2021-09-20 07:55:48.345883 ktch-0.2.0/LICENSE
+-rw-r--r--   0        0        0      316 2023-04-13 04:50:43.332584 ktch-0.2.0/README.md
+-rw-r--r--   0        0        0      814 2023-06-01 00:37:37.601300 ktch-0.2.0/ktch/__init__.py
+-rw-r--r--   0        0        0      553 2023-05-30 07:52:28.753316 ktch-0.2.0/ktch/datasets/__init__.py
+-rw-r--r--   0        0        0    11047 2023-05-30 07:52:28.754382 ktch-0.2.0/ktch/datasets/_base.py
+-rw-r--r--   0        0        0        0 2022-12-11 05:38:36.524177 ktch-0.2.0/ktch/datasets/data/__init__.py
+-rw-r--r--   0        0        0    46290 2022-08-04 14:54:31.590989 ktch-0.2.0/ktch/datasets/data/data_landmark_mosquito_wings.csv
+-rw-r--r--   0        0        0    88299 2022-08-05 14:24:20.181451 ktch-0.2.0/ktch/datasets/data/data_outline_bottles.csv
+-rw-r--r--   0        0        0   285403 2022-08-04 15:02:34.740790 ktch-0.2.0/ktch/datasets/data/data_outline_mosquito_wings.csv
+-rw-r--r--   0        0        0      799 2022-08-04 14:54:31.592162 ktch-0.2.0/ktch/datasets/data/meta_landmark_mosquito_wings.csv
+-rw-r--r--   0        0        0      846 2022-08-05 14:24:29.858660 ktch-0.2.0/ktch/datasets/data/meta_outline_bottles.csv
+-rw-r--r--   0        0        0      792 2022-12-28 15:03:59.552650 ktch-0.2.0/ktch/datasets/data/meta_outline_mosquito_wings.csv
+-rw-r--r--   0        0        0    18006 2022-08-06 16:19:26.502747 ktch-0.2.0/ktch/datasets/data/test_coef_nharm_6_norm_false_outline_bottles.csv
+-rw-r--r--   0        0        0    17900 2022-08-06 16:21:05.211446 ktch-0.2.0/ktch/datasets/data/test_coef_nharm_6_norm_true_outline_bottles.csv
+-rw-r--r--   0        0        0        0 2022-12-11 05:38:47.499486 ktch-0.2.0/ktch/datasets/descr/__init__.py
+-rw-r--r--   0        0        0       71 2022-08-04 13:17:19.062753 ktch-0.2.0/ktch/datasets/descr/data_landmark_mosquito_wings.rst
+-rw-r--r--   0        0        0       68 2022-08-05 14:26:37.531493 ktch-0.2.0/ktch/datasets/descr/data_outline_bottles.rst
+-rw-r--r--   0        0        0       68 2022-08-04 15:14:08.538505 ktch-0.2.0/ktch/datasets/descr/data_outline_mosquito_wings.rst
+-rw-r--r--   0        0        0     5340 2023-05-30 08:44:14.197928 ktch-0.2.0/ktch/landmark/_Procrustes_analysis.py
+-rw-r--r--   0        0        0      835 2023-03-24 02:11:14.247029 ktch-0.2.0/ktch/landmark/__init__.py
+-rw-r--r--   0        0        0     3992 2021-09-21 01:54:55.378710 ktch-0.2.0/ktch/landmark/_landmark.py
+-rw-r--r--   0        0        0        0 2022-01-15 09:33:16.901541 ktch-0.2.0/ktch/landmark/tests/__init__.py
+-rw-r--r--   0        0        0     1097 2023-06-01 00:10:23.018240 ktch-0.2.0/ktch/outline/__init__.py
+-rw-r--r--   0        0        0    12904 2023-06-01 00:09:48.310946 ktch-0.2.0/ktch/outline/_elliptic_Fourier_analysis.py
+-rw-r--r--   0        0        0      690 2023-05-18 08:04:07.126268 ktch-0.2.0/ktch/outline/_plot/reconstructed_shapes.py
+-rw-r--r--   0        0        0     7401 2023-01-07 02:23:20.969778 ktch-0.2.0/ktch/outline/_spherical_harmonic_analysis.py
+-rw-r--r--   0        0        0        0 2022-01-15 09:33:16.901733 ktch-0.2.0/ktch/outline/tests/__init__.py
+-rw-r--r--   0        0        0     1763 2023-05-31 04:22:10.407679 ktch-0.2.0/ktch/outline/tests/test_elliptic_Fourier_analysis.py
+-rw-r--r--   0        0        0        0 2021-07-21 14:32:32.343272 ktch-0.2.0/ktch/tests/__init__.py
+-rw-r--r--   0        0        0     2379 2023-06-01 01:01:59.041878 ktch-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1685 1970-01-01 00:00:00.000000 ktch-0.2.0/PKG-INFO
```

### Comparing `ktch-0.1.2/LICENSE` & `ktch-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ktch-0.1.2/ktch/__init__.py` & `ktch-0.2.0/ktch/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,26 +8,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import importlib
 import types
+from pathlib import Path
+from importlib.metadata import version
+
 
 from . import landmark
 from . import outline
 
-from ._template import TemplateEstimator, TemplateTransformer, TemplateClassifier
-from ._version import __version__
-
+__version__ = version(__name__)
 
 __all__ = [
     "landmark",
     "outline",
     "datasets",
-    "TemplateEstimator",
-    "TemplateTransformer",
-    "TemplateClassifier",
     "__version__",
 ]
```

### Comparing `ktch-0.1.2/ktch/datasets/_base.py` & `ktch-0.2.0/ktch/datasets/_base.py`

 * *Files 13% similar despite different names*

```diff
@@ -280,7 +280,55 @@
 
     return Bunch(
         coef=coef,
         meta=meta,
         DESCR=fdescr,
         filename=data_file_name,
     )
+
+
+###########################################################
+#
+#   utility functions
+#
+###########################################################
+
+
+def convert_coords_df_to_list(df_coords):
+    """Convert a dataframe of coordinates to a list of numpy arrays.
+
+    Parameters
+    ----------
+    df_coords: pandas.DataFrame of index (specimen_id, coord_id), columns (axis (x, y (, z)))
+        The dataframe of coordinates.
+
+    Returns
+    -------
+    list_coords: list
+        The list of numpy arrays.
+    """
+    dim = df_coords.shape[1]
+    coords_list = [
+        df_coords.loc[specimen_id].to_numpy().reshape(-1, dim)
+        for specimen_id in df_coords.index.get_level_values(0).unique()
+    ]
+    return coords_list
+
+
+def convert_coords_df_to_df_sklearn_transform(df_coords):
+    """Convert a dataframe of coordinates to a dataframe of coordinates
+    for sklearn transformers.
+
+    Parameters
+    ----------
+    df_coords: pandas.DataFrame of index (specimen_id, coord_id), columns (axis (x, y (, z)))
+        The dataframe of coordinates.
+
+    Returns
+    -------
+    df_coords_new: pandas.DataFrame of index (specimen_id), columns (coord_id, axis)
+        The dataframe of coordinates compatible with input of scikit-learn transformers.
+    """
+
+    df_coords_new = df_coords.unstack().swaplevel(axis=1).sort_index(axis=1)
+
+    return df_coords_new
```

### Comparing `ktch-0.1.2/ktch/datasets/data/data_landmark_mosquito_wings.csv` & `ktch-0.2.0/ktch/datasets/data/data_landmark_mosquito_wings.csv`

 * *Files identical despite different names*

### Comparing `ktch-0.1.2/ktch/datasets/data/data_outline_bottles.csv` & `ktch-0.2.0/ktch/datasets/data/data_outline_bottles.csv`

 * *Files identical despite different names*

### Comparing `ktch-0.1.2/ktch/datasets/data/data_outline_mosquito_wings.csv` & `ktch-0.2.0/ktch/datasets/data/data_outline_mosquito_wings.csv`

 * *Files identical despite different names*

### Comparing `ktch-0.1.2/ktch/datasets/data/meta_landmark_mosquito_wings.csv` & `ktch-0.2.0/ktch/datasets/data/meta_landmark_mosquito_wings.csv`

 * *Files identical despite different names*

### Comparing `ktch-0.1.2/ktch/datasets/data/meta_outline_bottles.csv` & `ktch-0.2.0/ktch/datasets/data/meta_outline_bottles.csv`

 * *Files identical despite different names*

### Comparing `ktch-0.1.2/ktch/datasets/data/meta_outline_mosquito_wings.csv` & `ktch-0.2.0/ktch/datasets/data/meta_outline_mosquito_wings.csv`

 * *Files identical despite different names*

### Comparing `ktch-0.1.2/ktch/datasets/data/test_coef_nharm_6_norm_false_outline_bottles.csv` & `ktch-0.2.0/ktch/datasets/data/test_coef_nharm_6_norm_false_outline_bottles.csv`

 * *Files identical despite different names*

### Comparing `ktch-0.1.2/ktch/datasets/data/test_coef_nharm_6_norm_true_outline_bottles.csv` & `ktch-0.2.0/ktch/datasets/data/test_coef_nharm_6_norm_true_outline_bottles.csv`

 * *Files identical despite different names*

### Comparing `ktch-0.1.2/ktch/landmark/_Procrustes_analysis.py` & `ktch-0.2.0/ktch/landmark/_Procrustes_analysis.py`

 * *Files 27% similar despite different names*

```diff
@@ -40,44 +40,62 @@
     Attributes
     ------------
     mu_: ndarray, shape (n_landmarks, n_dim)
         The mean shape of the aligned shapes.
 
     Notes
     ------------
-    GPA involves translating, rotating, and scaling  the configurations to each other to minimize the sum of the squared distances with respect to positional, rotational, and size parameters, subject to a size constraint [Gower_1975]_, [Goodall_1991]_.
+    GPA for shape involves translating, rotating, and scaling  the configurations to each other to minimize the sum of the squared distances with respect to positional, rotational, and size parameters, subject to a size constraint [Gower_1975]_, [Goodall_1991]_.
+
+    GPA for size-and-shape
 
     References
     ------------
     .. [Gower_1975] Gower, J.C., 1975. Generalized procrustes analysis. Psychometrika 40, 33–51.
     .. [Goodall_1991] Goodall, C., 1991. Procrustes Methods in the Statistical Analysis of Shape. J Royal Statistical Soc Ser B Methodol 53, 285–321.
 
     """
 
-    def __init__(self, tol=10**-7, debug=False):
+    def __init__(self, tol=10**-7, scaling=True, debug=False):
         self.tol = tol
+        self.scaling = scaling
         self.debug = debug
         self.mu_ = None
 
     def fit(self, X):
         return self
 
     def transform(self, X):
-        """GPA for shapes
+        """GPA for shapes/size-and-shapes.
 
         Parameters
         ----------
         X : array-like, shape (n_shapes, n_landmarks, n_dim)
             Configurations to be aligned.
 
+        scaling: bool, default=True
+            If True, the configurations are aligned by translation, rotation, and scaling.
+            If False, the configurations are aligned by translation and rotation.
+
         Returns
         -------
         X_ : ndarray, shape (n_shapes, n_landmarks, n_dim)
-            Shapes (aligned configurations)
+            Shapes/Size-and-Shape (aligned configurations)
         """
+
+        scaling = self.scaling
+
+        if scaling:
+            X_ = self._transform_shape(X)
+        else:
+            X_ = self._transform_size_and_shape(X)
+
+        return X_
+
+    def _transform_shape(self, X):
         X_ = np.array(X, dtype=np.double, copy=True)
         X_ = self._center(X_)
         mu = np.sum(X_, axis=0) / len(X_)
         mu = mu / centroid_size(mu)
 
         diff_disp = np.inf
         total_disp_prev = np.inf
@@ -92,14 +110,42 @@
             if self.debug:
                 print("total_disp: ", total_disp, "diff_disp: ", diff_disp)
 
         self.mu_ = mu
 
         return X_
 
+    def _transform_size_and_shape(self, X):
+        X_ = np.array(X, dtype=np.double, copy=True)
+        X_ = self._center(X_)
+        mu = np.sum(X_, axis=0) / len(X_)
+
+        diff_disp = np.inf
+        total_disp_prev = np.inf
+        while diff_disp > self.tol:
+            total_disp = 0
+            X_new = np.zeros(X_.shape)
+            for i, x in enumerate(X):
+                R, scale = sp.linalg.orthogonal_procrustes(x, mu)
+                x_ = x @ R
+                total_disp += np.sum((x_ - mu) ** 2)
+                X_new[i] = x_
+            X_ = X_new
+
+            diff_disp = np.abs(total_disp_prev - total_disp)
+            total_disp_prev = total_disp
+            mu = np.sum(X_, axis=0) / len(X_)
+
+            if self.debug:
+                print("total_disp: ", total_disp, "diff_disp: ", diff_disp)
+
+        self.mu_ = mu
+
+        return X_
+
     def fit_transform(self, X):
         return self.transform(X)
 
     def _center(self, X):
         X_centered = np.array([x - np.mean(x, axis=0) for x in X])
         return X_centered
```

### Comparing `ktch-0.1.2/ktch/landmark/__init__.py` & `ktch-0.2.0/ktch/landmark/__init__.py`

 * *Files identical despite different names*

### Comparing `ktch-0.1.2/ktch/landmark/_landmark.py` & `ktch-0.2.0/ktch/landmark/_landmark.py`

 * *Files identical despite different names*

### Comparing `ktch-0.1.2/ktch/outline/__init__.py` & `ktch-0.2.0/ktch/outline/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,12 @@
 # limitations under the License.
 
 # from ._polar_Fourier_analysis import PFA
 from ._elliptic_Fourier_analysis import EllipticFourierAnalysis
 
 # from ._spherical_harmonic_analysis import SphericalHarmonicAnalysis, PCContribDisplay
 
-# from ._wavelet_analysis import WaveletAnalysis
-
-# __all__ = ['PFA', 'EllipticFourierAnalysis', 'WaveletAnalysis']
 __all__ = [
     "EllipticFourierAnalysis",
     # "SphericalHarmonicAnalysis",
     # "PCContribDisplay",
 ]
```

### Comparing `ktch-0.1.2/ktch/outline/_elliptic_Fourier_analysis.py` & `ktch-0.2.0/ktch/outline/_elliptic_Fourier_analysis.py`

 * *Files 12% similar despite different names*

```diff
@@ -72,32 +72,33 @@
     References
     ------------
     .. [Kuhl_Giardina_1982] Kuhl, F.P., Giardina, C.R. (1982) Elliptic Fourier features of a closed contour. Comput. Graph. Image Process. 18: 236–258.
 
 
     """
 
-    def __init__(self, n_harmonics=20, reflect=False, metric="", impute=False):
+    def __init__(self, n_harmonics=20, dim=2, reflect=False, metric="", impute=False):
         # self.dtype = dtype
         self.n_harmonics = n_harmonics
+        self.dim = dim
         self.reflect = reflect
         self.metric = metric
         self.impute = impute
 
-    def transform(self, X, t=None):
-        return self.fit_transform(X, t)
+    def fit_transform(self, X, t=None, norm=True):
+        return self.transform(X, t, norm=norm)
 
-    def fit_transform(self, X, t=None, norm=True, as_frame=False):
+    def transform(self, X, t=None, norm=True):
         """
 
         Fit the model with X.
 
         Parameters
         ------------
-        X: {list of array-like, array-like} of shape (n_samples, n_coords, 2)
+        X: {list of array-like, array-like} of shape (n_samples, n_coords, dim)
             Coordinate values of n_samples.
             The i-th array-like of shape (n_coords_i, 2) represents
             2D coordinate values of the i-th sample.
 
         t: array-like of shape (n_samples, n_coords), optional
             Parameters indicating the position on the outline of n_samples.
             The i-th ndarray of shape (n_coords_i, ) corresponds to
@@ -111,63 +112,44 @@
         as_frame: bool, default=False
             Return the result as a pandas DataFrame.
 
         Returns
         ------------
         X_transformed: array-like of shape (n_samples, (1+2*n_harmonics)*n_dim)
             Returns the array-like of coefficients.
+            (a_0, a_1, ..., a_n, b_0, b_1, ..., b_n, , c_0, c_1, ..., c_n, , d_0, d_1, ..., d_n)
 
         """
-
-        n_harmonics = self.n_harmonics
+        dim = self.dim
 
         if t is None:
             t_ = [None for i in range(len(X))]
 
         if len(t_) != len(X):
             raise ValueError("t must have a same length of X ")
 
-        if as_frame:
-            X_transformed = pd.concat(
-                [
-                    self._fit_transform_single(X[i], t=t_[i], norm=norm, as_frame=True)
-                    for i in range(len(X))
-                ],
-                axis=0,
-            )
-            X_transformed["specimen_id"] = [
-                i for i in range(len(X)) for j in range(n_harmonics + 1)
+        if isinstance(X, pd.DataFrame):
+            X_ = [
+                row.dropna().to_numpy().reshape(dim, -1).T for idx, row in X.iterrows()
             ]
-            X_transformed = X_transformed.reset_index().set_index(
-                ["specimen_id", "harmonics"]
-            )
         else:
-            if isinstance(X, pd.DataFrame):
-                X_ = [x[0] for x in X.to_numpy()]
-            else:
-                X_ = X
+            X_ = X
 
-            X_transformed = np.stack(
-                [
-                    self._fit_transform_single(
-                        np.array(X_[i]), t_[i], norm=norm, as_frame=False
-                    )
-                    for i in range(len(X))
-                ]
-            )
+        X_transformed = np.stack(
+            [self._transform_single(X_[i], t_[i], norm=norm) for i in range(len(X_))]
+        )
 
         return X_transformed
 
-    def _fit_transform_single(
+    def _transform_single(
         self,
         X,
         t=None,
         norm=True,
         duplicated_points="infinitesimal",
-        as_frame=False,
     ):
         """Fit the model with a signle outline.
 
         Parameters
         ----------
         X: array-like of shape (n_coords, 2)
                 Coordinate values of an 2D outline.
@@ -240,25 +222,15 @@
         bn = _sse(dx, dt, n_harmonics)
         cn = _cse(dy, dt, n_harmonics)
         dn = _sse(dy, dt, n_harmonics)
 
         if norm:
             an, bn, cn, dn = self._normalize(an, bn, cn, dn)
 
-        if as_frame:
-            harmonics = pd.Series([i for i in range(n_harmonics + 1)])
-            df_a = pd.DataFrame(an, index=harmonics)
-            df_b = pd.DataFrame(bn, index=harmonics)
-            df_c = pd.DataFrame(cn, index=harmonics)
-            df_d = pd.DataFrame(dn, index=harmonics)
-            X_transformed = pd.concat([df_a, df_b, df_c, df_d], axis=1)
-            X_transformed.columns = ["an", "bn", "cn", "dn"]
-            X_transformed.index.name = "harmonics"
-        else:
-            X_transformed = np.concatenate([an, bn, cn, dn])
+        X_transformed = np.hstack([an, bn, cn, dn])
 
         return X_transformed
 
     def _normalize(self, an, bn, cn, dn):
         a1 = an[1]
         b1 = bn[1]
         c1 = cn[1]
@@ -394,19 +366,14 @@
         return feature_names_out
 
     @property
     def _n_features_out(self):
         """Number of transformed output features."""
         return (self.n_harmonics + 1) * 4
 
-    def set_output(
-        self, *, transform: None | Literal["default", "pandas"] = None
-    ) -> BaseEstimator:
-        return super().set_output(transform=transform)
-
 
 ###########################################################
 #
 #   utility functions
 #
 ###########################################################
```

### Comparing `ktch-0.1.2/ktch/outline/_plot/reconstructed_shapes.py` & `ktch-0.2.0/ktch/outline/_plot/reconstructed_shapes.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,31 @@
 class PCContribDisplay:
-    """"""
+    """Plot shape variation along PC axes.
+
+    Parameters
+    ----------
+    pca : PCA
+        Fitted PCA object.
+
+
+    Returns
+    ----------
+
+
+
+
+    """
 
     def __init__(self, pca, *, display_labels=None) -> None:
         self.pca = pca
         self.display_labels = display_labels
 
     def plot(
-        self, *, n_PCs=(1, 2, 3), sd_values=(-2, -1, 0, 1, 2), , ax=None, im_kw=None
+        self, *, n_PCs=(1, 2, 3), sd_values=(-2, -1, 0, 1, 2), ax=None, im_kw=None
     ):
-
         return self
 
     @classmethod
     def from_estimators(cls, estimator, X, y, *, labels=None):
         return cls.from_predictions()
 
     @classmethod
```

### Comparing `ktch-0.1.2/ktch/outline/_spherical_harmonic_analysis.py` & `ktch-0.2.0/ktch/outline/_spherical_harmonic_analysis.py`

 * *Files identical despite different names*

### Comparing `ktch-0.1.2/pyproject.toml` & `ktch-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -16,56 +16,64 @@
 description = "**ktch** is a python package for model-based morphometrics."
 homepage = "https://doc.ktch.dev/index.html"
 keywords = ["morphometrics", "theoretical morphology"]
 license = "Apache-2.0"
 name = "ktch"
 readme = "README.md"
 repository = "https://github.com/noshita/ktch"
-version = "0.1.2"
+version = "0.2.0"
 
 [tool.poetry.dependencies]
 numpy = "^1.22"
 pandas = "^1.4"
 python = ">= 3.8, < 3.12"
 scikit-learn = "^1.2"
 scipy = "^1.8"
+toml = "^0.10"
 
 [tool.poetry.extras]
-docs = ["sphinx", "sphinx-gallery", "sphinx_rtd_theme", "numpydoc", "matplotlib", "toml"]
+docs = [
+  "sphinx",
+  "sphinx-gallery",
+  "sphinx_rtd_theme",
+  "numpydoc",
+  "matplotlib", # "toml"
+]
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 autopep8 = "^1.6.0"
 flake8 = "^5.0.4"
 invoke = "^1.4.1"
 jupyter = "^1.0.0"
 jupyterlab = "^3.4.4"
+jupytext = "^1.14.5"
 liccheck = "^0.7.2"
+llvmlite = "^0.39.1"
 matplotlib = "^3.5.2"
+module-name = "^0.6.0"
+myst-nb = "^0.17.2"
+nbsphinx = "^0.9.2"
+numba = "^0.56.4"
 numpydoc = "^1.4.0"
+opencv-python = "^4.7.0.68"
 plotly = "^5.9.0"
 poetry2conda = "^0.3.0"
 pydata-sphinx-theme = "^0.12"
 pytest = "^7.1"
 pytest-cov = "^3.0"
 seaborn = "^0.11.0"
+setuptools = "<60.0"
 sphinx = "^5.3"
 sphinx-autobuild = "^2021.3"
 sphinx-gallery = "^0.11"
-sphinxcontrib-bibtex = "^2.5"
-toml = "^0.10"
-xarray = "^2022.6.0"
-
-[tool.poetry.group.dev.dependencies]
-llvmlite = "^0.39.1"
-numba = "^0.56.4"
-opencv-python = "^4.7.0.68"
-setuptools = "<60.0"
 sphinx-notfound-page = "^0.8.3"
+sphinxcontrib-bibtex = "^2.5"
 tqdm = "^4.64.1"
 tslearn = "^0.5.3.2"
+xarray = "^2022.6.0"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
 
 [tool.poetry2conda]
 name = "ktch"
```

### Comparing `ktch-0.1.2/PKG-INFO` & `ktch-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ktch
-Version: 0.1.2
+Version: 0.2.0
 Summary: **ktch** is a python package for model-based morphometrics.
 Home-page: https://doc.ktch.dev/index.html
 License: Apache-2.0
 Keywords: morphometrics,theoretical morphology
 Author: Noshita, Koji
 Author-email: noshita@morphometrics.jp
 Requires-Python: >=3.8,<3.12
@@ -25,14 +25,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Provides-Extra: docs
 Requires-Dist: numpy (>=1.22,<2.0)
 Requires-Dist: pandas (>=1.4,<2.0)
 Requires-Dist: scikit-learn (>=1.2,<2.0)
 Requires-Dist: scipy (>=1.8,<2.0)
+Requires-Dist: toml (>=0.10,<0.11)
 Project-URL: Repository, https://github.com/noshita/ktch
 Description-Content-Type: text/markdown
 
 # ktch - A python package for model-based morphometrics
 
 [![codecov](https://codecov.io/gh/noshita/ktch/branch/main/graph/badge.svg?token=SJN66K7KJY)](https://codecov.io/gh/noshita/ktch)
```

